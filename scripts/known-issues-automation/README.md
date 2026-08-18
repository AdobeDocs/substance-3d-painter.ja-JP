---
source-git-commit: 0376fe6500551442b28831d5742ecbbc9363ab19
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 1%

---
# 既知の問題Generator — Substance 3D Painter

Substance 3D Painterのマークダウン文書の既知の問題の生成を自動化します。この文書は以下で公開されています。
`https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html`

問題はJiraの叙事詩`SBSFOUR-6267`から取得されています。 このスクリプトは、すべての問題を取得し、ターゲットバージョンで既に修正されている内容をフィルターで除外し、コミット可能なフォーマットされたマークダウンファイルを出力します。

&#x200B;---

## クイックスタート

これらの手順は、以下の1回限りの設定が既に完了していることを前提としています。

1. **GlobalProtect VPN**&#x200B;に接続
2. `.env`ファイルの`TARGET_VERSION`を、ドキュメントを生成しているバージョンに設定します（例： `12.0.3`）
3. `scripts/known-issues-automation/`ディレクトリからスクリプトを実行します：

   ```
   python fetch_known_issues.py
   ```

4. 出力の概要を確認 – フェッチされた問題の数と除外された問題の数が報告されます。
5. 生成された`known-issues.md`を`help/release-notes/known-issues.md`にコピー

> 不足している問題や予期しない問題がある場合は、`raw_issues.json`を調べて、フィルターが適用される前にJiraが返した内容を確認してください。

&#x200B;---

## 1回限りの設定

### &#x200B;1. 依存関係のインストール

```bash
pip install requests python-dotenv
```

### &#x200B;2. `.env`ファイルを作成

```bash
cp .env.example .env
```

### &#x200B;3. Jiraパーソナルアクセストークンを取得

1. `https://jira.corp.adobe.com`にログイン
2. 左側のサイドバー→**パーソナルアクセストークン**&#x200B;のプロファイルに移動します
3. **トークンの作成**&#x200B;をクリックし、名前を指定して、生成された値をコピーします

> PATはブラウザーセッションが終了しても期限切れにならず、スクリプト化されたAPIアクセスのセッションクッキーよりも信頼性が高くなります。

### &#x200B;4. `.env`ファイルに入力

```
JIRA_PAT=your-personal-access-token
TARGET_VERSION=12.0.3
OUTPUT_FILE=known-issues.md
```

`TARGET_VERSION`は、既知の問題のページを生成しているSubstance 3D Painterのバージョンです。 除外する修正済みの問題を制御します。以下の[フィルターロジック](#filtering-logic)を参照してください。

&#x200B;---

## リポジトリ構造

```
.
├── README.md                  # This file
├── fetch_known_issues.py      # Main script
├── .env.example               # Environment variable template (safe to commit)
├── .env                       # Your local credentials — never commit this
├── raw_issues.json            # Raw Jira dump from last run — gitignored
└── known-issues.md            # Generated output from last run — gitignored
```

&#x200B;---

## Jiraリファレンス

| フィールド | Value |
|---|---|
| Jiraインスタンス | `https://jira.corp.adobe.com` |
| プロジェクトキー | `SBSFOUR` |
| 既知の問題の説明 | `SBSFOUR-6267` |

生成されたドキュメントに表示されるためには、すべての既知の問題をこのエピックにリンクする必要があります。 問題をページに追加またはページから削除する必要がある場合は、マークダウンを手動で編集するのではなく、Jiraで記事を更新します。

&#x200B;---

## スクリプトの仕組み

### ステップ1：フェッチ

このスクリプトは、JQLを使用してJira REST APIにクエリを実行します。

```
"Epic Link" = SBSFOUR-6267 ORDER BY created ASC
```

結果はページごとに50件の問題でページネーションされます。 各問題について次のフィールドが取得されます： `summary`、`issuetype`、`status`、`affectedVersions`、`fixVersions`、`labels`。

認証で`JIRA_PAT`からのベアラートークンが使用されています。 企業のJiraインスタンスは内部SSL証明書を使用しているため、これらのリクエストに対する証明書の検証は無効になっています。これは、Adobeネットワークで予期される動作です。

### ステップ2：未処理ダンプ

フィルター処理または書式設定の前に、スクリプトは`raw_issues.json`を書き込みます。 これは、Jiraが返したすべての問題の簡易化されたスナップショットであり、次に何が起こるかに関係なく、常に生成されます。 出力が間違っているように見える場合は、まずこのファイルを調べてください – これはJiraが提供したデータを正確に示します。

### ステップ3：フィルタ

同時に適用される2つのルールを使用して問題をフィルタリングします。

1. **状態フィルター** – アクティブな既知の問題は、`Backlog`と`Dev In Progress`の問題のみです。 ステータス`Fixed`の問題は除外の対象の候補であり、以下のバージョンチェックが対象となります。

2. **バージョンフィルター** — `Fixed`の問題は、その修正バージョンの1つが`TARGET_VERSION`以下の場合にのみ除外されます。 修正のバージョンが`TARGET_VERSION`より高い場合は、文書化されているバージョンに修正が出荷されていないため、問題は引き続き含まれます。

これは、2つのバージョンが同時に開発されている場合に対応します。`12.1.0`で修正された問題は、`12.0.3`の既知の問題として残ります。

完全な決定テーブルについては、[フィルター処理ロジック](#filtering-logic)を参照してください。

### 手順4 – カテゴリを解析する

各問題の概要は、文字列の先頭でカテゴリータグについて解析されます。

- `[Shader] Some description`→カテゴリ： `["Shader"]`、説明： `"Some description"`
- `[Crash][Engine] Some description`→カテゴリ： `["Crash", "Engine"]`、説明： `"Some description"`
- `No brackets here`にはカテゴリが→りません。カテゴリなし扱いになります

**主カテゴリ**&#x200B;は常に最初のタグです。 これにより、グループ化とセクションの配置が決まります。

### 手順5：グループ化と並べ替え

課題の構成は次のとおりです。

- 案件は主なカテゴリ別にグループ化されています
- グループは、案件数で降順にソートされます（最大のグループが最初）。
- 複数の懸案事項を含むグループがドキュメントの上部に表示されます
- 1つの案件のみ含み、カテゴリに分類されていない案件があるグループは、セクションヘッダーのない複数の案件のグループの後に表示されます
- `[Crash]`を主カテゴリとする問題は、常に最後の`## Stability`セクションに配置されます

### ステップ6：フォーマットと書き込み

スクリプトは`known-issues.md`を次の内容で出力します：

- YAML frontmatter （helpxメタデータ）
- ターゲットバージョンを指定するイントロ段落を含む`# Known issues`見出し
- 形式が`` * `[Category]` Description ``の問題
- マルチカテゴリの問題： `` * `[Category1]` `[Category2]` Description ``
- カテゴリグループ間の空白行
- クラッシュの問題に関する`## Stability`セクションの最後

&#x200B;---

## フィルタリングロジック

| ステータス | バージョンセットを修正しますか？ | バージョンとターゲットの修正 | 含まれる？ |
|---|---|---|---|
| `Backlog` | — | — | はい |
| `Dev In Progress` | — | — | はい |
| `Fixed` | いいえ | — | いいえ（保守的に除外） |
| `Fixed` | はい | ターゲット≤バージョンの修正 | いいえ（出荷済み） |
| `Fixed` | はい | 修正バージョン/ターゲット | 〇（修正は将来のバージョンで提供） |

&#x200B;---

## 出力形式

```markdown
---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html"
...
---

# Known issues

This page lists all the active known issues present in v12.0.3 of Substance 3D Painter:

* `[Engine]` Error when using Smart Materials if Texture Set has no tile 1001
* `[Engine]` Geometry mask shows artifacts at UV borders with instanced layers

* `[Shader]` user0 channel always can not be read as sRGB with specific shader

* `[Export]` GLTF exports at the wrong size
* `[Import]` Cannot import obj file with "nan" values

## Stability

* `[Crash]` Select "Export mesh" when mesh failed to load
```

**書式設定上の注意：**&#x200B;カテゴリタグは、2つのバックティックではなく、1つのバックティックの折り返しを使用します – `` `[Category]` ``。 従来の手動で管理されるドキュメントには、二重バックチェックエラーが含まれていました。このスクリプトでは、常に正しい形式が生成されます。

&#x200B;---

## トラブルシューティング

**401許可されていません**
- **GlobalProtect VPN**&#x200B;に接続していることを確認します
- お客様のPATは有効期限が切れているか取り消された可能性があります – `https://jira.corp.adobe.com/secure/ViewProfile.jspa`に新しいPATを生成し、`.env`を更新してください

**`JIRA_PAT is not set`エラー**
- `.env.example`から`.env`ファイルを作成し、トークンを入力したことを確認してください
- `python-dotenv`が`.env`ファイルを見つけられるように、`scripts/known-issues-automation/`ディレクトリ内からスクリプトを実行していることを確認してください

**出力に問題が見つかりません**
- `raw_issues.json`を確認してください。問題がない場合、Jiraのエピック`SBSFOUR-6267`にリンクされていません。
- 問題が`raw_issues.json`にあるが出力にない場合、フィルターによって除外されました。その状態を確認し、`TARGET_VERSION`に対してバージョンを修正してください

実行時の&#x200B;**`TARGET_VERSION`警告**
- このスクリプトは実行されますが、`TARGET_VERSION`が設定されていない場合は、すべての`Fixed`件の問題が控えめに除外されます。 最終的な文書を生成する前に、必ず設定してください。
