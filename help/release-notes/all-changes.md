---
breadcrumb-title: ''
description: Substance 3D Painterのすべてのバージョンに加えられた変更とアップデートを確認し、機能の進化と改善点を経時的に追跡します。
title: すべての変更
user-guide-description: ''
user-guide-title: ''
source-git-commit: 479eb327180dd223bbff362e3f200995565cbcfa
workflow-type: tm+mt
source-wordcount: '40779'
ht-degree: 0%
---

# すべての変更

Substance 3D Painterの以前のすべてのリリースのリリースノートが、最新のものから古いものへと並べ替えられて記載されています。

>[!NOTE]
>
> Painterに影響を与える可能性がある既知の問題を確認するには、[専用のドキュメントページ](known-issues.md)を参照してください。

## バージョン12

### 12.2.0

リリース日： **2026/10/21**

概要： **この更新プログラムはメジャーリリースであり、ベイク用の新しいケージペイント機能が追加され、ポリゴンの塗りつぶし機能が強化されています。 詳細については、完全なリリースノートを参照してください。**

**追加：**

* ベイク、ケージペイント
* &amp;lbrack;ケージペイント&amp;rbrack；基本ケージペイント UIを作成
* &amp;lbrack;ケージペイント&amp;rbrack；新しいケージ表示オプション
* &amp;lbrack;ケージペイント&amp;rbrack；編集可能な選択/塗りつぶしツール
* &amp;lbrack;ケージペイント&amp;rbrack;ツールバーにブレンドモードを表示
* &amp;lbrack;ケージペイント&amp;rbrack; HDRスライダUIの変更
* &amp;lbrack;ケージペイント&amp;rbrack;ビジュアライゼーションシェーダー
* &amp;lbrack;ケージペイント&amp;rbrack; スタックのリセットオプション
* 多角形フィルツールの改善
* &amp;lbrack；ポリゴンフィル&amp;rbrack;ポリゴンパッチを追加
* &amp;lbrack；ポリゴンフィル&amp;rbrack;ポリゴンループを追加
* &amp;lbrack；ポリゴンフィル&amp;rbrack; 対称サポート（ループ/パッチ）
* &amp;lbrack；ポリゴンフィル&amp;rbrack;対称エッジプレビュー
* &amp;lbrack；ポリゴンフィル&amp;rbrack;ループと部分ループのある三角形を削除
* &amp;lbrack；ポリゴンフィル&amp;rbrack;アクティブなテクスチャセットのみに表示されるワイヤーフレーム
* &amp;lbrack；ポリゴンフィル&amp;rbrack；クリックできない三角形の赤いエッジハイライト
* &amp;lbrack；ポリゴン塗りつぶし&amp;rbrack；塗りつぶしモードのオプションを無効にしない
* &amp;lbrack；ポリゴンフィル&amp;rbrack；すべてのチャンネルプロパティをポリゴンフィルで設定できるようにします
* &amp;lbrack；ポリゴン塗りつぶし&amp;rbrack；前のストロークを再開は、ポリゴン塗りつぶしで機能します
* &amp;lbrack；ポリゴンフィル&amp;rbrack;アクティブでないテクスチャセット上に禁止カーソルを表示
* &amp;lbrack；ポリゴンフィル&amp;rbrack; ALTインスタントプレビュー
* &amp;lbrack；ポリゴンフィル&amp;rbrack;ポリループへの一時的な切り替え用ショートカット(SHIFT+A)
* &amp;lbrack;ビューポート&amp;rbrack; テクスチャセット/UV タイル選択ハイライトを表示
* &amp;lbrack;ビューポート&amp;rbrack;リアルタイムビューポートでOrder Independent Transparencyのサポートを追加
* &amp;lbrack；ディスプレイ設定&amp;rbrack；ディスプレイ設定を新しいグループに再編成する
* &amp;lbrack；ツール&amp;rbrack;ブラシストロークに加算描画のサポートを追加
* &amp;lbrack；ツール&amp;rbrack；多角形の塗りつぶしで加算ブレンドのサポートを追加
* &amp;lbrack;USD&amp;rbrack；書き出したUSDを不透明度マップと一緒に使用すると、Arnoldですべての透明度がレンダリングされる
* &amp;lbrack;Nvidia&amp;rbrack；最新のNvidiaドライバー(616.56 ～ 617.14)に関する警告の追加
* 新しい「メッシュ_uv_neighbor」エンジンマップ入力を追加
* ベイカーをバージョン3.23.0に更新する
* エンジンをバージョン9.6.1にアップデートする

**修正済み：**

* &amp;lbrack;ベイク処理&amp;rbrack; Ambient occlusion名で背面を無視が機能しない
* &amp;lbrack;ベイク処理&amp;rbrack; &amp;lbrack;AMD&amp;rbrack;デバイスがヘビーハイポリメッシュでベイク処理すると失われる
* &amp;lbrack；パフォーマンス&amp;rbrack; Painter hogs VRAM usage
* &amp;lbrack;ビューポート&amp;rbrack; HDPI画面でプロジェクトを開く際にテクスチャが見つからない
* &amp;lbrack;Tool&amp;rbrack;マスクでペイントすると描画モードがグレー表示になる
* ネットワークへの書き出し後、一時フォルダーが削除されない
* &amp;lbrack;USD&amp;rbrack；書き出されたUSDジオメトリは、UV境界に沿って分割されます。
* &amp;lbrack;USD&amp;rbrack；不正な形式のUSDzをロードするとフリーズする

### 12.1.5

リリース日： **2026/09/15**

概要： **マイナーリリース**

**修正済み：**

* シェルフからネットワークへのイメージの書き出しが機能しない
* &amp;lbrack;Generator&amp;rbrack; 「テクスチャを使用」をfalseに設定しても、テクスチャ入力の使用は無効になりません
* 3d 投影の編集中にビューポートがフリーズする
* マテリアルレイヤーの解像度が低すぎます

### 12.1.4

リリース日： **2026/09/04**

概要： **マイナーリリース**

**修正済み：**

* ファイル名に非ASCII文字が含まれているファイルをインポートまたはエクスポートするときの&amp;lbrack;クラッシュ&amp;rbrack;クラッシュ

### 12.1.3

リリース日： **2026/08/26**

概要： **マイナーリリース**

**追加：**

* エンジンをバージョン9.4.6にアップデートする

**修正済み：**

* &amp;lbrack；グレースケールピッカー&amp;rbrack;ツールを変更した後もピッカーが開いたままになる
* &amp;lbrack；ゆがみベイク処理&amp;rbrack;ゆがみ補正がペイントおよび元に戻すときに壊れる(&amp;R)
* &amp;lbrack;投影ツール&amp;rbrack; ビューポートのインタラクションが投影ツールによってブロックされています
* &amp;lbrack;Dynamic Stroke&amp;rbrack;ブラシプロパティにDynamic Strokeパラメータがありません
* ネットワークへの書き出しが機能しない

### 12.1.2

リリース日： **2026/08/03**

概要： **マイナーリリース**

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack;レンダリング時にクラッシュが発生するSubstanceもあります
* &amp;lbrack;クラッシュ&amp;rbrack;ベイクモードでの再読み込みメッシュ
* &amp;lbrack;クラッシュ&amp;rbrack;グラフィックディスプレイの初期化に失敗すると、クラッシュが発生する可能性があります
* &amp;lbrack;クラッシュ&amp;rbrack;ログの更新中にテクスチャの書き出しがクラッシュすることがある
* &amp;lbrack;クラッシュ&amp;rbrack; 環境マップの読み込み/アップデート時にベイクモードでクラッシュが発生する場合がある
* &amp;lbrack;ベイク処理&amp;rbrack；高ポリゴンファイルを修正した後に烘焙を再起動すると、フリーズする場合がある
* &amp;lbrack;Photoshopに送る&amp;rbrack;レイヤーのマスクを書き出せない
* &amp;lbrack;エンジン&amp;rbrack;アンカーポイントの結果が、マスクとカラーチャンネル間でレンダリングされない

### 12.1.1

リリース日： **2026/07/09**

概要：マイナーリリース

追加：

* &amp;lbrack；スキューベイク&amp;rbrack;スキューの基準法線モードを表示: メッシュまたは三角形ごと
* &amp;lbrack；プロパティ&amp;rbrack;均一カラーを常にチャンネルのデフォルト値にリセットする
* &amp;lbrack;OpenPBR&amp;rbrack; 出力テンプレートを作成するために、書き出しテクスチャウィンドウでカテゴリ別にチャンネルを再編成する
* エンジンをバージョン9.4.5にアップデートする

修正：

* &amp;lbrack；プロジェクト&amp;rbrack；一部のプロジェクトを開いたり保存したりするのに通常より時間がかかることがあります
* &amp;lbrack;クラッシュ&amp;rbrack；複数のメッシュを再読み込みするとクラッシュが発生する場合がある
* &amp;lbrack;クラッシュ&amp;rbrack;マスクビューモードでチャンネルを削除するとクラッシュが発生する
* &amp;lbrack;クラッシュ&amp;rbrack;レンダリング時にクラッシュが発生するSubstanceもあります
* &amp;lbrack;ペイントのゆがみ&amp;rbrack;ペイントモードに切り替えても、ペイントのゆがみ内の選択したツールが選択されたままになる
* &amp;lbrack；共通設定のベイク&amp;rbrack; ケージ距離の設定で、ケージワイヤーフレームとシェーダービジュアライゼーションが更新されない
* &amp;lbrack;エンジン&amp;rbrack; UVパディング「3Dスペース隣接」モードが細い三角形で適切に機能しない
* &amp;lbrack;エンジン&amp;rbrack;アンカーポイントの結果が、マスクとカラーチャンネル間でレンダリングされない

### 12.1.0

リリース日： **2026/06/23**

概要： **このアップデートはメジャーリリースであり、新しいベイク処理の既定のUIステート、スキュー地図のペイント、自動リベイク処理、ハードサーフェスメッシュおよびOpenPBRの自動UVラップ解除の新しいオプションを含むベイカーの機能強化が含まれています。 詳細については、完全なリリースノートを参照してください。**

**追加済み**:

* &amp;Lbrack；ゆがみベイク&amp;Rbrack；ゆがみペイントツール
* &amp;lbrack；ゆがみベイク&amp;rbrack；ゆがみマップをペイントする際のゆがみプレビューシェーダーとゆがみ方向ベクタービジュアルを追加
* &amp;lbrack；スキューベイク処理&amp;rbrack;エッジ保護オプションを追加
* &amp;lbrack；スキューベイク処理&amp;rbrack; Auto rebake
* &amp;lbrack；スキューベイク処理&amp;rbrack; メッシュマップリストUIをリワーク(&amp;R)
* &amp;lbrack；スキューベイク&amp;rbrack; メッシュマップを分割/共通ベイク設定+共通設定をメッシュマップリストから移動（ベースカラーまたはマスクのみ）
* &amp;lbrack；スキューベイク処理&amp;rbrack; 「ビューポートを変更」ツールバーボタン
* &amp;lbrack；スキューベイク処理&amp;rbrack;ブラシの対称トグルを上部ツールバーに表示
* &amp;lbrack；スキューベイク&amp;rbrack; メッシュマップリストの同期メニューの「オプション名を変更」
* &amp;lbrack；スキューベイク&amp;rbrack; 「同期」ダイアログと「チェック済み」ダイアログを更新
* &amp;lbrack；スキューベイク処理&amp;rbrack;グレースケールカラーピッカーバリアントを作成
* &amp;lbrack；スキューベイク処理&amp;rbrack;ベイク処理モードアイコンを更新
* &amp;lbrack；自動ラップ解除&amp;rbrack;ハードサーフェスを統合オプション
* &amp;lbrack;OpenPBR&amp;rbrack; OpenPBR 1.1のサポートを追加
* &amp;lbrack;OpenPBR&amp;rbrack; OpenPBRをデフォルトのワークフローとシェーダーにする
* &amp;lbrack;OpenPBR&amp;rbrack; USDを介したOpenPBRマテリアルとテクスチャの読み込み
* &amp;lbrack;OpenPBR&amp;rbrack; USDを介したOpenPBRマテリアルとテクスチャの書き出し
* &amp;lbrack;OpenPBR&amp;rbrack; OpenPBRの命名規則を表示するために書き出しテクスチャウィンドウを更新
* &amp;lbrack;OpenPBR&amp;rbrack;サポートOpenPBRの変更に関するドキュメントを追加する
* &amp;lbrack;OpenPBR&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Iray内のOpenPBR 1.1をサポートする新しいMDLを追加
* USDの書き出しに関するいくつかのマイナーな改善
* &amp;lbrack;UI&amp;rbrack；別のテクスチャセットにペイントしようとすると、ビューポートに警告が表示される(&amp;R)
* &amp;lbrack；平坦化&amp;rbrack;テクスチャセット間でインスタンス化されたすべてのレイヤーを平坦化できるようにします
* &amp;lbrack;テクスチャセット設定&amp;rbrack；新しいウィンドウで複数のチャンネルを一度に選択できるようにします
* &amp;lbrack;History&amp;rbrack; 「value」を更新パラメータ名を反映するエントリ語を元に戻す
* &amp;lbrack;レイヤースタック&amp;rbrack;マスクの塗りつぶし効果をデフォルトで白(1.0)にする
* &amp;lbrack;Substance&amp;rbrack；新しい「メッシュハードのエッジの三角形」エンジンマップ入力を追加
* &amp;lbrack;Substance&amp;rbrack；新しい「メッシュハードエッジ」エンジンマップ入力を追加
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーインスタンスが同じ名前を使用できないようにする
* &amp;lbrack;シェーダー&amp;rbrack; USDまたはGLTFファイルを読み込むときに、プロジェクトテンプレートのシェーダーを使用します
* Adobe Color Engineをバージョン7.0にアップデートする
* MacOS Xの最小バージョンを13.0にアップグレード(Ventura)
* &amp;lbrack;Content&amp;rbrack; OpenPBR用の新しいプロジェクトテンプレート
* &amp;lbrack;Content&amp;rbrack；新しいシェーダーを使用するようにサンプルプロジェクトを更新する
* &amp;lbrack;Python&amp;rbrack;ジオメトリマスクAPIを拡張してUIのような包含モードと除外モードを許可

**固定**:

* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;メッシュマップ設定&amp;rbrack；他のテクスチャセットに設定を適用
* &amp;lbrack;クラッシュ&amp;rbrack;ワールド空間法線なしでマップから曲率をベイクする場合
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;ベイク処理&amp;rbrack;カスタムケージが有効になっているが、ファイルが選択されていないクラッシュでのベイク処理
* &amp;lbrack;クラッシュ&amp;rbrack; AO ベイク処理をキャンセルする
* &amp;lbrack；自動ケージ&amp;rbrack；高ポリゴンファイルパスが無効な場合の無限荷重
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;Windows&amp;rbrack;カラーピッカーが完全に黒くなったり、表示されない場合がある
* &amp;lbrack；ポリゴン塗りつぶしツール&amp;rbrack；このツールは非PBRでは機能しません
* &amp;lbrack;&amp;lbrack;ペイント&amp;rbrack; base colorチャンネルを削除しても、以前にペイントしたカラーが削除されない
* &amp;lbrack;USD&amp;rbrack; シェーダーインスタンスがすべて正しく検出されない
* &amp;lbrack;Substance&amp;rbrack；入出力ノードの最初の使用のみが考慮されます
* &amp;lbrack;シェーダー&amp;rbrack;Ambient occlusionが、異なるミキシング方式を使用するテクスチャセットで2回適用される
* &amp;lbrack;エンジン&amp;rbrack；青チャンネルが空（黒）の通常のテクスチャでは、正しいブレンド結果が得られない場合がある
* &amp;lbrack;GLTF Import&amp;rbrack;アルファブレンディングは、すべてのテクスチャセットで有効になっています
* &amp;lbrack;GLTF書き出し&amp;rbrack;アルファブレンディングは、書き出し時に常に有効になります
* &amp;lbrack;Export&amp;rbrack；両面ジオメトリは、GLTFファイルを読み込むときに常に無効になります。
* &amp;lbrack;Javascript&amp;rbrack;シェーダ設定の変更が取り消し履歴に影響しない
* &amp;lbrack;Samples&amp;rbrack; 表面化散乱がMeet Matの[表示設定]で有効になっていません

### 12.0.3

リリース日： **2026/05/05**

概要： **マイナーリリース**

**追加：**

* ベイカーをバージョン3.22.2に更新する
* エンジンをバージョン9.4.3にアップデートする
* &amp;lbrack;Python&amp;rbrack; スマートマテリアルを指定の場所に保存

**修正済み：**

* &amp;lbrack;Ubuntu&amp;rbrack; マテリアル選択時のクラッシュ
* &amp;lbrack;Mac&amp;rbrack；他のアプリデータへのアクセスを求める繰り返しポップアップが表示される
* &amp;lbrack;ベイク処理&amp;rbrack;アーティファクトが曲率マップに表示される可能性がある
* &amp;lbrack;ベイク処理&amp;rbrack;ベイク処理が遅くなる場合がある(&amp;rbrack;)
* &amp;lbrack；ジオメトリへのワープ&amp;rbrack;ジオメトリへのワープが無効になる場合がある
* &amp;lbrack;UV タイル&amp;rbrack；抽出されたアンカーポイントのアルファが他のタイルで無視される
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; PythonコンソールのSSL付き例外
* &amp;lbrack;Python&amp;rbrack；残りのQtウィジェットで終了時にPainterがクラッシュする

### 12.0.2

リリース日： **2026/04/07**

概要： **マイナーリリース**

**追加：**

* &amp;lbrack；カラーマネジメント&amp;rbrack；新規OCIOを追加してカラーピッカーのデフォルトのカラースペースを指定
* &amp;lbrack;Python&amp;rbrack; Python APIでの自動ラップ解除の表示

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack;ディスク容量が不足して保存すると、プロジェクトがクラッシュしたり壊れたりすることがあります
* &amp;lbrack;クラッシュ&amp;rbrack; &amp;lbrack；リボン&amp;rbrack;リボンを使用すると、一部のプロジェクトでクラッシュが発生する場合があります
* &amp;lbrack;クラッシュ&amp;rbrack; &amp;lbrack;ベイク&amp;rbrack; クラッシュ（.assbinファイルをフォルダーに書き込めない場合）
* &amp;lbrack;StagerからのImport&amp;rbrack; OBJ メッシュがプロジェクトの作成時に失敗することがある
* &amp;lbrack;Import&amp;rbrack; OBJの面が見つからない場合がある
* &amp;lbrack;Import&amp;rbrack; マテリアルが割り当てられていないUSD メッシュは、インポート時にクラッシュできます
* &amp;lbrack；塗りつぶされたパス&amp;rbrack; 対称の影響を受けません
* &amp;lbrack;ステンシル&amp;rbrack;プレビューの解像度がペイント結果よりも低い(&amp;lbrack;)
* &amp;lbrack;UI&amp;rbrack; 「uv island」は、ID マップカラーソースのツールチップに引き続き記載されています。
* &amp;lbrack;Display&amp;rbrack;シャドウが反転して表示される
* ベイク処理モードに切り替えた後も、ワープ投影変形が残る(&amp;lbrack;ビューポート&amp;rbrack;)
* Z軸でスケールを0に設定し、「ジオメトリにワープ」を有効にすると、&amp;lbrack；ワープ&amp;rbrack;グリッドが消える
* &amp;lbrack;Python&amp;rbrack;スコープ変更を含むチャンネルを追加すると、予期しないエラーが発生する

### 12.0.1

リリース日： **2026/03/18**

概要： **マイナーリリース**

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack；フリーズ&amp;rbrack；特定のプロジェクトからエクスポート

### 12.0.0

リリース日： **2026/03/09**&#x200B;概要： **これはメジャーリリースです。 このリリースには、レイヤーの統合、ジオメトリへのワープ、新しいポストエフェクト、新しいプロジェクトウィンドウの機能強化、およびその他の機能強化が含まれています。**

**追加済み**:

* &amp;lbrack；レイヤーを統合&amp;rbrack; レイヤースタック内のレイヤーを統合
* &amp;lbrack；レイヤーを統合&amp;rbrack；統合されたレイヤーをディスクに書き出し
* &amp;lbrack；ジオメトリへのワープ&amp;rbrack;ワープ投影に新しい自動ワープ機能を追加
* &amp;lbrack;Post-effects&amp;rbrack; ポストエフェクトを新しい要素の追加で置き換え
* &amp;lbrack;Post-effects&amp;rbrack;トーンマッパーを更新
* &amp;lbrack;Post-effects&amp;rbrack;ポストエフェクトアセットの新しい使用方法を追加
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Post-effects&amp;rbrack;デフォルトのポストエフェクトアセットをライブラリに統合
* &amp;lbrack；新規プロジェクト&amp;rbrack;プロジェクト作成用UIを改善
* &amp;lbrack；新規プロジェクト&amp;rbrack; メッシュ機能の再読み込みに関する変更点
* &amp;lbrack；新規プロジェクト&amp;rbrack; \*.geo.usdファイルを開くことを許可
* &amp;lbrack；プロジェクト設定&amp;rbrack;プロジェクト設定のUIを改善
* USDライブラリをバージョン25.05にアップデートする
* Substance engineをバージョン9.3.4にアップデートする
* AMD GPUの最小ドライバーを25.3.1/25.Q2に上げます。
* Qtを6.8.6にアップデートする
* &amp;lbrack;Scripting&amp;rbrack; JavaScript APIをバージョン1.1.20に更新
* Pythonを3.13にアップデートする

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack;マスクのマテリアルチャンネル出力を変更すると、クラッシュが発生する場合がある(&amp;lbrack;)
* &amp;lbrack;Import&amp;rbrack; EXRファイルの読み込み時に、USD テクスチャがリニアではなくsRGBに強制される
* &amp;lbrack;UV タイル&amp;rbrack; 1つのイメージを含むイメージシーケンスは、他のUV タイルも塗りつぶします
* &amp;lbrack;ベイク&amp;rbrack; AOがCPUとGPUのベイクで異なる
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack; ビューポートのBaseColorがカラーピッカーと一致しません
* &amp;lbrack;USD&amp;rbrack；均一の値が読み込まれない場合がある(&amp;lbrack;Uniform Values)を参照してください。

## バージョン11

### 11.1.3

リリース日： **2026/02/12**&#x200B;概要： **マイナーリリース**

**固定**:

* &amp;lbrack;ペイント&amp;rbrack;ステンシルと対称が機能しない場合がある(&amp;lbrack;)
* &amp;lbrack；パス&amp;rbrack；指先ストロークの不透明度スライダーを変更しても更新されない
* &amp;lbrack；プロジェクト&amp;rbrack；一部のジオメトリにペイントできません
* &amp;lbrack;Ribbon&amp;rbrack; テクスチャセットの解像度を変更するとインスタンス化パスが消える(&amp;rbrack;)
* &amp;lbrack;UI&amp;rbrack;カラーピッカーが縮小したり消えたりする場合がある

### 11.1.2

リリース日： **2026/01/13**&#x200B;概要： **マイナーリリース**

**追加済み**:

* &amp;lbrack;ベイク処理&amp;rbrack；非同期保存によるUV タイルプロジェクトのベイク処理時間の短縮
* &amp;lbrack;Shaders&amp;rbrack; Mention in シェーダー API変更ログがVulkanのマイグレーション後に変更される
* OpenEXRをバージョン3.4.4に更新する

**固定**:

* Nvidia GTX 10xxシリーズでの起動中に発生する&amp;lbrack;クラッシュ&amp;rbrack;クラッシュ
* &amp;lbrack;クラッシュ&amp;rbrack；別のテクスチャセットでカラーピッカーを使用すると、アプリケーション終了時にクラッシュが発生することがある
* &amp;lbrack；多くのレイヤーを含むプロジェクトでペイントを行う際のパフォーマンスの問題(&amp;rbrack;)
* &amp;lbrack；グラフィックタブレットペンでペイントする際のパフォーマンスの低下(&amp;R)
* &amp;lbrack;UI&amp;rbrack; カメラ設定は、レンダリングモード(Iray)では無効のままです。
* &amp;lbrack;Ribbon&amp;rbrack; Pathがコーナーの後で予期せずオーバーラップすることがあります。
* &amp;lbrack;Ribbon&amp;rbrack; UV タイルのパフォーマンスの問題
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack；折りたたみ時にイメージ入力が消える
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ネストされたグループは、非表示の場合に表示されていても残すことができます。
* &amp;lbrack;ベイク&amp;rbrack;&amp;lbrack;UI&amp;rbrack; 曲率のサンプリング半径を0.01より大きく設定できません
* &amp;lbrack;ベイク処理&amp;rbrack;&amp;lbrack;UI&amp;rbrack；最大オクルーダー距離を1より大きく設定できません
* &amp;lbrack;ベイク処理&amp;rbrack; AO設定「セルフオクルージョン」が複数のテクスチャセットで無視され、低が高ベイク処理として設定される
* &amp;lbrack;ベイク処理&amp;rbrack; ID マップが、低モードと高モードでFBXから頂点カラーをベイクしない
* &amp;lbrack;Content&amp;rbrack; Highpass filterを使用すると、カラーマネージドチャンネルの色が色あせて表示される

### 11.1.1

リリース日： **2025/12/09**&#x200B;概要： **マイナーリリース**

**追加済み**:

* &amp;lbrack;Performance&amp;rbrack；部分的なテクスチャを計算する際のUV タイルのパフォーマンスを向上させる
* &amp;lbrack;ベイカー&amp;rbrack;バージョン3.15.4にアップデート

**固定**:

* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack；以前のバージョンからプロジェクトを保存すると、常にクラッシュになる
* &amp;lbrack;クラッシュ&amp;rbrack;プロジェクトを閉じるとクラッシュが発生する場合がある
* &amp;lbrack;Project&amp;rbrack；以前のバージョンで作成されたプロジェクトを開くと、「メンバー数の不一致」エラーが発生する
* &amp;lbrack;ベイク処理&amp;rbrack; UV タイルが存在する場合、以前の烘焙結果と結合されない。
* Nvidia GTX 10XXシリーズでレイトレーシングが無効になっていても、ベイク処理中&amp;rbrack;デバイスが失われる(&amp;lbrack;)
* &amp;lbrack;ベイク処理&amp;rbrack；通常のAOは、パディングがないためにエッジに不具合があります
* &amp;lbrack;ベイク処理&amp;rbrack; AO設定「セルフオクルージョン」が複数のテクスチャセットで無視され、「名前で一致」がオンになる
* &amp;lbrack;high-poly メッシュで頂点カラーが不足している場合、ベイク処理&amp;rbrack;ID マップは完全に黒になります。
* &amp;lbrack;Ribbon&amp;rbrack; アルファブレンディングモードのツールチップに、覆い焼きリニアではなく画面描画モードが表示される
* &amp;lbrack;Path&amp;rbrack;パスの終端にポイントを近づけると、正接が予期しないループを起こす(&amp;lbrack;Path&amp;rbrack; Path_rbrack; Path_path)
* &amp;lbrack;Tool&amp;rbrack; マテリアルのプレビューが、マスクで投影が使用されていると機能しない
* &amp;lbrack;エンジン&amp;rbrack；小さなストロークをペイントすると、濃淡な斑点が表示されることがある
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーインスタンスの作成を元に戻しても正しく削除されない
* &amp;lbrack；書き出し&amp;rbrack; GLTF書き出しのAlphaモードは常にMASKに設定される
* &amp;lbrack;Python&amp;rbrack;スコープ指定された変更ブロック外でレイヤースタックを編集すると予期しないエラーが発生する

**既知の問題**:

* &amp;lbrack;Ribbon&amp;rbrack; UV タイルのパフォーマンスの問題
* &amp;lbrack;Ribbon&amp;rbrack; Pathがコーナーの後で予期せずオーバーラップすることがあります。
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Ribbon&amp;rbrack; Ribbon can クラッシュで非常に長いテキストを作成する
* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。

### 11.1.0

リリース日： **2025/11/18**&#x200B;概要： **このアップデートはメジャーリリースで、専用の新しいコンテンツ、塗りつぶしレイヤーの対称サポート、ディスプレイスメントのための物理サイズパラメーター、更新されたベイカーによるパフォーマンスの向上、WindowsおよびLinux用のVulkanの完全サポートなどの機能強化が含まれています。**

**追加済み**:

* 新しいリボンツール
* &amp;lbrack；ツール&amp;rbrack；新しいリボンツールを追加してシームレスなパスを作成
* &amp;lbrack;Ribbon&amp;rbrack; [プロパティ]ウィンドウでリボンプリセットショートカットを追加
* &amp;lbrack;Ribbon&amp;rbrack;パス上の頂点ごとにリボンの不透明度を変更できるようにします
* &amp;lbrack;Ribbon&amp;rbrack;パス上の頂点ごとにリボンのサイズを変更できるようにします
* &amp;lbrack;Ribbon&amp;rbrack;パスが閉じられたときに、Substanceで定義された開始/終了を削除する
* &amp;lbrack;Ribbon&amp;rbrack; ペイント/消しゴム/指先ツールのプロパティウィンドウでマテリアル/パスのプレビューを削除
* &amp;lbrack;Ribbon&amp;rbrack；セルフオーバーラップ時にアルファと一部のチャンネルに描画モードを追加
* 塗りつぶし対称
* &amp;lbrack;Fill&amp;rbrack; 塗りつぶしレイヤーやエフェクトの対称のサポートを追加
* &amp;lbrack;Fill&amp;rbrack;&amp;lbrack;UI&amp;rbrack; 塗りつぶしレイヤーとエフェクトのプロパティウィンドウで対称設定を表示
* &amp;lbrack;Fill&amp;rbrack; ビューポートメニューとプロパティウィンドウの両方で対称設定UIを再調整
* &amp;lbrack;Fill&amp;rbrack;ワープモードで投影したときに、法線テクスチャの向きが正しく変更される(&amp;R)
* ディスプレイスメント
* &amp;lbrack;ディスプレイスメント&amp;rbrack; 物理サイズをディスプレイスメントユニットとして使用
* パフォーマンスの向上
* &amp;lbrack；パフォーマンス&amp;rbrack；大きな三角形に小さなブラシストロークのレンダリングを改善
* &amp;lbrack;Performance&amp;rbrack; シェーダーのコンパイル時間を短縮する
* &amp;lbrack;Performance&amp;rbrack; WindowsおよびLinux用のVulkanの完全サポート
* &amp;lbrack；パフォーマンス&amp;rbrack；より高速なGPUレンダリングとAMD レイトレーシングのサポートによりベイカーを更新
* &amp;lbrack;UI&amp;rbrack;ツールのプロパティをグループに再編成し、デフォルトでいくつか折りたたむ
* &amp;lbrack;エンジン&amp;rbrack; Substance engineをバージョン9.2.5にアップデート
* &amp;lbrack;Substance&amp;rbrack;ツールと塗りつぶしでSubstanceリソースの解像度の上書きを表示
* &amp;lbrack；書き出し&amp;rbrack;グレースケールテクスチャを書き出すためのメッシュマップ書き出しプリセットの更新
* Python
* &amp;lbrack;ベイク処理&amp;rbrack;&amp;lbrack;Python&amp;rbrack; ベイカーの更新後に変更ログが中断したことを示す
* &amp;lbrack;Python&amp;rbrack; Pythonで塗りつぶし対称設定を表示
* コンテンツと新規コンテンツ
* &amp;lbrack;Content&amp;rbrack; Add 75 new tools for the Ribbon tool
* &amp;lbrack;Content&amp;rbrack;グラデーションビルダーリソースを更新してリボンと互換性を持たせる

**固定**:

* &amp;lbrack;クラッシュ&amp;rbrack;パスのロードが有効な状態で別のプロジェクトをスナップすると、クラッシュできる
* &amp;lbrack;クラッシュ&amp;rbrack;クリップボード内の別のセッションの情報がクラッシュする場合、パスパネル内で右クリック
* &amp;lbrack;UI&amp;rbrack;インタフェースがパス作成時にツールプロパティでスクロールアップする
* &amp;lbrack;UI&amp;rbrack;パスビューポートの表示が非表示のときにマウスカーソルが消える
* &amp;lbrack；パス&amp;rbrack;パスパネルで異なるツールプロパティをコピー&amp;ペーストすると、プロパティが不安定になる
* &amp;lbrack;Tool&amp;rbrack;消しゴムツールと指先ツールプリセットで、チャンネル選択が必ずしも更新されない
* &amp;lbrack;Tool&amp;rbrack;ペイントされた値はグレーですが、マスクに色付きツールプリセットを読み込むとUIが白く表示される
* &amp;lbrack;Tool&amp;rbrack;プリセットをマスクから作成すると、別のプリセットから読み込まれたチャンネル値が保持される
* &amp;lbrack;Substance&amp;rbrack; グラフで定義された標準カラースペースの上書きが考慮されない
* &amp;lbrack;Content&amp;rbrack;デフォルトのブラシシェイプリソースが古いSubstanceを使用

**既知の問題**:

* シェーダーインスタンス履歴が正しく追跡されない
* &amp;lbrack;Ribbon&amp;rbrack; UV タイルのパフォーマンスの問題
* &amp;lbrack;Ribbon&amp;rbrack; Pathがコーナーの後で予期せずオーバーラップすることがあります。
* &amp;lbrack;Ribbon&amp;rbrack;パスの終端にポイントを近づけると、正接が不要なループを作成する(&amp;lbrack; Ribbon&amp;rbrack;)
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Ribbon&amp;rbrack; Ribbon can クラッシュで非常に長いテキストを作成する
* &amp;lbrack;Tool&amp;rbrack; マテリアルのプレビューが、マスクで投影が使用されていると機能しない
* &amp;lbrack;ベイク処理&amp;rbrack; AO設定「セルフオクルージョン」が無視され、複数のテクスチャセットがあり、「名前で一致」が有効になっている
* &amp;lbrack;ベイク処理&amp;rbrack；通常のAOは、埋め込みが不足しているため、エッジに斑点があります
* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。

### 11.0.3

リリース日： **2025/08/05**&#x200B;概要： **マイナーリリース**

**追加済み**:

* &amp;lbrack;Substance 3D Assets&amp;rbrack; 3Dアセットパネルに通知ドットを追加
* &amp;lbrack;VFX Platform 2025&amp;rbrack;カラーマネジメント設定にACE 2.0構成を追加
* &amp;lbrack;VFX Platform 2025&amp;rbrack; OCIOをバージョン2.4.2にアップデート
* Irayをバージョン2024.10に更新します。
* &amp;lbrack;エンジン&amp;rbrack; Substance engine v.9.2.3にアップデート
* &amp;lbrack;Nvidia&amp;rbrack; Nvidiaの最小ドライバーバージョンを572.60(Win)および570.169(Linux)に上げる

**固定**:

* &amp;lbrack;Python&amp;rbrack;スコープ変更がヒストリーウィンドウに表示されない

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。

### 11.0.2

リリース日： **2025/06/10**&#x200B;概要： **マイナーリリース**

**追加済み**:

* &amp;lbrack;Mac&amp;rbrack；特定のオペレーティングシステムのバージョンに関する警告を追加し、アーティファクトが発生する
* &amp;lbrack；自動アップデート&amp;rbrack; AssetsエラーログのUXのマイナーな改善
* &amp;lbrack;自動ラップ解除&amp;rbrack;シーム機能の強化によるバージョン1.3.2へのアップデート
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;FBX&amp;rbrack;データが疎な複数のUV セットのサポートを追加
* FBXとして書き出された&amp;lbrack;Export&amp;rbrack; メッシュは、読み込み時に存在していた場合、その他のUV セットが欠落しています

**固定**:

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;ネットワークドライブに保存時のクラッシュ
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack；タブレット&amp;rbrack；パン時のちらつき
* &amp;lbrack;SpaceMouse&amp;rbrack;パスツールの操作中に発生する問題
* &amp;lbrack；自動ケージ&amp;rbrack; メッシュの再読み込み後にベイクできない
* &amp;lbrack；自動アップデート&amp;rbrack；最初のタイルが見つからない場合、画像シーケンスがリロードされない
* &amp;lbrack;Path&amp;rbrack;カスタム正接は他の正接に影響する可能性があります
* 最初のポイントが別のテクスチャセットにある場合、&amp;lbrack;Path&amp;rbrack; Pathがテクスチャセットに表示されません。
* &amp;lbrack;UI&amp;rbrack;プロジェクトを開いた後、一部のメニューが常に無効になる（対称など）
* &amp;lbrack;Properties&amp;rbrack; Cannot use/load ツールプリセット with Filled path tool
* &amp;lbrack;USD&amp;rbrack; USDファイルを使用するときに、カスタムシェーダーで複数のUV セットが認識されない
* &amp;lbrack;USD&amp;rbrack；同じ名前のカメラはオーバーライドされます。
* &amp;lbrack；書き出し&amp;rbrack; Photoshopに送信すると、カラーとグレースケールの両方の結果でカラースペースが正しく表示されない
* &amp;lbrack;Export&amp;rbrack;アルファ付きのグレースケールチャンネルが、PNG形式のグレースケールではなく、カラーとして書き出される
* &amp;lbrack;Export&amp;rbrack;グレースケールチャンネルをPSDとして書き出すと、ファイルが無効になるか、切り捨てられる
* &amp;lbrack；コンテンツ&amp;rbrack；多方向モードのワープフィルターが機能しない
* &amp;lbrack;Python&amp;rbrack; レイヤースタックノードのクロール時にリストエラーを割り当てることができません

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。

### 11.0.1

リリース日： **2025/04/10**&#x200B;概要： **マイナーリリース**

注意： **Linux CCDバージョンは4月29日まで延期されます**

**追加：**

* Qt 6.5.8にアップデートします。
* &amp;lbrack;Substance&amp;rbrack；複数のイメージ入力が同じ使用法を使用している場合に、フィルタのログメッセージを追加する
* &amp;lbrack;Nvidia&amp;rbrack；最新のNvidiaドライバー(572.47)に関する警告の追加

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack; シングルチャンネルスロットで使用を使用してsbsarをドラッグ&amp;ドロップする場合
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack；パス&amp;rbrack; [パスの種類を変更]オプションが、特定のパスをクリックしていないときにグレー表示されない
* &amp;lbrack;Fill Path&amp;rbrack；はSubstance マテリアルを選択できません
* &amp;lbrack;エンジン&amp;rbrack;ブラシストロークに沿った斑点
* &amp;lbrack;エンジン&amp;rbrack;パスが特定の設定で壊れる
* スポイトのカラースペースのドロップダウンに関する問題
* &amp;lbrack;Auto-update&amp;rbrack; &amp;lbrack;Python&amp;rbrack;バージョンなしでResourceIDを使用すると間違ったエラーメッセージが表示される
* &amp;lbrack；一部のプロジェクトを開くときのシェーダー&amp;rbrack;クラッシュ

**既知の問題：**

* &amp;lbrack;SpaceMouse&amp;rbrack;パスツールの操作中に発生する問題
* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。

### 11.0.0

リリース日： **2025/03/11**&#x200B;概要： **メジャーリリース、新しい自動アップデート機能、塗りつぶしパスツールなどのパスの機能強化、および新しいフィルターとベイク用の試験的な自動ケージ生成**

**追加済み**:

* 自動更新
* &amp;lbrack;Auto-update&amp;rbrack;アセットパネル内の変更されたアセットを自動更新
* &amp;lbrack;Auto-update&amp;rbrack;プロジェクト全体で変更されたアセットを自動更新
* &amp;lbrack；自動更新&amp;rbrack；自動更新をデフォルトでオフに保つ
* &amp;lbrack;Auto-update&amp;rbrack;リソースパラメータが一致しない場合に更新をオプションにする(.sbsar、.glsl、.ai、.svg)
* &amp;lbrack；自動更新&amp;rbrack；自動更新機能を無効にする環境変数を追加
* &amp;lbrack;Auto-update&amp;rbrack;&amp;lbrack;SBSAR&amp;rbrack;リソースパラメータが一致しない場合は更新をオプションにする
* 塗りつぶされたパス
* &amp;lbrack；パス&amp;rbrack;&amp;lbrack；塗りつぶし&amp;rbrack；塗りつぶされたパスを作成する新しいツールを追加
* パスの改善
* &amp;lbrack;Path&amp;rbrack;ポリゴンにスナップするパスを作成
* &amp;lbrack;Path&amp;rbrack;パスの種類を切り替えることができます
* &amp;lbrack;Path&amp;rbrack;コンテンツとマスクの間でペーストのパス頂点データをコピーできるようにします
* &amp;lbrack;Path&amp;rbrack；新しいポイントを作成するときに角度を制限できるようにします
* &amp;lbrack；パス&amp;rbrack；点の作成を線分に拘束できるようにします
* &amp;lbrack；パス&amp;rbrack;ワンクリックでシェイプを閉じる
* &amp;lbrack;Path&amp;rbrack;パス情報を表示
* &amp;lbrack;Path&amp;rbrack;パス頂点の拡大/縮小と回転を許可
* &amp;lbrack；パス&amp;rbrack;&amp;lbrack;UX&amp;rbrack；変換ギズモを簡単にアクセスできるようにする
* &amp;lbrack；パス&amp;rbrack;パスのプレビューを追加
* &amp;lbrack；パス&amp;rbrack; Shift + Pでパスのプレビューを無効にする
* &amp;lbrack;Path&amp;rbrack；側面から正接版を改善する
* &amp;lbrack；パス&amp;rbrack; 3Dパスにフォーカスを許可
* &amp;lbrack;Path&amp;rbrack; 頂点は、UIのオンとオフを切り替えるときにセレクションステータスを保持する(&amp;lbrack;)
* &amp;lbrack;Path&amp;rbrack; Backspaceを使用してパスを削除できるようにします
* &amp;lbrack;Path&amp;rbrack;ユーザが展開してもパスリストを開いたままにする(&amp;R)
* &amp;lbrack;Path&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack;コピー/ペースト時に重複した名前を正しく変更
* &amp;lbrack;Path&amp;rbrack; UIとツールチップの改善
* Performance
* &amp;lbrack；パフォーマンス&amp;rbrack；高テセレーションレベル使用時のビューポートのパフォーマンスを向上
* &amp;lbrack;Performance&amp;rbrack；新しい塗りつぶしレイヤー/エフェクトで最初のチャンネルのみを有効にする
* &amp;lbrack；パフォーマンス&amp;rbrack;ブラシストローク計算を並列化
* ベイク処理
* &amp;lbrack;ベイク処理&amp;rbrack；高ポリゴンメッシュを使用したベイク処理用に、新しい全自動ケージ生成オプションを追加（試験的）
* コンテンツ
* &amp;lbrack;Content&amp;rbrack; 6つの新しいフィルターを追加：スタイル化、量子化、異方性桑原、ベベルスムーズ、方向の距離、グレースケール変換
* &amp;lbrack;Content&amp;rbrack; ノイズとグランジをDesignerから最新バージョンに更新（新しい2D Voronoiを使用）
* &amp;lbrack;Content&amp;rbrack; 3つの新しいテクスチャジェネレータ（タイルランダム、Triangle Grid、Scratchesジェネレータ）を追加
* &amp;lbrack;Content&amp;rbrack; Unreal エンジンテンプレートの名前変更とプリセットの書き出し
* Python
* &amp;lbrack;シェルフ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; スマートマテリアルまたはスマートマスクをPythonからディスクに保存
* &amp;lbrack;Python&amp;rbrack; Python APIにベイク処理自動ケージを追加
* &amp;lbrack;Python&amp;rbrack; テクスチャセット/UV タイルの名前と説明の編集を許可
* &amp;lbrack;Python&amp;rbrack;ベクトルおよびフォントソースで解像度設定を共有
* &amp;lbrack；自動更新&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Pythonでのプロジェクトの自動更新機能の表示
* その他
* &amp;lbrack；書き出し&amp;rbrack；新しいパネルでオプションに簡単にアクセスできるようにする
* &amp;lbrack;Nvidia&amp;rbrack；最新のNvidiaドライバー(572.16)に関する警告の追加
* 角度スナップはオブジェクト/ワールド空間の選択の影響を受ける必要があります
* &amp;lbrack;テクスチャセットリスト&amp;rbrack;UV タイルにカスタム名を付けて書き出し時に使用できるようにする
* Mac
* &amp;lbrack;Mac&amp;rbrack;グラフィックレンダリングにOpenGLの代わりにMetalを使用
* &amp;lbrack;Mac&amp;rbrack; Drop Mac Intelサポート

**固定**:

* &amp;lbrack;クラッシュ&amp;rbrack;イメージ入力を削除
* 「レイヤースタック」ボタンを使用してスマートマットを追加できない
* &amp;lbrack;Python&amp;rbrack; Effects on GroupLayerNodeが見つかりません

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack；一部のプリセットを読み込む際のMacOS Intel&amp;rbrack; クラッシュ
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。
* &amp;lbrack;RedHat&amp;rbrack;カラーピッカーの問題

## バージョン10

### 10.1.2

リリース日： **2024/12/3**&#x200B;概要： **マイナーリリース、バグ修正**

**固定**:

* &amp;lbrack;クラッシュ&amp;rbrack;イメージ入力を削除
* 「レイヤースタック」ボタンを使用してスマートマットを追加できない
* &amp;lbrack;Python&amp;rbrack; Effects on GroupLayerNodeが見つかりません

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack；一部のプリセットを読み込む際のMacOS Intel&amp;rbrack; クラッシュ
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。
* &amp;lbrack;RedHat&amp;rbrack;カラーピッカーの問題

### 10.1.1

リリース日： **2024/11/5**&#x200B;概要： **マイナーリリース、バグ修正**

**追加済み**:

* &amp;lbrack;Project&amp;rbrack；新しいプロジェクト選択が検証されるまで、現在のプロジェクトを開いたままにする
* &amp;lbrack;自動ラップ解除&amp;rbrack; Texel densityを使用すると、UV アイランドをUDIMに分割しやすくなります。
* &amp;lbrack;ベイク処理&amp;rbrack;メッシュマップのコンテキストメニューにあるあいまいなコピーを修正
* &amp;lbrack；ワープ&amp;rbrack; Z(深度)軸のビューポートにスケーリングを削除
* &amp;lbrack;Import/Export&amp;rbrack；未使用の画像ファイル形式のサポートを削除
* Substance engineを9.1.4にアップデートします。

**固定**:

* &amp;lbrack;Assetsにクラッシュを再配置してプロジェクトを保存した後&amp;rbrack;
* &amp;lbrack;クラッシュ&amp;rbrack; aiserver libraryの問題(&amp;rbrack;)
* &amp;lbrack;クラッシュ&amp;rbrack；まれにIllustratorサーバーのクラッシュ
* &amp;lbrack;クラッシュ&amp;rbrack；まれに終了する場合がある
* 一部のコンピューターでクラッシュレポートを送信できません
* &amp;lbrack;ベイク処理&amp;rbrack; 頂点カラーが正しく読み取られません
* &amp;lbrack;UI&amp;rbrack;ウィンドウの場所と起動時の新機能がシフトされる
* &amp;lbrack;Assimp&amp;rbrack; MayaのStandardSurfaceがID ベイク処理で認識されません
* &amp;lbrack;Python&amp;rbrack; SSL libが見つからないためエラーが出力される
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Win&amp;rbrack; QColorConstants.Transparentの呼び出し時のエラー
* &amp;lbrack;Python&amp;rbrack; Pythonで作成されたレイヤのサムネイルは、レイヤースタック内をクリックするまで更新されません
* &amp;lbrack;シェーダー&amp;rbrack; シェーダー API変更ログ内のリンク切れ
* &amp;lbrack;3Dアセット&amp;rbrack; 3DアセットにアクセスするときにOSプロキシ設定を使用

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack；一部のプリセットを読み込む際のMacOS Intel&amp;rbrack; クラッシュ
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack;スクリプトで削除されたように見えるウィジェットは動作しています
* &amp;lbrack;RedHat&amp;rbrack;カラーピッカーの問題

### 10.1.0

リリース日： **2024/09/17**&#x200B;概要： **メジャーリリース、新規コンテンツ：塗りつぶし領域マスク/カラーフィルター、刺繍デカールフィルターと6つの汎用Substanceフィルター、マテリアルとシェーダープロパティを持つUSDの読み込み、パフォーマンス向上、VFX platform 2024準拠、Linux RedHatへの移行**

**追加済み**:

* &amp;lbrack;Content&amp;rbrack；新しい塗りつぶし領域マスク/カラーフィルターの追加
* &amp;lbrack；コンテンツ&amp;rbrack；新しい刺繍デカールフィルターを追加
* &amp;lbrack;Content&amp;rbrack; 6つの新しい汎用Substanceフィルター（FXAA、ピクセレート、ハイパス、ポスタリゼーション、スムースステップ、しきい値）を追加
* &amp;lbrack;USD&amp;rbrack；定義済みのASM マテリアルを使用してUSDレイヤーを書き出し
* &amp;lbrack;USD&amp;rbrack; マテリアルとシェーダーのプロパティを使用してUSDを読み込み
* &amp;lbrack;Performance&amp;rbrack;デフォルトで最適化されたレイヤースタックサムネールを有効にする
* &amp;lbrack；パフォーマンス&amp;rbrack;プロジェクトファイルのオープン時間とメモリ消費を削減（データデコード）
* VFX platform 2024準拠
* &amp;lbrack;VFX Platform 2024&amp;rbrack; Python 3.11にアップデート
* &amp;lbrack;VFX Platform 2024&amp;rbrack; OpenEXR 3.2にアップデート
* &amp;lbrack;VFX Platform 2024&amp;rbrack; &amp;lbrack;USD&amp;rbrack; OpenSubdiv 3.6.0を更新
* &amp;lbrack;VFX Platform 2024&amp;rbrack;&amp;lbrack；カラーマネジメント&amp;rbrack; OCIO 2.3.2にアップデート
* &amp;lbrack;Linux&amp;rbrack; Linux RedHatへの移行
* &amp;lbrack;Linux&amp;rbrack; Nvidiaドライバーの最小バージョンを535.171.04にアップデートする
* &amp;lbrack;Import&amp;rbrack; GLTF メッシュを読み込むときに、法線マップを反転するオプションを追加します
* &amp;lbrack;UI&amp;rbrack;ドラッグイベント検出距離にオペレーティングシステムの既定値を使用
* &amp;lbrack;Substance engine&amp;rbrack；実行ファイルからシンボルを削除するコールストリップ関数を追加
* &amp;lbrack；スプラッシュ画面&amp;rbrack；新しいスプラッシュ画面形式に更新
* Substance engineをバージョン9.1.3にアップデートする
* &amp;lbrack;Python&amp;rbrack; レイヤースタックドキュメントメニューにサンプルへのリンクを表示
* &amp;lbrack;JavaScript&amp;rbrack; Javascriptプラグインをjavascript/pluginsサブフォルダーに移動

**固定**:

* &amp;lbrack;Illustrator&amp;rbrack；特定のケースで.aiグラフィックが含まれているUV タイルの書き出しでクラッシュが発生する(&amp;lbrack;)
* &amp;lbrack;動的ストローク&amp;rbrack;&amp;lbrack；パス&amp;rbrack;ストロークごとにランダムがパスで機能しない
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack；プロパティ&amp;rbrack;タイリングが均一でない場合にロックが有効になる
* Painterプロジェクトをダブルクリックすると、Debug TXTファイルが作成される
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack；一部のテクスチャが見つからない可能性があります
* &amp;lbrack;ASM&amp;rbrack;拡散カラーチャンネルがメタリックを無視する
* &amp;lbrack;Content&amp;rbrack；ぼかしフィルターが「作業中」のカラースペースで機能しない
* &amp;lbrack;Content&amp;rbrack; Height調整フィルターもレイヤーのアルファを変更

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;ACE&amp;rbrack;ディスプレイ変形にsRGB ICEカラースペースを使用しない
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack；一部のプリセットを読み込む際のMacOS Intel&amp;rbrack; クラッシュ
* &amp;lbrack；リソース&amp;rbrack; クラッシュを再配置してプロジェクトを保存
* &amp;lbrack;エンジン&amp;rbrack；通常チャンネルでクローンツールを使用してペイントするとカラーが正しくシフトされない
* &amp;lbrack;Python&amp;rbrack; ゴーストウィジェットは、スクリプトがまだ機能しているため削除されています。
* &amp;lbrack;RedHat&amp;rbrack;カラーピッカーの問題

### 10.0.1

リリース日： **2024/06/11**&#x200B;概要： **マイナーリリース、バグ修正**

**追加：**

* &amp;lbrack;Library&amp;rbrack; Substanceフォントを通常のフォントファイルに変換
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack;SVG&amp;rbrack;スコープ選択のサムネールを明るいグレーの背景にする
* &amp;lbrack;Python&amp;rbrack；使用可能なカラースペースを一覧表示するビットマップソースに関数を追加

**固定**:

* &amp;lbrack;レイヤースタック&amp;rbrack;フォルダを他のフォルダに移動すると常に閉じる(&amp;rbrack;)
* &amp;lbrack;Save&amp;rbrack; 「コピーとして保存」または自動保存が失敗すると、プロジェクトファイルが失われる（特定のケースで）
* &amp;lbrack;Import&amp;rbrack；同じ名前で別の拡張子のアセットはオーバーライドされます
* &amp;lbrack；画像入力でアンカーポイントを使用するときに、プロパティ&amp;rbrack；設定が見つからない
* &amp;lbrack;Illustrator&amp;rbrack;サーバーのクラッシュ後、Painterを再起動しないとIllustratorファイルをインポートできない
* &amp;lbrack;Python&amp;rbrack;インスタンスの親をタイプ「properties」で設定することはできません
* &amp;lbrack;Python&amp;rbrack；高ポリゴンをベイクパラメータとして設定しても、高ポリゴンはロードされません
* &amp;lbrack;Python&amp;rbrack; set_color_space()のエラーメッセージが一般的すぎます
* &amp;lbrack;Python&amp;rbrack；参照ソースでサイクルを作成できます

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎます
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack；一部のプリセットを読み込む際のMacOS Intel&amp;rbrack; クラッシュ
* &amp;lbrack;Illustrator&amp;rbrack；特定のケースで.aiグラフィックが含まれているUV タイルの書き出しでクラッシュが発生する(&amp;lbrack;)
* &amp;lbrack;動的ストローク&amp;rbrack;&amp;lbrack；パス&amp;rbrack;ストロークごとにランダムがパスで機能しない

### 10.0.0

リリース日： **2024/05/16**&#x200B;概要： **メジャーリリース、Python APIを使用したレイヤースタックのエディション、ネイティブIllustratorファイルの読み取り、3Dアセットと新しいテキストリソースの統合**

**追加済み**:

* &amp;lbrack;Illustrator&amp;rbrack; PainterのアートボードでIllustratorファイルを使用
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack；スコープ&amp;rbrack; SVGの選択範囲にプレビューを追加
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Painterで直接3Dアセットを参照、選択、ダウンロード
* &amp;lbrack;Substance 3D Assets&amp;rbrack;&amp;lbrack;UI&amp;rbrack；新規パネル
* &amp;lbrack;Substance 3D Assets&amp;rbrack;サポート環境マップとマテリアル
* &amp;lbrack;Substance 3D Assets&amp;rbrack；再読み込みおよび操作が可能で、場所フォルダーを新しいSubstance 3D Assetsパネルで開く
* &amp;lbrack;Substance 3D Assets&amp;rbrack;ダウンロードマネージャの追加
* &amp;lbrack；テキストリソース&amp;rbrack；埋め込みフォントの使用を許可
* &amp;lbrack；テキストリソース&amp;rbrack; メッシュ上のフォント/テキストをレンダリングできるようにします
* &amp;lbrack；テキストリソース&amp;rbrack；新しいカテゴリでアセットパネルのユーザーおよびその他の共有パスのフォントを表示
* &amp;lbrack；テキストリソース&amp;rbrack;&amp;lbrack；プロパティ&amp;rbrack；高度なフォントプロパティのサポートを追加
* &amp;lbrack；テキストリソース&amp;rbrack;ミニシェルフ内のフォントを検索および表示できるようにします
* &amp;lbrack；テキストリソース&amp;rbrack；互換性のないフォントを読み込む際のエラーメッセージの追加/ダイアログ
* その他
* &amp;lbrack；塗りつぶし投影&amp;rbrack；小さい値を使用する場合のマニピュレーターの拡大縮小を改善
* &amp;lbrack;マニピュレーター&amp;rbrack; Ctrl ショートカットを押したときに新しい十字モードを追加
* &amp;lbrack;マニピュレーター&amp;rbrack;移動時のサーフェスマニピュレーターの安定性を向上
* &amp;lbrack;Export&amp;rbrack; SBSAR出力にカラースペース名を追加
* &amp;lbrack；パフォーマンス&amp;rbrack;ディスク上のアセットのライブラリ検出時間を改善
* &amp;lbrack;Substance&amp;rbrack; Substanceエンジンバージョン9.1.2にアップデート
* &amp;lbrack；ドラッグ&amp;ドロップ&amp;rbrack; ビューポートにドロップするときにデカールの回転をカメラに揃える
* &amp;lbrack;Python&amp;rbrack; レイヤースタック版
* &amp;lbrack;Python&amp;rbrack; UIでレイヤー、エフェクト、マスク、ジオマスクを選択できるようにする
* &amp;lbrack;Python&amp;rbrack;レイヤの描画モードの取得/設定を可能にする
* &amp;lbrack;Python&amp;rbrack; 塗りつぶしレイヤーの投影設定の取得/設定を許可する
* &amp;lbrack;Python&amp;rbrack; 塗りつぶしレイヤーからSubstanceマテリアルの色を照会できるようにします
* &amp;lbrack;Python&amp;rbrack;レイヤとエフェクト内の均一カラーとリソースのクエリと設定を可能にする
* &amp;lbrack;Python&amp;rbrack; レイヤースタック内のテキストリソースの作成と編集を可能にする
* &amp;lbrack;Python&amp;rbrack;レイヤおよびエフェクト上のアクティブなチャンネルを編集できるようにします
* &amp;lbrack;Python&amp;rbrack;バッチ処理を許可して、元に戻す/やり直しを1回実行
* &amp;lbrack;Python&amp;rbrack;ベクトルソースパラメータのロード/編集を許可
* &amp;lbrack;Python&amp;rbrack;カラーマネジメントを使用してレイヤーとエフェクトのカラープロパティを編集できるようにします
* &amp;lbrack;Python&amp;rbrack;インスタンス化されたレイヤのクエリーと作成を許可
* &amp;lbrack;Python&amp;rbrack; カラー選択効果を追加できるようにします
* &amp;lbrack;Python&amp;rbrack;ビットマップイメージのカラーマネジメントの制御を許可
* &amp;lbrack;Python&amp;rbrack; エンジンの一時停止/一時停止を解除できます
* &amp;lbrack;Python&amp;rbrack；兄弟ノードと親ノードに移動できるようにします
* &amp;lbrack;Python&amp;rbrack;フィルタ/ジェネレータ効果の作成を許可
* &amp;lbrack;Python&amp;rbrack;レベル効果を追加できるようにします
* &amp;lbrack;Python&amp;rbrack;レイヤにスマートマスクを追加できるようにします
* &amp;lbrack;Python&amp;rbrack;アンカーポイントの作成/編集を許可
* &amp;lbrack;Python&amp;rbrack;レイヤのマスクの取得/設定を許可する
* &amp;lbrack;Python&amp;rbrack；比較マスクエフェクトの作成を許可
* &amp;lbrack;Python&amp;rbrack; Substanceリソースのプリセットの照会と使用を許可
* &amp;lbrack;Python&amp;rbrack; Substanceリソースのinternal_properties関数を使用して、プリセットとその値を一覧表示できるようにします
* &amp;lbrack;Python&amp;rbrack；定義済みの書き出しプリセットを一覧表示できるようにします
* &amp;lbrack;Python&amp;rbrack;ライブラリで使用可能な書き出しプリセットを一覧表示できるようにします
* &amp;lbrack;Python&amp;rbrack；書き出しプリセットのコンテンツを取得できるようにします

**固定**:

* &amp;lbrack;クラッシュ&amp;rbrack; Ctrl-Zを使用して「シェーダーインスタンスを削除」を元に戻す
* &amp;lbrack;クラッシュ&amp;rbrack；最後の選択範囲がエフェクトであった場合に、空のスタックにレイヤーを作成
* &amp;lbrack;SVG&amp;rbrack;カスタム切り抜き領域値に関する問題
* &amp;lbrack;自動ラップ解除&amp;rbrack; UV方向を変更せずにパッキングのみを再計算すると、クラッシュが発生します。
* &amp;lbrack；ドラッグ&amp;ドロップ&amp;rbrack；外部リソースによる遅延が複数回プリロードされる
* &amp;lbrack;UI&amp;rbrack;リソースサムネイルをドラッグアンドドロップすると、レイヤースタックで警告メッセージが非表示になる
* &amp;lbrack;Performance&amp;rbrack;マスクされたUVタイルは計算されます。
* &amp;lbrack;USD&amp;rbrack;スコープ選択のハイライトが正しくありません
* &amp;lbrack;Resource&amp;rbrack；通常チャンネルでペイントしてプロジェクトを保存すると、ビットマップ画像が破損する
* &amp;lbrack;USD&amp;rbrack；左利きの頂点メッシュ順序のサポート
* &amp;lbrack;Substance&amp;rbrack；角度ウィジェットでは、デフォルトにリセットすると常に0に戻る
* &amp;lbrack;エンジン&amp;rbrack; ステンシル内のSVGによるペイントが機能しない
* &amp;lbrack;エンジン&amp;rbrack；取り消し後に法線マップブラシストロークが壊れる
* &amp;lbrack;Content&amp;rbrack; Graphic to マテリアルフィルターのアルファブレンディングとカラースペースが正しくありません
* &amp;lbrack;Content&amp;rbrack; Tile Generatorの描画モードが機能しない
* &amp;lbrack;Content&amp;rbrack;ヒストグラムスキャンフィルターで縞模様が発生することがある
* &amp;lbrack;Content&amp;rbrack; ベイク照明スタイルはペイントされたHeightを考慮しません
* &amp;lbrack;Python&amp;rbrack; シェーダー変更後にインスタンス化された画層情報を取得すると、予期しないエラーが発生する
* &amp;lbrack；特定の場合に「別名で保存」が失敗すると、プロジェクトファイルが失われる&amp;rbrack;

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Wayland OS上のレイヤースタックにリソースをドラッグ&amp;ドロップ
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎる
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent
* &amp;lbrack;Save&amp;rbrack; Sppプロジェクトファイルは、特定の場合に「コピーとして保存」が失敗すると失われる
* &amp;lbrack；一部のプリセットを読み込む際のMacOS Intel&amp;rbrack; クラッシュ
* &amp;lbrack;Illustrator&amp;rbrack; Painterを再起動しないと、サーバークラッシュ後にAiファイルをインポートできない
* &amp;lbrack;Import&amp;rbrack；同じ名前で別の拡張子のアセットはオーバーライドされます

## バージョン9

### 9.1.2

リリース日： **2024/01/30**&#x200B;概要： **マイナーリリース、バグ修正**

**追加済み**:

* &amp;lbrack;Performance&amp;rbrack；新規プロジェクトでの最初の塗りつぶしレイヤー作成時間を短縮
* &amp;lbrack;Performance&amp;rbrack；重い環境マップの読み込み時間を短縮
* &amp;lbrack;Substance&amp;rbrack;サムネールが生成されている場合でもプロジェクトを保存または閉じることができる

**固定**:

* ビューポートが変更されると、以前のバージョンのプロジェクトで保存が失敗する
* &amp;lbrack;クラッシュ&amp;rbrack;カスタムAOおよびカラーマネジメント使用時のメッシュの再読み込み
* &amp;lbrack；塗りつぶし投影&amp;rbrack；拡大・縮小マニピュレーターをクリックすると、「ペイント可能しない」というメッセージが表示される
* &amp;lbrack；ブラシ&amp;rbrack; アラインメントでペイントすると斑点が生じる
* &amp;lbrack;レイヤースタック&amp;rbrack;スタックが非常に長いと、レイヤー名の変更に時間がかかる。
* &amp;lbrack;レイヤースタック&amp;rbrack;マスクで互換性のないフィルターを使用すると、誤ったエラーメッセージが表示される
* &amp;lbrack;レイヤースタック&amp;rbrack；削除後に選択範囲が一番上のレイヤーに切り替わる
* &amp;lbrack；書き出し&amp;rbrack；生成された法線テクスチャは、常に3D空間の隣接パディングモードになります。
* &amp;lbrack;Export&amp;rbrack; テクスチャアルファが2D ビュー書き出しプリセットで生成されない
* &amp;lbrack;Export&amp;rbrack; SBSAR書き出しで、変換されたマップが正しく使用されない。
* &amp;lbrack;シェーダー&amp;rbrack; シェーダー API変更ログが最新のASM変更で最新ではありません

**既知の問題**:

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Wayland OS上のレイヤースタックにリソースをドラッグ&amp;ドロップ
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがHD画面で小さすぎる
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD export trigger by TextureStateEvent

### 9.1.1

リリース日： **2023/12/05**&#x200B;概要： **マイナーリリース、バグ修正、After Effectsへの送信機能**

**追加：**

* &amp;lbrack;Interop&amp;rbrack;テクスチャメッシュをAfter Effects(Ae 24.1)に送信できるようにします。

**修正済み：**

* &amp;lbrack;Fill&amp;rbrack; 投影へのUV セットが2UV セットを超えて読み取れません
* &amp;lbrack;クラッシュ&amp;rbrack; 16K 環境マップを使用
* &amp;lbrack;クラッシュ&amp;rbrack;イメージ入力として使用されるExr
* &amp;lbrack;クラッシュ&amp;rbrack;プロジェクト間でパスをコピー&amp;ペースト
* &amp;lbrack;QoL&amp;rbrack;デカールモードでAlphaリソースをドラッグ&amp;ドロップすると、マスクにUV 投影が発生する
* &amp;lbrack;Path&amp;rbrack;パス頂点をコピーすると、プロジェクトを再度開くときにターゲットパス名も変更される
* &amp;lbrack;Linux&amp;rbrack;カラー選択が複数の画面で壊れる
* &amp;lbrack；自動ラップ解除&amp;rbrack; texel density controlのUIの問題
* &amp;lbrack;Color Management&amp;rbrack; UIフィードバックは大文字と小文字に区別されますが、エンジンは区別されません。
* &amp;lbrack；カラーマネジメント&amp;rbrack;ユーザーデータの上書きによるマスク内のカラースペース選択が正しくない

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* AMD上のLinux Waylandでレイヤースタックにクラッシュをドラッグ&amp;ドロップする場合、&amp;lbrack；リソース&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Monterey OSで異方性フィルタリング値を変更する
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがhd画面で小さすぎる
* &amp;lbrack;Python&amp;rbrack; TextureStateEventによってトリガーされたUSDの書き出しクラッシュ

### 9.1.0

リリース日： **2023/11/07**&#x200B;概要： **SVGと透明度のサポートと、ドラッグ&amp;ドロップおよびパスツールの機能強化を導入したメジャーリリース**

**追加：**

* &amp;lbrack;SVG&amp;rbrack;ベクトルファイルの読み込みを許可(SVG)
* &amp;lbrack;SVG&amp;rbrack;&amp;lbrack;UI&amp;rbrack; SVG固有のプロパティのサポートを追加
* &amp;lbrack;SVG&amp;rbrack；元の画像の縦横比を簡単に維持するオプションを追加
* &amp;lbrack;SVG&amp;rbrack；透明度のあるSVGのアルファを自動使用できるようにする
* &amp;lbrack;Interop&amp;rbrack;テクスチャメッシュをAfter Effects（Ae 24.1ベータ版）に送信できるようにします。
* &amp;lbrack;Interop&amp;rbrack; Add settings for Send to After Effects
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack；アセット&amp;rbrack;&amp;lbrack;UI&amp;rbrack; UIスロットにドラッグ&amp;ドロップ時にアセットを自動読み込み
* &amp;lbrack;QoL&amp;rbrack；外部アセットをレイヤースタックにドラッグ&amp;ドロップできます
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack;アセットパネルからテクスチャをレイヤースタックにドラッグ&amp;ドロップ
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack;ジェネレータ、フィルタをメッシュにドラッグアンドドロップできるようにします
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack；外部アセットをメッシュにドロップできるようにする
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;投影&amp;rbrack; UV セット投影モードに新しいUV セットを追加
* &amp;lbrack;QoL&amp;rbrack; ビューポートとレイヤースタックに新しいレイヤーとしてスマートマスクをドラッグ&amp;ドロップ
* &amp;lbrack;QoL&amp;rbrack;マスクで使用した場合に複数の出力を持つジェネレータのセレクタを追加
* &amp;lbrack;QoL&amp;rbrack；塗りつぶし効果の上にシングルチャンネル画像をドラッグ&amp;ドロップできるようにする
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack; CTRL/ALT修飾子をドラッグ&amp;ドロップで使用して、エフェクトやレイヤーを作成する場所や方法を指定
* &amp;lbrack；パス&amp;rbrack；パスパネルでパスの表示を個別に切り替え
* &amp;lbrack;Path&amp;rbrack;パスポイントに変形マニピュレーターを使用できるようにします
* &amp;lbrack;Path&amp;rbrack; 頂点ごとの正接を手動で制御できるようにします
* &amp;lbrack；パス&amp;rbrack;パスのプロパティをコピー/ペースト
* &amp;lbrack;Path&amp;rbrack; 「正接のブレーク」ボタンに空のショートカットを導入
* &amp;lbrack;シェーダー&amp;rbrack; ASM シェーダーの不透明度とTranslucencyのサポートを追加
* &amp;lbrack;シェーダー&amp;rbrack; ASM シェーダーで吸収カラーチャンネルのサポートを追加
* &amp;lbrack;シェーダー&amp;rbrack; ASM シェーダーパラメータの向上ツールチップ
* &amp;lbrack;シェーダー&amp;rbrack; Translucencyチャンネルのデフォルトカラーを黒に変更
* &amp;lbrack；ディスプレイ設定&amp;rbrack;デフォルトでテンポラルアンチエイリアシングを有効にする
* &amp;lbrack；表示設定&amp;rbrack;デフォルトでサブサーフェススキャタリング設定を有効にする
* &amp;lbrack;Substance&amp;rbrack; グラフの入出力からカラースペースプロパティのサポートを追加
* &amp;lbrack;Substance&amp;rbrack; Substanceエンジンをバージョン9.0.3にアップデートする
* &amp;lbrack;UI&amp;rbrack;アプリウィンドウが小さくてもコンテキストツールバーボタンにアクセスできるようにする
* &amp;lbrack；自動ラップ解除&amp;rbrack；制御UV タイル番号(Texel Density)
* &amp;lbrack;ベイク&amp;rbrack; AMD GPU上のGPU レイトレーシングをデフォルトでディアクティベート
* &amp;lbrack；パフォーマンス&amp;rbrack; 16ビット画像に可逆圧縮を適用してプロジェクトのフットプリントを削減
* &amp;lbrack;Python&amp;rbrack; 3D ビューのデフォルトのカメラを処理できるようにします
* &amp;lbrack;Python&amp;rbrack;スクリプトによるメッシュ書き出し機能の表示
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Samples&amp;rbrack；新しいサンプルプロジェクト「French Restaurant Table」を追加
* &amp;lbrack;Content&amp;rbrack; Substanceロゴのアルファを新しいバージョンに更新
* &amp;lbrack;Content&amp;rbrack; 3つのSVGに焦点を当てたマテリアルフィルター（カスタムステッカー、カスタムスプレー、マテリアルへのグラフィック）を追加

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack;対称ツールを使用しない場合のマニピュレーターサイズの変更
* &amp;lbrack;クラッシュ&amp;rbrack; &amp;lbrack;レイヤースタック&amp;rbrack；何も選択されていない場合に画層を作成する
* &amp;lbrack;Project&amp;rbrack;リソースは、未使用のメッシュマップを削除すると破損する可能性があります
* &amp;lbrack;Project&amp;rbrack;イメージの再読み込みまたは再ベイク後にリソースが破損する
* &amp;lbrack；アセット&amp;rbrack;アセットを再ロードすると、お気に入りから削除される
* &amp;lbrack;Import&amp;rbrack;アセットパネルに「結果が見つかりません」と表示されている場合、リソースをインポートできません
* &amp;lbrack;UI&amp;rbrack;コンテキストツールバー矢印が表示されない場合がある
* &amp;lbrack;Substance&amp;rbrack;ブール値の[並べて表示]ボタンはサポートされていません
* &amp;lbrack；レベル&amp;rbrack;マスクで使用するとチャンネルラベルが正しくない
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; glTF/GLBファイルをPainterから書き出すと、物理サイズユニットがなくなります
* &amp;lbrack;Content&amp;rbrack；ぼかしフィルターの強度を16に固定
* &amp;lbrack;Content&amp;rbrack; Color Match filter &quot;target color&quot;画像入力が表示されない

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* AMD上のLinux Waylandでレイヤースタックにクラッシュをドラッグ&amp;ドロップする場合、&amp;lbrack；リソース&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Monterey OSで異方性フィルタリング値を変更する
* &amp;lbrack;クラッシュ&amp;rbrack;イメージ入力として使用されるExr
* &amp;lbrack;クラッシュ&amp;rbrack; 16K 環境マップを使用
* &amp;lbrack；自動ラップ解除&amp;rbrack; texel density controlのUIの問題
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューがhd画面で小さすぎる
* &amp;lbrack;Python&amp;rbrack; TextureStateEventによってトリガーされたUSDの書き出しクラッシュ
* &amp;lbrack;QoL&amp;rbrack;デカールモードでAlphaリソースをドラッグ&amp;ドロップすると、マスクにUV 投影が発生する

### 9.0.1

リリース日： **2023/09/19**&#x200B;概要： **いくつかの改善を含むマイナーなバグ修正リリース**

**追加：**

* &amp;lbrack;Import&amp;rbrack；読み込みウィンドウのデフォルトの読み込み場所を設定
* &amp;lbrack;ベイク処理モード&amp;rbrack;パラメータをデフォルト値にリセットできます
* &amp;lbrack;ベイク処理&amp;rbrack;プロジェクト作成時にベイク処理をペイント解像度に設定
* &amp;lbrack;対称&amp;rbrack; ショートカット Qから対称固有のマニピュレーターをバインド解除
* &amp;lbrack;Menu&amp;rbrack;ヘルプメニューに「ログを表示」オプションを追加
* &amp;lbrack;ビューポート&amp;rbrack;シャドウのレンダリング速度を上げる
* &amp;lbrack;Substance&amp;rbrack; エンジンをバージョン9.0.1にアップデート
* &amp;lbrack;Color Management&amp;rbrack; OCIO構成ファイルには、任意の拡張子を付けることができます
* &amp;lbrack；アセット&amp;rbrack;デカールを使用したSbsarリソースは、ワープ投影に自動設定される必要があります
* &amp;lbrack;Path&amp;rbrack; UIとギズモが非表示の状態でパスツールを操作しようとすると、メッセージが表示されます

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack; Alt +パスパネル上でドラッグ
* &amp;lbrack；リソースのインポート&amp;rbrack；インポートするリソースを削除するときにランダムなクラッシュが発生する
* 圧縮GLBファイルの読み込み時に発生するクラッシュ
* UVを共有するメッシュにペイントする際の問題
* キャッシュの再計算時または読み込み時にメッシュフラッシュが黒くなる
* &amp;lbrack；プロパティ&amp;rbrack;ドロップダウンでパラメーターをリセットする右クリックメニューが表示されない
* &amp;lbrack；レベル&amp;rbrack；前のレベルによってロックされた入力スライダー
* &amp;lbrack;AMD&amp;rbrack;&amp;lbrack;Sparse&amp;rbrack; SVTオプション（アクティブ化した場合、アーティファクトが生成される）
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack;頂点をダブルクリックしたときのワープ&amp;rbrack; クラッシュ
* &amp;lbrack;Path&amp;rbrack; UIとパスをベイク処理モードで表示
* &amp;lbrack;AMD&amp;rbrack;テクスチャが可視性で遊んでいるときに失われる
* &amp;lbrack；スパース&amp;rbrack;メッシュの向きを変えると解像度が低すぎる

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。

### 9.0.0

リリース日： **2023/06/20**&#x200B;概要： **3Dカーブを許可するペイントとパス、新しいベースマテリアル、従来のマテリアルのクリーンアップ、3Dカーブの新しいプリセットを含むメジャーリリース**

**追加：**

* &amp;lbrack;Path&amp;rbrack; [パスツールに沿って新しいペイントを追加]
* &amp;lbrack;Path&amp;rbrack;パスツールに空のショートカットを追加する
* &amp;lbrack;Path&amp;rbrack；既存のパスに新しいポイントを追加できるようにします
* &amp;lbrack;Path&amp;rbrack; ショートカットを追加して現在のパスの作成を終了
* &amp;lbrack；パス&amp;rbrack;パスのブラシプロパティの編集を許可
* &amp;lbrack;Path&amp;rbrack;ポイント配置時に正接を自動調整する(&amp;R)
* &amp;lbrack;Path&amp;rbrack;ポイント移動時に正接を再計算する(&amp;R)
* &amp;lbrack；パス&amp;rbrack；新しく作成したポイントをメッシュのサーフェスにスナップ
* &amp;lbrack；パス&amp;rbrack; 頂点ごとの圧力を編集できるようにします
* &amp;lbrack；パス&amp;rbrack；新しく作成したポイントの圧力を隣接するポイントから調整します。
* &amp;lbrack;Path&amp;rbrack;ポイントをスムーズ/コーナーに変換（正接の区切り）
* &amp;lbrack；パス&amp;rbrack；新しく追加したポイントをすぐに移動できるようにします
* &amp;lbrack；パス&amp;rbrack；既存のパスからポイントを削除できるようにします
* &amp;lbrack;Path&amp;rbrack;パスの方向を反転できるようにします
* &amp;lbrack;Path&amp;rbrack; ビューポート内のパスを選択できるようにします
* &amp;lbrack;Path&amp;rbrack;マーキー選択でパスポイントを選択できるようにします
* &amp;lbrack;Path&amp;rbrack;パスのすべてのポイントを選択するCTRL-Aショートカットを導入
* &amp;lbrack；パス&amp;rbrack;パスを閉じることを許可
* &amp;lbrack;Path&amp;rbrack;プロパティでパスアップ軸を指定できるようにします
* &amp;lbrack;Path&amp;rbrack; 頂点コントロールメニューをコンテキストツールバーに追加
* &amp;lbrack;Path&amp;rbrack;パスツールにペイント/消去/指先モードを導入
* &amp;lbrack;Path&amp;rbrack; ビューポート内のパスのビジュアルフィードバックを作成
* &amp;lbrack;Path&amp;rbrack;パスの方向の視覚的インジケータを追加
* &amp;lbrack;Path&amp;rbrack;パスの表示設定にラインThicknessを追加
* &amp;lbrack;Path&amp;rbrack;パスUIを非表示にする
* &amp;lbrack；パス&amp;rbrack；現在選択されているレイヤーのパスを一覧表示するパスを追加パネル
* &amp;lbrack；パス&amp;rbrack；パスパネルのパスの上にカーソルを置いたときに視覚的なフィードバックを追加
* &amp;lbrack；パス&amp;rbrack;パスツールが選択された場合に常にパスパネルを表示
* &amp;lbrack；パス&amp;rbrack;パスパネルでパスの名前変更、削除、コピー、カット、複製を許可
* &amp;lbrack;Path&amp;rbrack;パスツールを使用して2D ビューポートで操作しようとするとメッセージが表示される
* &amp;lbrack;Library&amp;rbrack；新規コンテンツの統合（パスツールとベースマテリアル）
* &amp;lbrack;動的ストローク&amp;rbrack;動的ストロークの距離プロパティを追加
* &amp;lbrack;動的ストローク&amp;rbrack;サイズと間隔のプロパティを動的ストロークに追加
* &amp;lbrack;動的ストローク&amp;rbrack; 動的ストロークの開始/中間/終了プロパティを追加
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; USDフォーマットのプロジェクト設定パラメータを表示
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; USDフォーマットのプロジェクト作成パラメータを表示
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;USD&amp;rbrack；書き出したUSDファイル内にプロジェクトパス情報を追加
* &amp;lbrack;GLTF&amp;rbrack; GLTFファイルの再読み込み時にライブラリのテクスチャを更新
* &amp;lbrack;シェーダー&amp;rbrack；方向が異なるUV アイランドのシームの斑点を軽減
* &amp;lbrack;エンジン&amp;rbrack; Substanceエンジンバージョン9.0にアップデート

**修正済み：**

* &amp;lbrack;Import&amp;rbrack; テクスチャを含む一部のGLBがPainterでテクスチャを取得しない
* &amp;lbrack;AMD&amp;rbrack；すべての3D 投影塗りつぶしの境界上の斑点
* &amp;lbrack;エンジン&amp;rbrack;レイヤーの表示/非表示を切り替えるとテクスチャが壊れる(&amp;r)
* 描画モードを変更すると、&amp;lbrack;エンジン&amp;rbrack;テクスチャが空になる場所がある
* &amp;lbrack;エンジン&amp;rbrack;テクスチャ/投影が空のワープモードになることがある
* &amp;lbrack;Iray&amp;rbrack;レンダリングの保存時に反復を0にリセット
* &amp;lbrack;Log&amp;rbrack;ファイル/新規を実行するときのUSDエラーメッセージ

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;レイヤースタック&amp;rbrack；入力ソースがレイヤーごとに保存されない

## バージョン8

### 8.3.1

リリース日： **2023/04/27**

**追加：**

* &amp;lbrack;ベイク処理モード&amp;rbrack; ビューポートビジュアライゼーションの表示/非表示を切り替える（空の）ショートカットを追加(&amp;L)
* &amp;lbrack;ベイク処理モード&amp;rbrack; 「ベイク処理メッシュを隠す」ボタンを使用すると、常にローポリゴンが表示される
* &amp;lbrack;ベイク処理モード&amp;rbrack；現在のテクスチャセットに基づいて名前で一致するサフィックスを表示
* &amp;lbrack;Import&amp;rbrack; GLTFバイナリファイル(glb)のサポートを追加
* &amp;lbrack;テクスチャセットリスト&amp;rbrack;メニューを追加してシェーダーインスタンスを選択または作成
* &amp;lbrack;テクスチャセットリスト&amp;rbrack;テクスチャセットとUV タイルの解像度をすばやく変更できます
* &amp;lbrack;物理サイズ&amp;rbrack; UV 投影で物理サイズを使用する際のマニピュレーターのビヘイビアーを改善する
* &amp;lbrack;UI&amp;rbrack; 「別名で保存」をメインファイルメニューに戻す
* &amp;lbrack;UI&amp;rbrack; UIレイアウトにビュー選択を保存（2Dのみ、3Dのみ、両方）
* &amp;lbrack;USD&amp;rbrack;サポートされていないUSDシェイプを使用したプロジェクト作成時のエラーメッセージがあまり曖昧でない
* &amp;lbrack;Python&amp;rbrack; ベイク処理の進行状況に従ってベイク処理イベントを追加
* &amp;lbrack;Python&amp;rbrack;烘焙のキャンセルを許可
* &amp;lbrack;Python&amp;rbrack；書き出しのファイルの種類とビット深度に「出力テンプレートに基づく」を表示
* &amp;lbrack;Python&amp;rbrack; TextureStateEvent.Updateの更新時間を表示

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack;プロジェクトを閉じるときに発生する稀なクラッシュ
* &amp;lbrack;クラッシュ&amp;rbrack; &amp;lbrack;ベイク処理&amp;rbrack；特定のプロジェクトのHeightまたは曲率とメッシュマップシンクをアクティブ化
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;シェーダーインスタンス作成後にマテリアルを追加する際のスクリプト&amp;rbrack;クラッシュ
* &amp;lbrack;ベイク処理モード&amp;rbrack；ニュートラルマテリアルのAO強度が影響を与えない
* &amp;lbrack;ベイク処理モード&amp;rbrack;モデルがロードされる前にベイク処理モードに切り替えると、クラッシュが発生します。
* &amp;lbrack;ベイク処理モード&amp;rbrack; 「ベイク処理プロセス」タブにエラーメッセージがありません
* &amp;lbrack;ベイク処理モード&amp;rbrack;ニュートラルマテリアルの設定は、メッシュの再読み込み後は無効です
* &amp;lbrack;ベイク処理モード&amp;rbrack;ビューポート区切りは、モードごとに保存されるのではなく、グローバルに保存されます。
* &amp;lbrack;ベイク処理モード&amp;rbrack；可視化の問題：平均法線がケージサーフェスを変えない
* &amp;lbrack；カラーマネジメント&amp;rbrack; OCIO env varが存在する場合、カラースペースの自動検出設定が無効になる
* &amp;lbrack;Content&amp;rbrack; Mask OutlineフィルターにHeight入力を含む斑点がある
* &amp;lbrack;Content&amp;rbrack; 勾配ぼかしフィルターの適用度スライダーが1.0に固定されています
* &amp;lbrack;Interop&amp;rbrack; SamplerからGLTFでプロジェクトを作成できません
* &amp;lbrack;レイヤースタック&amp;rbrack;投影タイリングの値がマニピュレーターで正しく更新されない
* &amp;lbrack;Linux&amp;rbrack;グラフィックタブレットペンとHDPIが100%を超えるカーソルの間のオフセット
* &amp;lbrack；プロジェクト作成後にメッシュを再読み込みするときにPython&amp;rbrack; クラッシュが発生する
* &amp;lbrack;Substance&amp;rbrack; 3D ノイズがメッシュの再読み込み後に壊れる
* &amp;lbrack;UV タイル&amp;rbrack;UV 投影のオフセットを1にクランプ
* &amp;lbrack;ビューポート&amp;rbrack；直線のビジュアルフィードバックが表示されなくなった
* &amp;lbrack;WhatsNew&amp;rbrack；機能タイトルの行の改行が正しくありません

**既知の問題：**

* &amp;lbrack;Import&amp;rbrack; テクスチャを含む一部のGLBがPainterでテクスチャを取得しない

### 8.3.0

*（リリース：2023年1月10日*）概要： **新しいベイクモード、USDファイルの新しい読み込みと書き出し、UV 投影の物理サイズサポートを備えたメジャーリリース**

**追加：**

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク処理プロセス専用の新しいベイク処理モード

* &amp;lbrack;ベイク処理モード&amp;rbrack; ショートカットを設定してベイク処理モードをF8モードに切り替え

* &amp;lbrack;ベイク処理モード&amp;rbrack; ビューポートに「ベイク処理を開始」および「キャンセル」ボタンを追加

* &amp;lbrack;ベイク処理モード&amp;rbrack; テクスチャセットリストにベイク処理選択項目を追加

* &amp;lbrack;ベイク処理モード&amp;rbrack；新しいメッシュマップベイカーを追加ウィンドウでベイカーを選択

* &amp;lbrack;ベイク処理モード&amp;rbrack；新しいメッシュマップ設定を追加ウィンドウでベイク処理設定を編集

* &amp;lbrack;ベイク処理モード&amp;rbrack；新しいベイク処理ログウィンドウを追加してベイク処理プロセスに従う

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク処理パラメータの追加とヒストリーウィンドウへの操作の取り消し

* &amp;lbrack;ベイク処理モード&amp;rbrack; メッシュマップ設定にブレッドクラムを追加

* &amp;lbrack;ベイク処理モード&amp;rbrack; メッシュマップベイカーウィンドウにメッシュマップサムネールを追加

* &amp;lbrack;ベイク処理モード&amp;rbrack; 3D ビューポートで折りたたみ可能な表示設定を追加

* &amp;lbrack;ベイク処理モード&amp;rbrack;ハイポリゴンメッシュの表示/非表示を切り替えるビジュアライゼーション設定を追加

* &amp;lbrack;ベイク処理モード&amp;rbrack; ケージメッシュとワイヤーフレームの表示/非表示を切り替える視覚化設定を追加

* &amp;lbrack;ベイク処理モード&amp;rbrack;ローポリメッシュを表示/非表示にするビジュアライゼーション設定を追加

* &amp;lbrack;ベイク処理モード&amp;rbrack; UVシームのないハードエッジをエラーとして表示するビジュアライゼーション設定を追加

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク処理ログが表示されない場合は、メッシュとベイクのエラーをビューポートに通知します。

* &amp;lbrack;ベイク処理モード&amp;rbrack；すべてのテクスチャセットでベイカー設定を同期するアクションを追加

  ベイカーウィンドウで、名前の横にあるリンクアイコンをクリックすると、各ベイカー（および一般的な設定）をテクスチャセット間で同期できます。 この操作を実行すると、同じパラメーターを共有するテクスチャセットーを選択できるウィンドウが開きます。

* &amp;lbrack;ベイク処理モード&amp;rbrack; ベイカー設定のコピー&amp;ペーストにアクションを追加

  ベイカーウィンドウでは、ウィンドウ上部の専用メニューまたは右クリックして表示されるコンテキストメニューから、テクスチャセット間で各ベイカー設定をコピーおよびペーストする操作が可能です。

* &amp;lbrack;ベイク処理モード&amp;rbrack；エラーから適切な設定にジャンプするには、ベイク処理ログの「追加」ボタン

  ベイカーが失敗した場合や、メッシュが正しく読み込まれない場合は、ベイクログにエラーメッセージが表示されます。 メッセージの横のボタンをクリックすると、ベイカーとメッシュマップ設定ウィンドウが開き、関連する設定が表示されます。 これにより、問題の原因を簡単に特定して、解決できます。

* &amp;lbrack;ベイク処理モード&amp;rbrack;メニューを追加してテクスチャセットとベイカーの選択内容を管理

  「テクスチャセットリスト」と「メッシュマップベイカー」ウィンドウの両方に、選択範囲のコピーと反転に役立つ小さなアクションメニューが追加されました。

* &amp;lbrack;ベイク処理モード&amp;rbrack;テクスチャセットごとにベイカー選択リストを分割

* &amp;lbrack;ベイク処理モード&amp;rbrack;テクスチャセットごとに共通設定を分割

* &amp;lbrack;ベイク処理モード&amp;rbrack;インタフェースをフリーズせずにハイポリおよびケージメッシュをロード

* &amp;lbrack;ベイク処理モード&amp;rbrack; ビューポート進行状況バーを使用してメッシュの読み込みを表示

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク処理ログにメッシュの読み込み状況を追加

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク中にビューポートのメッシュをオンにする

* &amp;lbrack;ベイク処理モード&amp;rbrack；現在のメッシュビューポートの表示設定に基づいてベイク処理順序を設定

* &amp;lbrack;ベイク処理モード&amp;rbrack；暗黙的なベイク処理ケージをビューポートに表示

  カスタムメッシュファイルを使用していない場合、自動ケージメッシュが生成され、ビューポートに表示されます。 このサイズは、ベイク処理の共通設定の[最大前頭距離]パラメータに基づきます。 メッシュを使用して、ローとハイのポリゴン間のマッチングがどの程度行われるかを示します。

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク処理ログの名前で一致するメッシュ名のリストを表示

* &amp;lbrack;ベイク処理モード&amp;rbrack;ニュートラルマテリアルを使用して3Dモデルをビューポートで表示

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク処理モードでエンジン計算を無効にする

* &amp;lbrack;ベイク処理モード&amp;rbrack;ベイク中にアプリを終了すると警告が表示されます

* &amp;lbrack;ベイカー&amp;rbrack;アンチエイリアス設定ラベルを更新

  アンチエイリアス設定値は「スーパーサンプリング」に名前が変更され、明示的な乗数を使用して動作を明確にしています。

* &amp;lbrack;ベイカー&amp;rbrack; ベイカーをバージョン2.5.7にアップデートします。

* &amp;lbrack;USD&amp;rbrack; Universal Scene Description(USD)ファイルの読み込みと書き出し

* &amp;lbrack;USD&amp;rbrack; USDファイルを選択するときにUSDオプションを新規プロジェクトウィンドウに追加

* &amp;lbrack;USD&amp;rbrack；新しいスコープとバリアントの追加を選択ウィンドウ

  USDファイルを読み込む際に、「新規プロジェクト」または「プロジェクト構成」ウィンドウで「変更」ボタンをクリックすると、読み込むUSDファイルの部品とバリアントを選択できます。

* &amp;lbrack;USD&amp;rbrack; 「再分割レベルを追加」オプション

  サブディビジョンを含むUSD メッシュファイルを使用して新しいプロジェクトを作成する場合は、スライダーを使用してサブディビジョンのレベルを選択できます。 プロジェクトは、分割されたメッシュで作成されます。 このレベルは、プロジェクト構成を介して変更できます。

* &amp;lbrack;USD&amp;rbrack; USDスキンメッシュを特定のフレームで読み込む

  アニメーションを含むUSD メッシュファイルを使用して新しいプロジェクトを作成する場合は、埋め込まれたタイムラインシーケンスを示すスライダーを使用してフレームを選択できます。 このフレームは、プロジェクト構成を介して変更できます。

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; USDファイルをエクスポートするオプションを追加

  書き出しテクスチャウィンドウに、新しい「USDを書き出し」チェックボックスが追加されました。 オンにすると、任意のテンプレートを使用してUSDファイルとテクスチャマップを書き出すことができます。

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack; メッシュ書き出しにUSDファイルフォーマットを追加

* &amp;lbrack;USD&amp;rbrack；既存の「USD PBR Metal ラフネス」書き出しプリセットの名前をより明確に変更

  以前は「USD PBRメタルラフネス」として知られていましたUSDの書き出しテンプレートには、書き出しテクスチャ/出力テンプレート/USDz(Apple AR)から引き続きアクセスできます。

* &amp;lbrack；自動ラップ解除&amp;rbrack; パッキングのロック方向を追加

  自動ラップ解除設定の新しいオプションにより、パッキング機能を使用するときに既存のUV アイランドの向きを保持できます。 新規プロジェクト/自動ラップ解除オプション/UV アイランド方向からアクセスできます。

* &amp;lbrack;物理サイズ&amp;rbrack；塗りつぶしエフェクト/レイヤーで物理サイズを自動的に使用する設定を追加

  物理サイズが埋め込まれたマテリアルを使用する場合に、自動で物理サイズスケールに切り替える新しいオプションが追加されました。 これは、新規プロジェクト、またはマテリアルを割り当てるときに編集/プロジェクト設定/物理サイズ/塗りつぶしレイヤースケーリングを物理サイズに切り替えを介して、プロジェクトごとに有効にできます。

* &amp;lbrack;物理サイズ&amp;rbrack;UV 投影用に物理サイズを表示

  物理サイズの拡大・縮小がUV 投影で利用できるようになりました。これにより、メッシュの物理サイズに基づいてマテリアルの自動サイズ変更が可能になります。 これは、塗りつぶしレイヤーまたはエフェクトのプロパティウィンドウのスケール/物理サイズを使用して選択できます。

* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack;アプリケーションバージョンのクエリを許可

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack；新しいベイク処理パラメーターと一致するようにAPIを更新

* &amp;lbrack；スクリプティング&amp;rbrack;&amp;lbrack;Python&amp;rbrack;ベイク処理モジュール：ベイク処理パラメータを編集

* &amp;lbrack；スクリプティング&amp;rbrack;&amp;lbrack;Python&amp;rbrack;ベイク処理モジュール：ベイクの起動/キャンセル

* &amp;lbrack；スクリプティング&amp;rbrack;&amp;lbrack;Python&amp;rbrack; ベイク処理モジュール： select 曲率方式

* &amp;lbrack；スクリプティング&amp;rbrack;&amp;lbrack;Python&amp;rbrack; ベイク処理モジュール：ベイカー/uvタイルの選択

* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack; ベイク処理モジュール：すべてのテクスチャセットでベイカー設定を同期

* &amp;lbrack;SVT&amp;rbrack; AMD GPUで疎ハードウェアサポートを有効にする

  AMD GPUで、スパース仮想テクスチャシステムのハードウェアアクセラレーションを有効にできるようになりました。 この設定は、一般環境設定で自動的に有効になります。

* &amp;lbrack;投影&amp;rbrack；円柱投影のパラメータ名を変更

  「Cylinder Cap Culling」パラメーターの名前が「バックフェースカリング」に変更され、アクションがより適切に表現されるようになりました。 関連付けられたツールチップは、それに応じて調整されます。

* &amp;lbrack;Project&amp;rbrack;アプリケーションのバージョンをプロジェクトに保存し、スクリプトを使用して取得

  バージョン8.2以降では、アプリケーションのバージョンは保存時にsppファイル内に保存されるようになりました。 このバージョン番号は、Python APIのプロジェクトモジュールにあるlast_saved_substance_painter_version()関数を使用して取得できます。 8.2より前に作成されたプロジェクトの場合、戻り値はnullになります。

* &amp;lbrack;Import&amp;rbrack; 3Dモデルの一般的な読み込み時間を短縮

  メッシュの一般的な読み込み時間を改善しました。 例えば、ベイク処理用に高ポリゴンのメッシュを読み込む際の待ち時間を短縮できます。 最適化は、特にOBJファイルの読み込みに適用されます。

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack；特定のスタックでフィルタのチャンネルを変更する

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;M1&amp;rbrack; レイヤースタックを作成して塗りつぶしレイヤーを離れるときのクラッシュ

  この問題は、Mac OS 13(Ventura)にアップデートすることで修正できます。

* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack；間違った型でui.add_dock_widget()を使用した場合のPython&amp;rbrack; クラッシュ

* &amp;lbrack;ベイク&amp;rbrack;ベイクが失敗したときのログのエラーメッセージが不完全である

* &amp;lbrack;ベイク処理&amp;rbrack; ベイク処理の終了時にメモリが解放されない(&amp;r)

* &amp;lbrack;エンジン&amp;rbrack; テクスチャキャッシュが、エフェクトの表示/非表示を変更しても更新されない

* &amp;lbrack；書き出し&amp;rbrack; 2D ビューがランダムに均一マップを書き出す

* &amp;lbrack;Project&amp;rbrack;プロジェクトを大きなメッシュで保存する際のメモリ割り当てエラー

* &amp;lbrack;ビューポート&amp;rbrack; TAAでペイントすると斑点が発生する場合がある(&amp;lbrack;C&amp;rbrack; TAA)

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;レイヤースタック&amp;rbrack；入力ソースがレイヤーごとに保存されない

### 8.2.0

*（リリース：2022年10月6日*）概要： **新しいオンボーディングパネル（新しいウェルカムパネルと新機能パネル）、SBSARへの書き出し、フォルダーの効果、生活の質を高めるいくつかの改善、およびバグ修正を含むメジャーリリース。**

**追加：**

* &amp;lbrack；オンボーディング&amp;rbrack；新規ユーザーを歓迎するオンボーディングパネル

  新しいCCユーザーがPainterを初めて開いたときの新しいようこそ画面が追加されました。

* &amp;lbrack;Onboarding&amp;rbrack；新機能の検出可能性を向上させる新機能パネル

  主な新機能が表示される新しい「新機能」画面を追加しました。 メジャーアップデート後にPainterを初めて開くと、このアイコンは自動的に表示されます。このアイコンにアクセスするには、ヘルプ/新機能を選択します。

* &amp;lbrack;Onboarding&amp;rbrack; 「古いようこそ」の名前を「ホーム画面」に変更

  新しいようこそ画面と混同されないように、古いようこそ画面の名前をホーム画面に変更しました。

* &amp;lbrack;UI&amp;rbrack；高DPI画面のスケーリングの問題を解決

  カスタム表示スケーリングを使用した高解像度画面でのPainter UI適用を改善しました。

* &amp;lbrack;UI&amp;rbrack; UIの永続的なエラーメッセージを回避する

  以前のプロジェクトのエラーメッセージが、下部のステータスバーから削除されるようになりました。

* &amp;lbrack;UI&amp;rbrack；再作業保存メニュー

  追加の保存オプションがサブメニューにグループ化され、一部のオプションの名前が変更されて一貫性が保たれます。

* &amp;lbrack;UI&amp;rbrack; UIレイアウトの保存と書き出し/共有

  ウィンドウメニュー内には、UIレイアウトをファイルに保存し、再ロードするための新しいアクションが追加されています。 ペイントレイアウトとレンダリングレイアウトは別々に保存されます。 UIレイアウトを保存、リセット、読み込みするための様々な機能が「substance_painter.ui」に追加されました。

* レイヤーの描画モード/不透明度にコピー/ペーストアクションを追加

  レイヤーの右クリックメニューに「描画オプション」という新しいエントリを追加しました。 レイヤー間ですべてのチャンネルの描画モードと不透明度をコピー&amp;ペーストできます。

* レイヤーのすべてのチャンネルに描画モード/不透明度を適用する

  レイヤーの描画モードと不透明度に右クリック機能が追加されました。これにより、現在クリックしている設定をすべてのチャンネルに適用できます。

* キーボードショートカットでメッシュを再読み込みする(Ctrl+Shift+R)

  編集可能なショートカットが追加され、最後に使用可能な設定でメッシュファイルが再読み込みされるようになりました。 編集/再読み込みメッシュからもアクセスできます。

* Substanceパラメーターをデフォルトにリセット

  .sbsarリソースの下部のプロパティに、リソースをデフォルトにリセットできる新しいボタンが追加されました。

* ペイントブラシをデフォルトにリセット

  「プロパティ」の「ブラシ」セクションに新しいメニューが追加され、デフォルトの基本ブラシにリセットできるようになりました。

* 右クリックして個々のSubstanceパラメーターをデフォルトにリセット

  .sbsarリソース内の個々のパラメーターを右クリックでリセットできるようになりました。

* &amp;lbrack；アセットパネル&amp;rbrack; 「ピン」のお気に入りアセットをアセットパネルの上に表示

  ライブラリアセットに新しい右クリックオプションが追加され、パネルの上部にお気に入りとしてピンできるようになりました。 保存済みの検索を使用して、お気に入りのすべてのアセットを表示することもできます。

* &amp;lbrack；アセットパネル&amp;rbrack;アセットの削除、再読み込み、名前変更

  ユーザーライブラリのアセットを削除、再ロード、名前を変更するための右クリックメニューオプションが追加されました。 ディスク上のライブラリの場所から直接削除され、元の場所から再ロードされます。 .abrや.sbsarなどのパッケージに含まれるアセットは、個別に編集できません。

* &amp;lbrack;カラー選択&amp;rbrack; カラー選択効果に描画モードを追加

* &amp;lbrack;レイヤースタック&amp;rbrack;フィルターに描画モードと不透明度を追加

* &amp;lbrack;レイヤースタック&amp;rbrack;塗りつぶしレイヤー/エフェクトに128より大きいタイリング値を許可

* &amp;lbrack;レイヤースタック&amp;rbrack;塗りつぶしレイヤー/効果の円柱投影のシリンダキャップ

  塗りつぶしレイヤープロパティの円柱投影に、円柱キャップを削除するオプションが追加されました。

* &amp;lbrack;Log&amp;rbrack; UV タイルプロジェクトを作成しようとするときに、メッシュパーツが負のスペースにある場合にエラーメッセージを表示します

  UV部分が負のスペースで見つかったため、UV タイルプロジェクトを作成できない場合のエラーメッセージがより明確になりました。

* &amp;lbrack；プロジェクト&amp;rbrack;プロジェクトを開くときに、エラーメッセージ「データが最新すぎます」にバージョンを表示する

  アプリケーションにとって新しすぎるプロジェクトを開くと、エラーメッセージにプロジェクトのバージョンが表示されるようになり、適切なアプリケーションバージョンの特定が容易になりました。

* &amp;lbrack;ビューポート&amp;rbrack；下からメッシュを照らすことができます

  「ローカル」に設定した場合に環境マップの照明を環境に合わせるために、 Display Settings > Environment > Environment settingsに新しいカメラアラインメントカメラが追加されました。

* &amp;lbrack;ビューポート&amp;rbrack；表示R、G、B、Alphaのビューポート（ソロ表示モード）

  ディスプレイ設定/ビューポート設定/チャンネルディスプレイに、シングルディスプレイモードでチャンネルのR、G、BまたはAlphaコンポーネントのみを表示できる新しいカラーチャンネル設定が追加されました。

* &amp;lbrack;シェーダー&amp;rbrack;ユーザチャンネルをマテリアルレイヤシェーダでRGBAとして設定できるようにします

  マテリアルレイヤリング用のシェーダー内でテクスチャセットチャンネル設定を行う際に、デフォルト値から外れるチャンネルのフォーマットを指定できるようになりました。 これにより、特にグレースケールのみではなくカラーユーザチャンネルを要求できます。

* &amp;lbrack;Export&amp;rbrack; テクスチャをSBSARとしてエクスポートできるようにします

  ファイル/書き出しテクスチャウィンドウを使用してテクスチャを書き出す場合、SBSAR（Substanceアーカイブ）ファイルのフォーマットを選択して一緒に再グループ化できます。 SBSARのコンテンツは、使用される出力テンプレートによって駆動されます。 sbsar ファイル形式は、書き出しプリセットで設定することもできます。 ハイブリッド構成（SBSAR +その他の形式）を使用する場合、SBSARを対象とするテクスチャはグループ化され、残りは同時に書き出されます。

* &amp;lbrack；書き出し&amp;rbrack; EXRファイルフォーマットの16ビットオプションを表示

  EXR テクスチャファイルの書き出し時に、書き出し設定ウィンドウで16 bit（ハーフ浮動小数）または32 bit(浮動小数)をテクスチャできるようになりました（書き出し設定と書き出しプリセットの両方）。 古いプロジェクトと古い書き出しプリセットは、古い動作を反映するためにデフォルトで16fビットに設定されます。

* &amp;lbrack;Python&amp;rbrack; テクスチャセットがいつ変更されたかを知らせるイベントを追加

  新しい「substance_painter.event.TextureStateEvent」により、ペイントストローク、新しいチャンネルの追加、チャンネルの削除などによってテクスチャセットが変更された日時を知ることができます。

* &amp;lbrack;Python&amp;rbrack; テクスチャセットの設定でメッシュマップリソースの取得と設定を可能にする

  メッシュマップリソースを取得および設定するための新しい関数が「substance_painter.project」モジュールに追加されました。 これらの関数は、テクスチャセット設定で参照されるメッシュマップを更新するために使用できます。

* &amp;lbrack；プラグイン&amp;rbrack；他のJSプラグインを取得するオプションを削除

  非推奨の共有webサイトでホストされたため、JavaScriptプラグインを取得するオプションを削除しました。

* &amp;lbrack;Content&amp;rbrack；新しいRobloxテンプレートの追加とプリセットの書き出し

  新しいRobloxの「マテリアルバリアント」および「サーフェスの外観」プロジェクトテンプレートと書き出しプリセットが追加され、PBRテクスチャをRobloxに簡単に書き出せるようになりました。 テンプレートには、ファイル/新規プロジェクトウィンドウからアクセスできます。

* Substance engineを最新バージョンにアップデート(8.6.3)

* &amp;lbrack;Steam&amp;rbrack; Apple Siliconチップセット(Apple M1 / M2)用に最適化されたビルド

**修正済み：**

* 16k exrを使用する場合のクラッシュ

* &amp;lbrack;クラッシュ&amp;rbrack; Ctrl Z シェーダーインスタンスの削除後

* &amp;lbrack;Iray&amp;rbrack; IoRが一部のシェーダで1にブロックされる

* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;ベイク処理&amp;rbrack；一部のhigh-polyがロードに失敗する

* &amp;lbrack；カラーマネジメント&amp;rbrack;フィルター付きUIのカラースペース名が正しくない

* &amp;lbrack;Python&amp;rbrack; import関数から返されるリソースオブジェクトに型がありません

  PythonでSubstanceパッケージをインポートするとき、関数はグラフではなくパッケージを返していました。 リソースモジュールは、Substanceパッケージのグラフを取得するための関数とパラメーターを提供するようになりました。

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;レイヤースタック&amp;rbrack；入力ソースがレイヤーごとに保存されない
* &amp;lbrack;Painting&amp;rbrack; Temporal anti aliasingでペイントすると斑点が発生する場合がある
* &amp;lbrack；書き出し&amp;rbrack; 2D ビューがランダムに均一マップを書き出す

### 8.1.3

*（リリース：2022年8月25日*）概要： **マイナーバグ修正リリース**

**追加：**

* Iray SDK 1.6にアップデートする

**修正済み：**

* &amp;lbrack；古い障害シェーダーを持つシェーダー&amp;rbrack; クラッシュ
* &amp;lbrack;マテリアルレイヤー&amp;rbrack；のマテリアルが、プロジェクトを再度開くと消えることがある

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;レイヤースタック&amp;rbrack；入力ソースがレイヤーごとに保存されない
* &amp;lbrack;クラッシュ&amp;rbrack; Ctrl Z シェーダーインスタンスの削除後
* &amp;lbrack;Iray&amp;rbrack; IoRは、一部のシャドウで1にブロックされています

### 8.1.2

*（リリース：2022年7月19日*）概要： **マイナーバグ修正リリース**

**追加：**

* &amp;lbrack；自動ラップ解除&amp;rbrack；セグメンテーションアルゴリズムを選択するための新しいオプション「有機的メッシュ用に最適化」
* &amp;lbrack;物理サイズ&amp;rbrack; New Project and Project Configurationでユニットオプションを表示
* &amp;lbrack；カラーマネジメント&amp;rbrack; ACE使用時にモニター表示をデフォルトで使用する
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;Python&amp;rbrack;プロジェクト作成時にACE env-varプリセットファイルを考慮
* &amp;lbrack；カラーマネジメント&amp;rbrack；設定変更時に新規プロジェクトウィンドウでカラーマネジメント設定をリセット
* &amp;lbrack；カラーマネジメント&amp;rbrack; env-varが存在する場合は、OCIO設定へのアクセスを無効にする
* &amp;lbrack；カラーマネジメント&amp;rbrack;パラメーターが存在しなくなったときにACE設定を安全に更新する
* Substance engineをバージョン8.6.0にアップデートする
* &amp;lbrack；書き出し&amp;rbrack; ディスプレイスメントのサポートで新しいGLTF書き出しプリセットを追加
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;リソース情報（カスタムメタデータを含む）を取得
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；各テクスチャセットのメッシュ名のリストを照会する関数を追加
* &amp;lbrack;Content&amp;rbrack；新規ブレンダーテンプレートの追加とプリセットの書き出し

**修正済み：**

* Irayを起動するときにクラッシュが発生する(&amp;lbrack;MacOS&amp;rbrack;)
* &amp;lbrack；サムネール&amp;rbrack; シェルフサムネールが正しく読み込まれない
* 複数のUVチャンネルは無視されます
* &amp;lbrack；自動ラップ解除&amp;rbrack；長い島を分割する際の不要な計算
* &amp;lbrack；自動ラップ解除&amp;rbrack;オプション長い島は考慮されません
* &amp;lbrack；自動ラップ解除&amp;rbrack; UVを再パックするときに余分なデータ（頂点カラー）が失われる
* &amp;lbrack;UI&amp;rbrack;カラーマネジメントが有効な場合のプロパティウィンドウの水平スクロールバー
* &amp;lbrack；カラーマネジメント&amp;rbrack; OCIO構成にsubstance_3d_painter_standard_srgbロールがありません
* &amp;lbrack;Generator&amp;rbrack;ユーザデータの誤った使用が「無効」になっています
* &amp;lbrack;Color Management&amp;rbrack; Color Space &quot;Not Compatible&quot;のドロップダウンはクリックできません
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;シェーダー&amp;rbrack; sRGBオーバーライドの定義が機能しない
* &amp;lbrack;Generator&amp;rbrack;ユーザデータの「disable」の誤った使用
* &amp;lbrack;レイヤースタック&amp;rbrack;UV タイルプロジェクトでプレビューが壊れる
* &amp;lbrack;シェーダー&amp;rbrack; APIドキュメントが完全に最新のBent normalsではありません
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Interoperability&amp;rbrack；特殊文字を使用してStagerに送信できない
* &amp;lbrack;Content&amp;rbrack；一部のブラシプリセットのサムネールが空か、暗すぎる

**既知の問題：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。
* &amp;lbrack;レイヤースタック&amp;rbrack；入力ソースがレイヤーごとに保存されない
* &amp;lbrack;クラッシュ&amp;rbrack; Ctrl Z シェーダーインスタンスの削除後
* &amp;lbrack;Iray&amp;rbrack; IoRが一部のシェーダで1にブロックされる
* &amp;lbrack；古い障害シェーダーを持つシェーダー&amp;rbrack; クラッシュ

### 8.1.1

*（リリース：2022年6月28日*）概要： **マイナーリリースの修正プログラム**

**追加：**

* &amp;lbrack;レイヤースタック&amp;rbrack; Altがマスクをクリックしてもエフェクトの選択が解除されない

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack；古いプロジェクトを開くソロ表示モード
* &amp;lbrack;クラッシュ&amp;rbrack;プロパティのジェネレータを削除
* &amp;lbrack;テクスチャセット設定&amp;rbrack；通常/Ambient occlusionミキシングと通常の方式へのHeightが壊れています
* &amp;lbrack；書き出し&amp;rbrack; 拡散パディングを使用してテクスチャを書き出すと黒いマップがレンダリングされる

**既知の問題：**

* MontereyでIrayを起動する際に発生するMacOSのクラッシュ(&amp;lbrack;)
* &amp;lbrack;Preview Thumbnail&amp;rbrack; Simplified thumbnail not updated when an anchor is used
* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。

### 8.1.0

*（リリース：2022年6月7日*）概要： **ICCサポートのあるメジャーリリース、物理サイズデータに基づくマテリアルのスケーリング、新しいベイカー、スポイト機能の強化、その他のコンテンツの範囲**

**追加：**

* &amp;lbrack；カラーマネジメント&amp;rbrack; Adobe Color Engine付きICCプロファイルのサポートを追加(ACE)
* &amp;lbrack；カラーマネジメント&amp;rbrack; ICCの作業用カラースペースとして「Adobe 98 RGB」のサポートを追加
* &amp;lbrack；カラーマネジメント&amp;rbrack；設定ファイルを介してACE/ICC設定を許可
* &amp;lbrack；カラーマネジメント&amp;rbrack；従来のモードでカラーピッカーにリニアカラー値を入力できるようにする
* &amp;lbrack；カラーマネジメント&amp;rbrack; UI外でカラーを選択するために使用するカラープロファイルを指定します。
* &amp;lbrack；カラーマネジメント&amp;rbrack; ビューポートで最後に選択したディスプレイ値を記憶
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;Substance&amp;rbrack;カラーマネジメントでジェネレーター/フィルターを正しく動作させる
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;Substance&amp;rbrack；新しいカラースペースオーバーライドキーワード$workingおよび$standardsrgbの追加
* &amp;lbrack;物理サイズ&amp;rbrack;&amp;lbrack;エンジン&amp;rbrack; メッシュから物理サイズ情報を抽出
* &amp;lbrack;物理サイズ&amp;rbrack;&amp;lbrack;エンジン&amp;rbrack; 物理サイズ計算
* &amp;lbrack;物理サイズ&amp;rbrack; UIで物理サイズを使用するオプションを表示
* &amp;lbrack;物理サイズ&amp;rbrack; ビューポートにビジュアルヘルパーを追加する
* &amp;lbrack;ベイク処理&amp;rbrack; Heightベイカーを追加
* &amp;lbrack;ベイク処理&amp;rbrack; Bent normalsの追加ベイカー
* &amp;lbrack;ベイク処理&amp;rbrack；不透明度ベイカーを追加
* &amp;lbrack；スポイトツール&amp;rbrack;マウスの横に表示され、カラーが管理された新しいスポイトツールのプレビュー
* &amp;lbrack；スポイト&amp;rbrack;カラーピッカーパネルを再度開くと、最後の位置に再表示される(&amp;L)
* &amp;lbrack；スポイト&amp;rbrack; マテリアルピッカーの新しいアイコン
* &amp;lbrack；スポイト&amp;rbrack;カラーピッカーのチャンネルプレビューをカラー管理
* &amp;lbrack；スポイト&amp;rbrack;クリックして選択する機能をスポイトに追加
* &amp;lbrack；スポイト&amp;rbrack; マテリアルピッカーが非アクティブチャンネルをアクティブにしません
* &amp;lbrack；スポイト&amp;rbrack; ショートカットでスポイトを使用できるようにする
* &amp;lbrack；スポイト機能&amp;rbrack；スポイト機能が適切なチャンネルを選択する(&amp;R)
* &amp;lbrack；スポイト&amp;rbrack;カラーピッカーモードに入ると、すべてのショートカットが無効になる
* &amp;lbrack；スポイト&amp;rbrack; 16進フィールドの自動選択を解除
* &amp;lbrack；スポイトツール&amp;rbrack; マテリアルピッカー使用時にパネルを閉じない
* &amp;lbrack；スポイト&amp;rbrack;チャンネルが選択できないときに新たに無効になった状態
* &amp;lbrack;Export&amp;rbrack; 正接属性をglTFエクスポートに追加
* Substance engineをv8.4にアップデートする
* 自動ラップ解除を0.9.0に更新する
* Qt 5.15.8にアップデートします。
* Python 3.9にアップデートする
* &amp;lbrack;シェーダー&amp;rbrack; Bent normalsシェーディングのサポートを追加
* &amp;lbrack;MacOS&amp;rbrack; 3DConnection SpaceMouseのサポート
* &amp;lbrack;Python&amp;rbrack; APIで使用されているPythonバージョンをドキュメント化する
* &amp;lbrack;Content&amp;rbrack; 105プリセットで6つの新しい3D ノイズを追加
* &amp;lbrack;Content&amp;rbrack; 20個の新しい経年劣化マップと2つの布地の折り目パターン
* &amp;lbrack;Content&amp;rbrack; 「メッシュマップ」書き出しプリセットを更新して新しいベイカーを使用
* &amp;lbrack;Content&amp;rbrack；ぼかし勾配とワープフィルターは、テクスチャセットの解像度に依存します
* &amp;lbrack;Content&amp;rbrack; 3つの新しいベイカーを使用するようにサンプルプロジェクトを更新

**修正済み：**

* &amp;lbrack;glTF&amp;rbrack；特殊文字を含むglTFを開けません
* &amp;lbrack;エンジン&amp;rbrack;異方性とSVTが無効なアーティファクト
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;M1&amp;rbrack; スマートマテリアルが正しく表示されない
* &amp;lbrack;メッシュ処理&amp;rbrack; Modelerからメッシュを読み込めません
* &amp;lbrack;UI&amp;rbrack;カラーマネジメントが有効になっている新規プロジェクトウィンドウの水平スクロールバー
* &amp;lbrack；カラーマネジメント&amp;rbrack；一部のOCIO構成でカラーピッカーに作業用スペース値が表示されない
* &amp;lbrack；カラーマネジメント&amp;rbrack; ビューポートのブラシプレビューがカラーマネジメントされない
* &amp;lbrack;SpaceMouse&amp;rbrack; Pivotがフォーカスの変更に伴ってすぐに更新されず、場合によってはモデルから外れる
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exported USD files has a wrong structure
* &amp;lbrack;USD&amp;rbrack；書き出し時のAmbient occlusion問題
* &amp;lbrack;Content&amp;rbrack; Preview Sphereサンプルプロジェクトに合わせてサムネールのメッシュを更新

**既知の問題：**

* 拡散パディングを使用してテクスチャを書き出すと黒いマップがレンダリングされる
* 正常/Ambient occlusionミキシングが壊れている
* まれにIray起動時にクラッシュが発生する(&amp;lbrack;MacOS&amp;rbrack;)
* &amp;lbrack;Preview Thumbnail&amp;rbrack; Simplified thumbnail not not updated when an anchor
* &amp;lbrack；カラーマネジメント&amp;rbrack; Linux上のACEを使用したHDRカラースペース変換では、カラーがクランプされます。

## バージョン7

### 7.4.3

*（リリース：2022年4月11日*）概要： **2D ビューポートで3Dconnection SpaceMouseをサポートしているバグ修正**

**追加：**

* &amp;lbrack;SpaceMouse&amp;rbrack; 2D ビューポートでの3DConnection SpaceMouseのサポート

**修正済み：**

* &amp;lbrack；カラーピッカー&amp;rbrack；は16進フィールドに書き込めません
* &amp;lbrack；カラーマネジメント&amp;rbrack; 投影モードで使用されているリソースがオーバーレイでカラーマネジメントされない
* &amp;lbrack；カラーマネジメント&amp;rbrack;エラーがログに記録されない
* &amp;lbrack;SpaceMouse&amp;rbrack;ユーザがSpaceMouseを持っていない場合、一般的なエラーメッセージを削除する
* &amp;lbrack;SpaceMouse&amp;rbrack;プロジェクトを読み込むとき、ピボットポイントは常に非表示になります
* &amp;lbrack;ベイカー&amp;rbrack; 「平均法線」設定はUV タイルプロジェクトには影響しません
* &amp;lbrack;UV タイル&amp;rbrack；別のタイルでメッシュを再読み込みすると、非アクティブなuvタイルオーバーレイが消える(&amp;rbrack;)
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Remote scripting is broken
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；複数のチャネルをAPIから照会できず、エラーが発生します
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; event when using ProjectEditionEntered
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;クラッシュがget_active_recipient()を呼び出した場合

**既知の問題：**

* 3Dconnection SpaceMouseはMacOSではサポートされていません
* &amp;lbrack;UI&amp;rbrack；新しいプロジェクトウィンドウに、カラーマネジメントが表示された水平スクロールバー(&amp;R)
* &amp;lbrack;Mac M1&amp;rbrack; スマートマテリアルが正しく表示されない

### 7.4.2

*（リリース：2022年3月8日*）概要： **3Dconnection SpaceMouseとカラーマネジメント(OCIO)の改善をサポートしているバグ修正**

**追加：**

* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack;ナビゲーション用の3D ビューポートでの3Dconnection SpaceMouseのサポート
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; 3D ビューポートのProおよびEnterprise SpaceMouseモデルの基本ショートカット/キー
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; 3D ビューポートの専用の回転中心アイコン
* &amp;lbrack；カラーマネジメント&amp;rbrack; OCIO configurationのロールを使用してデフォルト設定を変更
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーウィジェットのプロパティウィンドウをカラーマネジメント
* &amp;lbrack;Color Management&amp;rbrack; Colorマテリアルプレビューのプロパティウィンドウを管理
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーピッカーのカラーマネジメントスウォッチ
* &amp;lbrack；カラーマネジメント&amp;rbrack；標準のsRGBカラースペースを定義する設定を追加
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーピッカーのディスプレイセレクターリストで、OCIO configから標準sRGBカラースペースを追加
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラースペースオーバーライドメニューの改善
* &amp;lbrack；カラーマネジメント&amp;rbrack;ディスプレイ設定の環境マップカラースペースを上書きします
* &amp;lbrack；カラーマネジメント&amp;rbrack；現在のディスプレイに基づいてカラーピッカーグラデーションを描画
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーエディタのデフォルトでHDR 値をクランプ
* &amp;lbrack；カラーマネジメント&amp;rbrack;レガシーモードのフィルターにパススルー（カラースペースなし）を使用
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーエディタに表示されるグラデーションを&amp;lbrack;0 ～ 1&amp;rbrack；の範囲に一致するように制限する
* &amp;lbrack；カラーマネジメント&amp;rbrack;レガシーモードのカラーピッカーで表示セレクターを非表示
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーピッカーの16進数フィールドを常にsRGBカラースペースに作成する
* &amp;lbrack；カラーマネジメント&amp;rbrack;データチャンネルのカラーピッカー表示ドロップダウンを無効にする
* &amp;lbrack；最適化&amp;rbrack;ワープグリッドは、カバーされたUVタイルのみを再計算します。
* &amp;lbrack;Export&amp;rbrack; Sketchfab、USD、およびglTF用にUV タイルプロジェクトをエクスポートできるようにします
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack；トネマッピング関数の変更を許可

**修正済み：**

* &amp;lbrack;Sketchfab&amp;rbrack；既存のモデルを更新すると新しいモデルが作成される
* &amp;lbrack;Sketchfab&amp;rbrack；以前に更新されたモデルを検索する際のクラッシュ
* USDへの書き出し時のクラッシュ
* ジオメトリマスクで新しいシェーダーインスタンスを作成するとき、またはジオメトリが非表示のときにクラッシュが発生する。
* &amp;lbrack；読み込まれたリソースの種類を変更する際のImport Asset Window&amp;rbrack; クラッシュ
* 法線のメッシュマップは、レイヤースタックで使用すると反転します
* &amp;lbrack;Substance&amp;rbrack;ユーザーデータのブレンドモードが考慮されない
* &amp;lbrack；カラーマネジメント&amp;rbrack;ファイル名にカラースペースを含むビットマップは、UV タイルシーケンスとして読み込まれます
* &amp;lbrack；カラーマネジメント&amp;rbrack; グラフのカラーマネジメントされた出力が間違ったカラースペースにあります
* &amp;lbrack；カラーマネジメント&amp;rbrack；多角形の塗りつぶしツールが間違ったカラーを表示する
* &amp;lbrack;Color Management&amp;rbrack; ACE tonemapperがソロモードのチャンネルに適用される
* &amp;lbrack；カラーマネジメント&amp;rbrack;ツールプレビューの球体照明がカラーマネジメントされない
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack；変換されたマップは正しく変換されません
* &amp;lbrack；スクリプティング&amp;rbrack;&amp;lbrack;Python&amp;rbrack;&amp;lbrack；カラーマネジメント&amp;rbrack;テンプレートおよびOCIO環境変数を使用して作成されたプロジェクトはレガシーモードです
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；起動時にJavaScript evaluate関数を使用できない
* &amp;lbrack;3DAdobeオファー&amp;rbrack；デフォルトでサポートされていない言語で地域設定を使用すると、Painterを起動できません

**既知の問題：**

* 3Dconnection SpaceMouseはMacOSではサポートされていません
* &amp;lbrack;UI&amp;rbrack；新しいプロジェクトウィンドウに、カラーマネジメントが表示された水平スクロールバー(&amp;R)
* &amp;lbrack;ベイカー&amp;rbrack; 「平均法線」設定はUV タイルプロジェクトには影響しません
* &amp;lbrack;Mac M1&amp;rbrack; スマートマテリアルが正しく表示されない
* &amp;lbrack；カラーマネジメント&amp;rbrack; 投影モードで使用されているリソースがオーバーレイでカラーマネジメントされない
* &amp;lbrack；カラーピッカー&amp;rbrack；は16進フィールドに書き込めません

### 7.4.1

*（リリース：2021年12月14日*）概要： **カラーマネジメントの改善に関するバグの修正**

**追加：**

* &amp;lbrack；カラーマネジメント&amp;rbrack；書き出したファイル名にデータロールを使用
* &amp;lbrack;Color Management&amp;rbrack；新規プロジェクトおよびプロジェクト設定ウィンドウでOCIOが選択されている場合は、デフォルトでColor Managementセクションを展開します
* &amp;lbrack；カラーマネジメント&amp;rbrack；従来のモードでACEのトーンマッパーを追加
* &amp;lbrack；カラーマネジメント&amp;rbrack;デフォルト設定の調整
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack;データチャンネルのファイル名に$colorSpaceを入力
* &amp;lbrack;Export&amp;rbrack; UV タイルプロジェクトをStagerに書き出し
* &amp;lbrack；相互運用性&amp;rbrack;SteamおよびSubstanceエディションでは使用できません
* &amp;lbrack;Interoperability&amp;rbrack; UV タイルプロジェクトをStagerに送れるようにする

**修正済み：**

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;クラッシュ&amp;rbrack; PainterがCatalinaで開始しない
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;クラッシュ&amp;rbrack;ユーザチャンネルのデータタイプまたはカラーマネジメントで再生中にランダムにクラッシュする
* &amp;lbrack；カラーマネジメント&amp;rbrack;マスクディスプレイカラースペースの新規メニューでグレースケールとして使用されるリソース
* &amp;lbrack；カラーマネジメント&amp;rbrack；従来のモード+ソロビューでは、ビューポートのユーザーチャンネルが暗くなる
* &amp;lbrack；カラーマネジメント&amp;rbrack；環境マップはiRayで使用される場合は常に線形です。
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーピッカーが、レガシーモードのデータチャンネルに適切な値を選択しない
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーピッカーが、レガシーモードのSubstanceの内部で壊れている
* &amp;lbrack；カラーマネジメント&amp;rbrack;ドロップダウンメニューを使用しているときに、ビューポートのソロチャンネル表示を切り替えると、適切なカラースペースで表示される
* &amp;lbrack；カラーマネジメント&amp;rbrack；書き出しは、レガシーモードのカラーマネジメントされたユーザチャンネルに間違った変換を適用します
* マテリアル表示に戻すと、単独の表示マスクで作成したストロークが表示されない
* &amp;lbrack;Export&amp;rbrack；変換されたマップは、カラーマネジメントチャンネルとして書き出されません
* &amp;lbrack;テクスチャセット&amp;rbrack；名前を変更したユーザチャンネルで、元の名前のツールチップが表示されない
* &amp;lbrack;Steam&amp;rbrack; Steamでファイルの整合性をチェックする際にファイルが見つかりません

**既知の問題：**

* &amp;lbrack;Mac M1&amp;rbrack; スマートマテリアルが正しく表示されない

### 7.4.0

*（リリース：2021年11月24日*）概要： **メジャーリリース。 1stバージョンのカラーマネジメントの導入、2Dまたは3Dビューのドッキング解除、細長い島を避けるための自動ラップ解除の新しいオプション、Python APIおよび新しいコンテンツからのJavaScript関数の呼び出し**

**追加：**

* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーマネジメントOpenColorIO version 2のサポート
* &amp;lbrack；カラーマネジメント&amp;rbrack;プロジェクト設定にカラーマネジメント設定を追加
* &amp;lbrack；カラーマネジメント&amp;rbrack;プロジェクトを開いたときにカラーマネジメント設定が変更されるという警告ウィンドウ
* &amp;lbrack；カラーマネジメント&amp;rbrack；無効なOCIO設定ファイルが選択された場合にエラーメッセージを表示
* &amp;lbrack；カラーマネジメント&amp;rbrack; OCIO環境変数で設定を上書きできるようにします
* &amp;lbrack；カラーマネジメント&amp;rbrack;デフォルトでアプリケーションに統合された複数のOCIO設定
* &amp;lbrack；カラーマネジメント&amp;rbrack；読み込んだビットマップファイル名からカラースペース名を抽出
* &amp;lbrack；カラーマネジメント&amp;rbrack;プロパティウィンドウの設定から1つのカラースペースでカラースペースを上書きできるようにします
* &amp;lbrack；カラーマネジメント&amp;rbrack; テクスチャセット設定にカラーマネジメントオプションを追加
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack; 2Dビューと3Dビューを別々にカラーマネジメントできるようにします
* &amp;lbrack；カラーマネジメント&amp;rbrack;環境マップを作業用カラースペースに読み込んで変換
* &amp;lbrack；カラーマネジメント&amp;rbrack；現在のカラースペースでカラーピッカーとエディターを調整
* &amp;lbrack；カラーマネジメント&amp;rbrack；新しいドロップダウンメニューでビューポートのカラースペースの表示変形を選択できるようにします
* &amp;lbrack；カラーマネジメント&amp;rbrack; Irayレンダリング結果に表示変形を適用
* &amp;lbrack；カラーマネジメント&amp;rbrack；異なるカラースペースを持つテクスチャの書き出し
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;Python&amp;rbrack；環境変数(OCIO)から新しいプロジェクトにカラーマネジメント設定を適用する
* &amp;lbrack;ビューポート&amp;rbrack; 2Dまたは3D ビューポートのドッキングを解除できるようにします
* &amp;lbrack；自動ラップ解除&amp;rbrack；細長い島を避けるための新しいオプション
* &amp;lbrack；スクリプトPython&amp;rbrack; Python APIからJavaScript関数を呼び出す
* &amp;lbrack；新規プロジェクトウィンドウ&amp;rbrack；読み込まれたマップセクションを折りたたみ可能にする
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;ワープ設定のオプションとして法線を非表示にする
* &amp;lbrack;Content&amp;rbrack; 11個の新しい経年劣化マップ
* &amp;lbrack;Content&amp;rbrack; 8つの新しいツールプリセット （ジッパー、コードの引き締め、グリッター）
* &amp;lbrack;Content&amp;rbrack; 8つの新しいマテリアル (scar、pocket、...)
* &amp;lbrack;Content&amp;rbrack; 1つの新しいジェネレータ（収縮ワープを膨張）

**既知の問題：**

* &amp;lbrack;Mac M1&amp;rbrack; スマートマテリアルが正しく表示されない
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;クラッシュ&amp;rbrack;ユーザチャンネルのデータタイプまたはカラーマネジメントで再生中にランダムにクラッシュする
* &amp;lbrack；カラーマネジメント&amp;rbrack;カラーピッカーが、レガシーモードのデータチャンネルに適切な値を選択しない
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; ビューポートでカラーマネジメントがアクティブなときにレンダリングをEXRまたはTIFFで保存すると、常にリニアに保存される
* &amp;lbrack；カラーマネジメント&amp;rbrack;マスクでグレースケールとして使用されているリソースが間違ったカラースペースメニューを表示する
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Envマップは、Irayで使用される場合は常に線形になります。
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack；変換されたマップは、カラーマネージドチャンネルとして書き出されません
* &amp;lbrack；カラーマネジメント&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack；書き出しは、ユーザーチャンネルがカラーマネジメントされているかどうか、レガシーモードでないかどうかを無視します

### 7.3.1

*（リリース： 2021年11月24日*）概要： **バグ修正**

**追加：**

* &amp;lbrack;投影&amp;rbrack；拡大・縮小はオブジェクト空間でのみ動作します

**修正済み：**

* &amp;lbrack;Mac M1&amp;rbrack; マテリアルレイヤーが機能しない
* &amp;lbrack;Mac M1&amp;rbrack;&amp;lbrack;投影&amp;rbrack;ワープが機能しない
* マイクロディテールが正しく表示されない
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack;クラッシュ&amp;rbrack；以前のバージョンで作成されたレイヤーでワープモードに切り替え
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;フリップが、トランスフォームがワールド空間に設定されている場合に機能しない
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack; 「分割」オプションは、分割の実行後も選択されたままになります。
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack;UV&amp;rbrack; 投影のフリップ時に基点がリセットされる
* &amp;lbrack;Filter&amp;rbrack;パラメータの再読み込みまたは変更時に烘焙照明環境が変わる
* &amp;lbrack；相互運用性&amp;rbrack;SteamおよびSubstanceエディションでは使用できません
* &amp;lbrack；相互運用性&amp;rbrack; 「マーケットプレイスで3Dアセットを参照」ボタンをクリックすると、「Stockおよびマーケットプレイス」の3DタブでCCDが開きます。

**既知の問題：**

* &amp;lbrack;Mac M1&amp;rbrack; スマートマテリアルが正しく表示されない

### 7.3.0

*（リリース：2021年10月13日*）概要： **メジャーリリース。 これには、新しい3Dワープ投影、新しい円柱投影、カラーピッカーの機能向上、Python APIの新しい機能、バグ修正**&#x200B;が含まれています

**追加：**

* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack; 3Dワープを新しい投影モードとして表示
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack; ビューポートにドラッグ&amp;ドロップして、Alpha、テクスチャ、およびプロシージャにデカールモードを許可
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;デカールショートカットとともにワープ投影を使用(ALT)
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;&amp;lbrack；ツールバー&amp;rbrack;ワープ全体または頂点ごとに変形
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;&amp;lbrack；ツールバー&amp;rbrack;グリッドポイントを追加する横、横、縦の分割オプション
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;&amp;lbrack；ツールバー&amp;rbrack;リセット操作専用メニュー
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;&amp;lbrack；ツールバー&amp;rbrack;ポイントの移動時に正接を自動調整するオプション
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;&amp;lbrack；ツールバー&amp;rbrack;グリッド版専用メニュー（サイズ、リセット、カラー、ハンドルサイズ）
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack；新しいキーボードショートカットで全頂点ワープ編集モードに切り替え(SHIFT+V)
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack; Click+Ctrlを使用すると、サーフェスツールと他のツールを切り替えることができます
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；円柱&amp;rbrack；円柱投影モードを表示
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ツールバー&amp;rbrack;グループマニピュレーター設定（サイズ、グリッドステップ、角度ステップ）
* &amp;lbrack；カラーピッカー&amp;rbrack；新規カラーピッカーUI
* &amp;lbrack；カラーピッカー&amp;rbrack;カラーピッカーウィジェットでsRGB値を使用
* &amp;lbrack；カラーピッカー&amp;rbrack;カラースウォッチの保存と削除を許可
* &amp;lbrack；カラーピッカー&amp;rbrack;カラースロットおよび標準スロットからアクセス可能なスポイト
* &amp;lbrack；カラーピッカー&amp;rbrack; 0 ～ 255の値の間でダイナミックカラーを編集できるようにします
* &amp;lbrack；カラーピッカー&amp;rbrack; HSV/RGBステートをアプリ全体で共通にする
* &amp;lbrack;Color Picker&amp;rbrack; Color Pickerウィンドウがセミパーシステントです
* &amp;lbrack；カラーピッカー&amp;rbrack; Escキーを押すとカラーピッカーウィンドウが閉じる
* UIの操作とペイント中のパフォーマンスが向上しました
* &amp;lbrack;エンジン&amp;rbrack；新しいSubstanceエンジンバージョン(8.3.0)に更新する
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；現在のプロジェクトのメッシュを再ロードできるようにします
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack;プロジェクト内のリソースの更新を許可
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; UV タイルの解決の設定と照会を許可する
* &amp;lbrack；相互運用性&amp;rbrack;SteamおよびSubstanceエディションでは使用できません
* &amp;lbrack；相互運用性&amp;rbrack; Bridgeから複数のリソースを受信

**修正済み：**

* カラーピッカーに適切なカラーが表示されない
* &amp;lbrack;ベイク処理&amp;rbrack; テクスチャセットリストが正しく並べられていない
* &amp;lbrack;FBX import&amp;rbrack; 3ds Max groupピボット変換は考慮されません
* &amp;lbrack；破損したSBSARの読み込みを伴うSubstance engine&amp;rbrack; クラッシュ
* 異なる言語の&amp;lbrack;MacOS&amp;rbrack;プロジェクト設定オプションが存在しません
* 自動保存により、長時間プロセス中にPainterがフリーズすることがある

**既知の問題：**

* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack; 「分割」オプションは、分割の実行後も選択されたままになります。
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;フリップが、トランスフォームがワールド空間に設定されている場合に機能しない
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack；ワープ&amp;rbrack;パッチ間のアーティファクトライン（稀に）
* &amp;lbrack;投影&amp;rbrack;&amp;lbrack;UV&amp;rbrack; 投影のフリップ時に基点がリセットされる
* &amp;lbrack;Mac M1&amp;rbrack; スマートマテリアルが正しく表示されない
* &amp;lbrack;M1&amp;rbrack;&amp;lbrack;Regression&amp;rbrack;マテリアルレイヤーが機能しない

### 7.2.3

*（リリース：2021年8月24日*）概要： **マイナーリリース、バグ修正**

**追加：**

* &amp;lbrack；ライブラリ&amp;rbrack；不要なファイルがクロールされないようにする方法を追加

**修正済み：**

* &amp;lbrack;Win&amp;rbrack;マルチスクリーンおよびスリープの問題
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;クラッシュ&amp;rbrack;エフェクト使用時のシェーダーの切り替え
* &amp;lbrack;ビューポート&amp;rbrack;フルプレビューモードでアルファなしのブラシカーソルが表示されなくなる
* &amp;lbrack;UI&amp;rbrack；角度ウィジェットが間違った方向に曲がる。
* &amp;lbrack;レイヤースタック&amp;rbrack；多くのサブフォルダは非常に長いフリーズを作成します
* &amp;lbrack;Iray&amp;rbrack; IrayとOpenGLの異なるビュー：動作していない場合は表示される
* &amp;lbrack;Iray&amp;rbrack；屈折インデックスが考慮されず、mdlプロパティに表示されません。
* &amp;lbrack;JavaScript&amp;rbrack; ShowExportDialog()がtrueを返さない
* Adobe Stockからmtlを読み取れない

### 7.2.2

*（リリース：2021年7月27日*）概要： **マイナーリリース、バグ修正**

**追加：**

* AMDドライバー要件のバージョンのアップグレード

**修正済み：**

* &amp;lbrack;Mac M1&amp;rbrack; Wrong Memory detection
* &amp;lbrack;Export&amp;rbrack；非常に長いパスが正しく表示されません

**既知の問題：**

* &amp;lbrack;Content&amp;rbrack;サンプルの古いシェーダ

### 7.2.1

*（リリース：2021年7月2日*）概要： **マイナーリリース、ホットフィックス**

**追加：**

* &amp;lbrack;Interop&amp;rbrack; UV タイルプロジェクトのStagerへの送信がまだサポートされていないことを知らせるツールヒントを追加
* &amp;lbrack；プラグイン&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Livelinkアイコンの更新

**修正済み：**

* &amp;lbrack;Nvidia&amp;rbrack;ドライバーバージョンが30で始まる場合、古いバージョンと見なされます。
* &amp;lbrack；ライブラリ&amp;rbrack;アセットパネルの状態が、プロジェクトが開いていないと保存されない。
* &amp;lbrack；ライブラリ&amp;rbrack；新しい保存された検索で、古い保存された検索のキーワードが保持される
* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack;UVTiles&amp;rbrack; meshIDあたりのID マップも考慮に入れる
* &amp;lbrack;Export&amp;rbrack; gLTFファイルで頂点カラーを読み込まない
* &amp;lbrack;Iray&amp;rbrack；一部のツールチップが見つかりません
* &amp;lbrack;Interop&amp;rbrack; Stagerが検出されない場合に、Stagerに送信が常に無効になるとは限らない
* &amp;lbrack;Resource Updater&amp;rbrack; Photoshopブラシメーカーを更新できない
* &amp;lbrack;Content&amp;rbrack；繊維ガラスエッジ摩耗ジェネレータが壊れています

### 7.2.0

*（リリース：2021年6月23日*）概要： **メジャーリリース。アセットパネルのアップデート、新しいチャンネルおよびパラメーターへのアクセスを含む新しいシェーダー、UIの全体的な更新、非常に要求されたパフォーマンスの向上、より充実した言語サポートなど、さまざまな機能を提供します。**

**追加：**

* &amp;lbrack;Libraries&amp;rbrack; New Asset panel to replace the シェルフ
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack；新規アセットパネルレイアウト
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack;デフォルトのアセットパネルの向きとUIの変更
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ライブラリにリストビューオプションを導入
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack;アセットパネルの新しいブレッドクラムナビゲーション
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack；保存された検索を選択するときに「すべてのライブラリ」を選択
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack；すべてのフォルダが選択解除されている場合に「すべてのライブラリ」を選択
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; パーティクルブラシ用の新しいタグ
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack；アプリ全体で「ライブラリ」が「すべてのシェルフ」に置き換えられました
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack；空のフォルダを非表示にする
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack；既定のユーザーライブラリは、空であっても表示されます
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack;UI&amp;rbrack;アセットタイプアイコンを介した新しいフィルタリングメソッド
* &amp;lbrack；ライブラリ&amp;rbrack; ショートカット「CTRL」で複数のアセットタイプを選択
* &amp;lbrack；ライブラリ&amp;rbrack；アセットプレビューのメモリ予算を制御する新しい環境変数
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack；コンテンツ&amp;rbrack；新規環境マップ
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack；コンテンツ&amp;rbrack;&amp;lbrack;UI&amp;rbrack;デフォルトマテリアルのレンダリングディスプレイスメント
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack；コンテンツ&amp;rbrack;プレビュー生成用のデフォルトとしてAdobe Standard Material(ASM)シェーダーを設定
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack；コンテンツ&amp;rbrack;&amp;lbrack;ASM&amp;rbrack；新規ASM シェーダー用の新規プロジェクトテンプレート
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack；サムネイル&amp;rbrack；新しいStudio 6 環境マップを使用
* &amp;lbrack；ライブラリ&amp;rbrack;&amp;lbrack；サムネール&amp;rbrack;サムネールを生成する代わりにリソースに読み込む
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Thumbnail&amp;rbrack; ディスプレイスメントをサムネイル生成に追加
* &amp;lbrack;テクスチャセット設定&amp;rbrack;
* &amp;lbrack;テクスチャセット設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack；新しいHeightを通常の変換方式に表示
* &amp;lbrack;テクスチャセット設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack;チャネルのUI編成の再編集
* &amp;lbrack;テクスチャセット設定&amp;rbrack;ユーザチャンネル制限を16チャンネルに上げる
* &amp;lbrack;テクスチャセット設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack；現在選択されているシェーダーと互換性のあるチャンネルを示す
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack；新規Adobe Standard Materialシェーダー
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;異方性、クリアコート、表面化散乱、Specular edge color、光沢のサポートを追加
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;デフォルトチャンネルのカラー値を変更
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack；テンプレートAdobe DimensionをAdobe Substance 3D Stagerに更新
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; シェーダーおよびMDLパラメータ用にラベルとツールチップを追加
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; SSSがサポートされていない場合でも、2D ビューで散乱カラーを表示する
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack；新しいMDLでIray内のASM シェーダーをサポート
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack；従来のPBR spec gloss &amp; coatedの更新された表面化散乱
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack；コンテンツ&amp;rbrack;サンプルのデフォルトのSSSタイプを変更
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; ASM API用に追加されたドキュメント
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ASM&amp;rbrack；使用されていないチャンネルを無視するようにシェーダを最適化
* &amp;lbrack;シェーダー&amp;rbrack；新しいテクスチャセットチャンネルを表示
* &amp;lbrack;シェーダー&amp;rbrack; 表面化散乱の向上
* &amp;lbrack;シェーダー&amp;rbrack；一部のシェーダ用に新しいシェーダーパラメータを非表示にしました
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーパラメータの場合に表示する
* &amp;lbrack;Performance&amp;rbrack;
* &amp;lbrack；ライブラリ&amp;rbrack;リソースプレビューの読み込み時間と計算パフォーマンスの向上
* &amp;lbrack;エンジン&amp;rbrack;ペイントパフォーマンスの向上
* &amp;lbrack；自動ラップ解除&amp;rbrack;
* &amp;lbrack；自動ラップ解除&amp;rbrack; パッキングのパフォーマンス向上
* &amp;lbrack；自動ラップ解除&amp;rbrack;UV タイルワークフローと互換性のある自動ラップ解除
* &amp;lbrack;自動ラップ解除&amp;rbrack;メッシュ方向に従ってUVを配置する新しいオプション
* &amp;lbrack；その他&amp;rbrack;
* &amp;lbrack；設定&amp;rbrack;デフォルトのズーム方向を変更
* &amp;lbrack;UI&amp;rbrack; UIの全体的な更新
* &amp;lbrack;UI&amp;rbrack;ヘルプメニューの再作業
* &amp;lbrack;UI&amp;rbrack；反転アイコンの置換(&amp;R)
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack；プラグイン&amp;rbrack;プラグインdccリンクのアイコンを置換
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;AMD&amp;rbrack；最低限必要なバージョンとポップアップメッセージを更新
* &amp;lbrack;レイヤースタック&amp;rbrack；選択した空のフォルダ内に新規レイヤを作成
* Pythonドキュメントを更新する
* &amp;lbrack;Branding&amp;rbrack;
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack;アプリケーション名をAdobe Substance 3D Painterに更新
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack；更新されたスタンドアロンバージョンを「Substance版」に
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack；更新されたアプリケーションの実行可能ファイル名、インストールパス、パッケージ、およびアイコン
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Renamed default library and path
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Updated About Window
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack；更新されたようこそ画面
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack；年ベースのバージョン番号を削除
* &amp;lbrack;Localization&amp;rbrack;ドイツ語、フランス語、簡体字中国語の新規翻訳
* &amp;lbrack；相互運用性&amp;rbrack;SteamおよびSubstanceエディションでは使用できません
* &amp;lbrack；相互運用性&amp;rbrack;Adobeエコシステムとの相互運用性：Designer、Sampler、Stager、およびBridge
* &amp;lbrack;Interoperability&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Designerからアセットを受信および更新
* &amp;lbrack；相互運用性&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Samplerからアセットを受信
* &amp;lbrack；相互運用性&amp;rbrack;&amp;lbrack;UI&amp;rbrack;アセットをStagerに送信
* &amp;lbrack；相互運用性&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Adobe Bridgeで表示
* &amp;lbrack；相互運用性&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Adobe 3Dアセットにすばやくアクセスできるようにします
* &amp;lbrack；相互運用性&amp;rbrack; sbsarの新しい使用法タグ
* &amp;lbrack;Interoperability&amp;rbrack; Handle received asset types
* Adobe Substance 3D DesignerまたはAdobe Substance 3D Samplerから受け取った相互運用性&amp;rbrack;アセットは、ユーザーが選択したデフォルトのライブラリに保存されます。
* &amp;lbrack；相互運用性&amp;rbrack;&amp;lbrack;UI&amp;rbrack；左ツールバーに、StagerまたはPhotoshopに送信するための新しいアイコンを表示

**修正済み：**

* &amp;lbrack；タブレット&amp;rbrack；筆圧ペイント時のパフォーマンス低下
* スライダーコントロールを持つタブレットでの&amp;lbrack；タブレット&amp;rbrack；の問題
* &amp;lbrack;クラッシュ&amp;rbrack;テクスチャセットリストとエクスポーターの名前が一致しません
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack；ライブラリ&amp;rbrack;サブライブラリをダブルクリック
* &amp;lbrack；ライブラリ&amp;rbrack;ライブラリディレクトリのクロール時の問題
* &amp;lbrack；ライブラリ&amp;rbrack；強制プレビュー生成コマンドラインが予期したとおりに動作しない
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack; [ライト環境をベイク]フィルタは既定では黒です
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack;&amp;lbrack；書き出しメッシュ&amp;rbrack; Linux/MacOSで作成されたglTFを読み込めない
* &amp;lbrack;Linux&amp;rbrack;ファイルをアセットパネルにドラッグ&amp;ドロップすると、クラッシュが発生する場合がある
* &amp;lbrack;自動ラップ解除&amp;rbrack; 自動ラップ解除は、メッシュが再読み込み用に選択されていない場合でも使用可能です。
* &amp;lbrack;パーティクル&amp;rbrack;グラビティに対するパーティクルの動作が正しくない
* &amp;lbrack;レイヤースタック&amp;rbrack;レベルヒストグラムは、一部のチャンネルの輝度のみを使用できます
* &amp;lbrack；ジオメトリマスク&amp;rbrack;ジオメトリマスクの編集時にフォルダ上で右クリックメニューが機能しない
* &amp;lbrack;投影&amp;rbrack;球面投影法およびバイリニアフィルタリングとのシーム(&amp;r)
* &amp;lbrack;UV タイル&amp;rbrack;マスクをファイルにのみ書き出し、タイル0、0を書き出す
* &amp;lbrack；書き出しメッシュ&amp;rbrack; FBX メッシュの書き出しが空です
* &amp;lbrack;Iray&amp;rbrack；の法線マップが、レンダリング時に新規プロジェクトで考慮されない
* &amp;lbrack；保存&amp;rbrack；共有ドライブの保存問題
* &amp;lbrack;ベイク&amp;rbrack;パラメータを変更してメッシュを再ベイク処理すると、警告が表示される
* &amp;lbrack;ベイク処理&amp;rbrack;&amp;lbrack;Regression&amp;rbrack；高ポリゴンメッシュのグローバルバウンディングボックスにシーンの原点が含まれていない場合、正しくない結果が生成されます
* &amp;lbrack;Python&amp;rbrack;カスタムユーザーライブラリは考慮されません

**既知の問題：**

* &amp;lbrack；ライブラリ&amp;rbrack;プロジェクトが開かれていない場合、保存された検索は保存されません
* &amp;lbrack;NVIDIA&amp;rbrack;ドライバーが最新の場合でも、古いドライバーに関するメッセージを表示

### 7.1.1 (2021.1.1)

*（リリース：2021年3月23日*）概要：**マイナーリリース、カラーピッカーに16進数値を入力できるバグ修正**

**追加：**

* &amp;lbrack;Log&amp;rbrack；互換性のないAMD GPUドライバーについてユーザーに警告
* &amp;lbrack；カラーピッカー&amp;rbrack;16進数値の入力を許可

**修正済み：**

* &amp;lbrack;ベイカー&amp;rbrack;パフォーマンスの低下
* &amp;lbrack；ジオメトリマスク&amp;rbrack; Altでメッシュ名をクリックするとクラッシュが発生する場合がある
* &amp;lbrack;エンジン&amp;rbrack;ペイントが必要なときにビュー全体をリフレッシュしない(&amp;r)
* &amp;lbrack;レイヤースタック&amp;rbrack;シェーダーの変更後に選択範囲がスタックする
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack；カラーピッカー&amp;rbrack;カラーが選択したカラーと少し異なる
* &amp;lbrack；書き出し&amp;rbrack;PSDファイルフォーマットを使用すると、UV タイルごとに1ファイルが生成されない
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; alg.mapexport.getPathsExportDocumentMaps()が一部の値を返さない
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；無効化されたプラグインは、Painterを再度開いたときに再び有効になる

### 7.1.0 (2021.1.0)

*（リリース：2021年1月28日*）概要：**メジャーリリース、ジオメトリの一部を選択してペイントできる新しいジオメトリマスク、レイヤースタックでのエフェクトのコピー&amp;ペースト、UV タイルワークフローの改善、Iray、ベイカー、Substance engine、新しいコンテンツの更新**

**追加：**

* 新しいジオメトリマスクとジオメトリの選択した部分のペイント
* &amp;lbrack；ジオメトリマスク&amp;rbrack;ジオメトリの選択した部分をメッシュ名でペイント可能
* &amp;lbrack；ジオメトリマスク&amp;rbrack；両方のビューポートの長方形の選択
* &amp;lbrack；ジオメトリマスク&amp;rbrack；任意のレイヤー上の除外されたジオメトリを非表示/無視できるようにします
* &amp;lbrack；ジオメトリマスク&amp;rbrack;&amp;lbrack；プロパティ&amp;rbrack;クリック&amp;ドラッグによるチェックボックスのクイック選択
* &amp;lbrack；ジオメトリマスク&amp;rbrack;&amp;lbrack；プロパティ&amp;rbrack;&amp;lbrack;UI&amp;rbrack;プロパティウィンドウのドロップダウンですべてを含める/除外
* &amp;lbrack；ジオメトリマスク&amp;rbrack;&amp;lbrack；プロパティ&amp;rbrack; ALT+左クリックでリスト内の1つの項目をすばやく選択できるようにします
* &amp;lbrack；ジオメトリマスク&amp;rbrack;&amp;lbrack；プロパティ&amp;rbrack;プロパティウィンドウでメッシュ名/UV タイルをホバリングすると、ビューポートにオーバーレイされる
* &amp;lbrack；ジオメトリマスク&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack;ジオメトリマスクにコピー/ペーストオプションを追加
* &amp;lbrack；ジオメトリマスク&amp;rbrack；除外されたジオメトリを非表示/無視ボタンの新しいアイコン
* &amp;lbrack；ジオメトリマスク&amp;rbrack；除外されたジオメトリを非表示/無視するための新しいツールチップ
* &amp;lbrack；ジオメトリマスク&amp;rbrack;キーボードショートカット ALT+Hで「除外されたジオメトリを無視を非表示」ボタンのオン/オフを切り替え
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack; UV タイルおよび簡易モード用の新しい塗りつぶしレイヤー球プレビューサムネイル
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack;UV タイルマスクから簡単に出ることができます
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;テクスチャセットリスト&amp;rbrack; UV タイルごとに説明を与えることができます
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;テクスチャセット設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ドロップダウンメニューの2つの新しいセクションタイトルで、UV タイルの解像度を変更
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack; マテリアルをビューポートにドラッグするときにUV タイルマスクを終了
* &amp;lbrack;レイヤースタック&amp;rbrack;エフェクトのコピー/ペーストオプションを追加
* &amp;lbrack;レイヤースタック&amp;rbrack；あるライブラリから別のテクスチャセットへのエフェクトのコピー/ペーストを許可
* &amp;lbrack;レイヤースタック&amp;rbrack;エフェクトの複数選択を許可
* &amp;lbrack;レイヤースタック&amp;rbrack;レイヤーエフェクトのショートカットとしてコピー/ペーストオプションを追加
* &amp;lbrack;レイヤースタック&amp;rbrack;エフェクトを別のレイヤーにドラッグすると、マスクとコンテンツが自動的に切り替わる
* &amp;lbrack;レイヤースタック&amp;rbrack；別のレイヤーからマスクをペーストするときに自動的にマスクを作成
* &amp;lbrack;レイヤースタック&amp;rbrack;エフェクトのコンテキストの右クリックメニュー内にmove effectアクションを追加
* &amp;lbrack;レイヤースタック&amp;rbrack；あるレイヤーから別のレイヤーへエフェクトをドラッグ&amp;ドロップできるようにする
* &amp;lbrack;レイヤースタック&amp;rbrack；項目をフォルダにドラッグすると、その項目はフォルダの一番上に配置されます
* Irayをバージョン2020.1.0に更新します。
* &amp;lbrack;ベイカー&amp;rbrack; ベイカーをバージョン2.5.4にアップデート
* &amp;lbrack;ベイカー&amp;rbrack；個々のUV タイルをベイクの進行状況ウィンドウに表示
* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack;UI&amp;rbrack；現在のボタンを新しいテクスチャセットですばやくベイクできるようにする
* &amp;lbrack;ベイカー&amp;rbrack; Alt+左クリックでベイカーの1つを素早く選択できるようにする
* Substance engineをバージョン8.0.8にアップデートする
* &amp;lbrack;Substance engine&amp;rbrack；新しい.sbsarファイルでデフォルトカラーをサポート
* &amp;lbrack；自動ラップ解除&amp;rbrack;パフォーマンスの向上
* &amp;lbrack;Export&amp;rbrack；どのUV タイルの解像度がプロジェクトのデフォルトと異なるかを示すビジュアルフィードバックを追加
* &amp;lbrack;Export&amp;rbrack；書き出したシェーダー JSONファイルにシーンサイズ係数を追加
* &amp;lbrack；言語&amp;rbrack；日本語翻訳を追加
* &amp;lbrack;UI&amp;rbrack；内部依存のバージョン管理を含む「バージョン情報」ウィンドウを更新
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; シェルフリソースの管理を許可
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;プロジェクトがベイクおよび書き出し可能な状態になったことを知らせる
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; シェルフがディスク上のリソースのクロールを完了した時点を知らせる
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; テクスチャセットごとのUVタイルのリストのクエリを許可
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; シェルフリソースにカスタムプレビューを割り当てられるようにします
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;カスタムシェルフの管理を許可
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；各サブモジュールにメソッドインデックスを追加する
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack;ドキュメントの新しいスタイル
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Improvement of resources and シェルフドキュメント
* &amp;lbrack;Content&amp;rbrack;ステッチを作成する3つの新しいツールプリセット
* &amp;lbrack;シェルフ&amp;rbrack；新しいSubstance shareプラットフォームへの移行中に「Substance shareに書き出し」を一時的に削除

**修正済み：**

* 異なる解像度のモニターを使用するとクラッシュが発生する
* いくつかの珍しいプロジェクトとのSubstance engineのクラッシュ
* レイヤーを切り替える際に、「除外されたジオメトリを非表示/無視」でビューポートの更新が失敗する
* &amp;lbrack;2D ビュー&amp;rbrack; 2D ビューポートが一部のプロジェクトで見つからない
* &amp;lbrack;ベイク処理&amp;rbrack; 「メッシュ名で一致」はオブジェクトの一部を無視する
* &amp;lbrack;レイヤースタック&amp;rbrack;レイヤーエフェクトをクリックするとフォルダーが開く
* &amp;lbrack;Geometry Mask&amp;rbrack;UV タイルなしでメッシュを再読み込みしても、マスクにカウントされる。
* &amp;lbrack；ジオメトリマスク&amp;rbrack; ビューポートの右クリックメニューには、正しいツールがありません
* &amp;lbrack;エンジン&amp;rbrack；特定のプロジェクトで大幅に遅延する
* &amp;lbrack;Scripting&amp;rbrack; WindowsでのリモートJSON POSTリクエストによる高レイテンシー
* &amp;lbrack;Linux&amp;rbrack; Vramの量が、特定の統合GPUで正しく検出されない
* &amp;lbrack；自動ラップ解除&amp;rbrack; クラッシュまたは一部のプロジェクトでの長時間ラップ解除(&amp;R)

## バージョン6

### 6.2.2 (2020.2.2)

*（リリース：2020年9月28日*）概要： **マイナーリリース、Python APIの一部の関数に関するバグ修正**

**追加：**

* &amp;lbrack;Performance&amp;rbrack;カラーIDセレクションを使用する場合に、すべてのUV タイルを計算しない
* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack;UI&amp;rbrack；表示テクスチャセットの説明
* &amp;lbrack;ベイカー&amp;rbrack; 烘焙設定の保存を許可
* &amp;lbrack;ベイカー&amp;rbrack；すべてを折りたたむ/すべてのオプションを展開を「選択」タブに追加
* &amp;lbrack;テクスチャセットリスト&amp;rbrack；空の場合は説明を非表示
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;テクスチャセットリスト&amp;rbrack; UV タイルをクリックするとリストが展開/折りたたまれます
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;UI&amp;rbrack; テクスチャセットリストパネルを水平方向にサイズ変更できるようにする
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;UI&amp;rbrack；選択されていないテクスチャを使用した、UV タイルとテクスチャセットワークフローの両方の一貫したツールチップテキスト
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；書き出しプリセットを使用してテクスチャを書き出せる
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack;ドキュメントに変更ログを追加
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack；特定のスタックで使用可能なすべてのチャンネルを照会できるようにします
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack;コンソールUIの改善

**修正済み：**

* &amp;lbrack;AMD&amp;rbrack；古いバージョンのドライバーが正しく検出されない
* 異なるUV タイルレイアウトのメッシュを再読み込みするときにクラッシュが発生することがある
* 非常に重いメッシュでUDIMを使用しているパーティクルでクラッシュが発生する
* ディスプレイスメント情報を含むメッシュを書き出すときに&amp;lbrack;UV タイル&amp;rbrack;クラッシュが発生することがある
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;クラッシュ&amp;rbrack; psdフォーマットの2D ビューを書き出すとクラッシュが発生する場合がある
* プロジェクト作成時に画像をシーケンスとして読み込めません
* 無限ループに陥ったエンジン
* スナップモードのショートカットを変更するときに、常にスナップモードでカメラが回転する(&amp;lbrack;ショートカット&amp;rbrack;)
* オプションがオフの場合でも、メッシュは再読み込み時に常に自動ラップ解除されます
* &amp;lbrack;テクスチャセットリスト&amp;rbrack；説明テキストフィールドが編集中に完全には表示されない場合がある
* &amp;lbrack;テクスチャセットの表示/非表示を切り替えるドロップダウンメニューが完全には表示されない（&amp;rbrack; テクスチャセットリスト&amp;rbrack;）
* &amp;lbrack;テクスチャセットリスト&amp;rbrack；目のアイコンをクリックしても、「テクスチャセット名を編集」を入力することはできません。
* &amp;lbrack;テクスチャセット設定&amp;rbrack;チャンネルを削除すると、下のチャンネルも削除される
* &amp;lbrack;Export&amp;rbrack; Include allおよびReset allでは、UV タイルが考慮されません
* &amp;lbrack;ベイカー&amp;rbrack；選択されていないベイカーがベイクプロセス中に表示されます。
* 入力として使用されるベイク済みマップに対して、解決策の更新が考慮されない
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;UV タイル&amp;rbrack; 3D ビューポートマスクが選択された状態でフォルダの後にスマートマテリアルを追加すると、ビューポートがフリーズする
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack; ワイヤーフレームは、ペイントスルーモードの隠れたタイルでも表示される
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Sketchfab&amp;rbrack; 「プラス」サブスクリプションタイプに関する問題
* &amp;lbrack;Sketchfab&amp;rbrack;アカウントの切り替え後、「このアセットはプライベートです」チェックボックスが表示されない
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Content&amp;rbrack; &quot;Wiggly&quot; ブラシプリセットはパフォーマンスの問題につながる可能性があります
* &amp;lbrack；プラグインPhotoshop&amp;rbrack;ログ内のメッセージ：UV タイルワークフローと互換性がありません
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; PYTHONPATH env varは、アプリケーションの起動を妨げます
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Pythonドキュメント内のタイプミス

### 6.2.1 (2020.2.1)

*（リリース：2020年7月29日*）概要： **マイナーリリース、ホットフィックス**

**追加：**

* Substance変数「Environment_PAINTER_VRAM_BUDGET」を追加して、GPU VRam量を上書きします
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack；パフォーマンス&amp;rbrack;ポリゴンフィルツールを使用する場合に、すべてのUVタイルを計算しない

**修正済み：**

* &amp;lbrack;Iray&amp;rbrack;レンダリングを保存するとエラーが発生し、黒いイメージが表示される
* &amp;lbrack;Linux&amp;rbrack; CentOS 7.3のスプラッシュスクリーン後のクラッシュ
* &amp;lbrack;Linux&amp;rbrack; Vramの量が特定の設定で正しく検出されない
* &amp;lbrack;クラッシュ&amp;rbrack；重複したテクスチャセット名でプロジェクトを開く
* &amp;lbrack;エンジン&amp;rbrack;マスク変更時のキャッシュ無効化の問題
* &amp;lbrack;テクスチャセットリスト&amp;rbrack;テクスチャセットがディアクティベートされると、間違ったフォントが表示される

**既知の問題：**

* &amp;lbrack;テクスチャセットリスト&amp;rbrack；説明を非表示にできません
* &amp;lbrack;テクスチャセットリスト&amp;rbrack; UIの問題
* &amp;lbrack;Iray&amp;rbrack; PSDレンダリングが開かない
* &amp;lbrack；プラグインPhotoshop&amp;rbrack; UV タイルワークフローと互換性がありません

### 6.2.0 (2020.2.0)

*（リリース：2020年7月23日*）概要： **新しいUV タイルワークフロー、UV タイル間のペイント、パフォーマンスの向上を備えたメジャーリリース**

**追加：**

* UV タイル(UDIM)
* &amp;lbrack;UV タイル&amp;rbrack; UVタイル間のペイント
* &amp;lbrack;UV タイル&amp;rbrack; UV タイルの新しいワークフローと従来のワークフローを切り替えることができます
* &amp;lbrack;UV タイル&amp;rbrack;リソースとしてUDIM/UV タイル画像シーケンスをインポートする
* &amp;lbrack;UV タイル&amp;rbrack; [テクスチャセットリスト]ウィンドウにテクスチャセットごとのUV タイルのリストを追加
* &amp;lbrack;UV タイル&amp;rbrack; 「テクスチャセット設定」で複数のUV タイルの解像度を一度に編集できるようにする
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;2D ビュー&amp;rbrack; UV タイルをグリッドとして表示
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;2D ビュー&amp;rbrack; UV タイル情報の表示/非表示を切り替える新規ビューポートボタン
* &amp;lbrack;UV タイル&amp;rbrack; UV タイルプロジェクトのペイントツールをデフォルトでシングルチャンネルに切り替える
* &amp;lbrack;UV タイル&amp;rbrack;ペイント中にマスクされたUV タイルを無視するためのコンテキストツールバーの「新規」ボタン
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack;パフォーマンス向上のための新しいレイヤースタックアイコン
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack;ツールバーのペイントおよび塗りつぶしアイコンを改善
* &amp;lbrack;UV タイルマスク&amp;rbrack;&amp;lbrack;2D ビュー&amp;rbrack；複数のUV タイルを一度に含めるまたは除外できるようにします（左クリック、Ctrl +左クリック）
* &amp;lbrack;UV タイルマスク&amp;rbrack；含める新しいUV タイルマスク、新しいアイコンを含むレイヤーごとにタイルを除外
* &amp;lbrack;UV タイルマスク&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack；一部しか含まれていない場合に、UV タイルマスクアイコンにUV タイル数を表示
* &amp;lbrack;UV タイルマスク&amp;rbrack;&amp;lbrack;2D/3D ビュー&amp;rbrack;カーソルの下のUV タイルを表示するホバーエフェクトを追加
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack；特定のUV タイルの選択とベイクを許可
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack; テクスチャセット/UV タイルの選択オプションを追加
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack；右クリックメニューオプションを使用してテクスチャセット内のUV タイルを選択
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack;ドラッグによりテクスチャセット/UV タイルですばやく選択
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack; メッシュマップの「すべて」と「なし」ボタンを、より明示的な選択オプションで置き換える
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack;ベイクするテクスチャの数を表示
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack；特定のUV タイルの選択と書き出しを許可
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack;ドラッグしてUV タイルをすばやく選択
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack; UV タイルのドロップダウンメニューオプションを追加
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack；一部の書き出しプリセットがUV タイル(Adobe Dimension、Sketchfab、glTF、USD)で動作しない場合に使用不可にする
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack；コンテンツ&amp;rbrack；新しい$udimタグを使用するように書き出しプリセットを更新
* &amp;lbrack;UV アイランド&amp;rbrack;UV タイルが重なるメッシュを読み込む際のエラーレポートを改善
* &amp;lbrack;UV タイル&amp;rbrack; Iray内で互換性のあるUV タイル
* &amp;lbrack;UV タイル&amp;rbrack;&amp;lbrack；スクリプト&amp;rbrack; UV タイル書き出しドキュメントをPythonドキュメントに追加
* Performance
* &amp;lbrack;Performance&amp;rbrack；作業中に計算を一時停止するコンテキストツールバーの「新規」ボタン(SHIFT+ESC)
* &amp;lbrack；パフォーマンス&amp;rbrack; テクスチャセットキャッシュの計算を遅らせることでプロジェクトを開く時間を短縮
* &amp;lbrack;Performance&amp;rbrack;プロジェクトを開くときにメッシュマップの読み込みを待たない
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;2D/3D ビュー&amp;rbrack；未使用時にビューポート内のマスクチャンネルを計算しない
* &amp;lbrack;Performance&amp;rbrack; ビューポートに表示されているメッシュマップを読み込むときに、アプリケーションをブロックしない
* &amp;lbrack;Performance&amp;rbrack;プロジェクト保存時の増分保存速度を改善する
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack;デフォルトの拡張設定を変更して時間とプロジェクトサイズの節約を促進
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;ベイカー&amp;rbrack；特定のベイカーでグレースケールに切り替えて、時間とプロジェクトサイズの節約を促進
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack; エンジンのパフォーマンスを向上させて、テクスチャをより高速に書き出す
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack；多くのテクスチャセットを含む書き出しダイアログを開く際の応答性が向上します
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack;タブ「書き出しのリスト」に切り替えるときにパフォーマンスを改善
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Iray起動時間を短縮
* その他
* &amp;lbrack;ベイカー&amp;rbrack; テクスチャセットの選択オプションを追加
* シェーダーインスタンス管理を[テクスチャセットの設定]に移動する
* &amp;lbrack;2D/3D ビュー&amp;rbrack; ビューポートの下部に編集するマスクの種類を示すメッセージを追加
* &amp;lbrack;レイヤースタック&amp;rbrack；従来のサムネールと新しいサムネールを切り替えるための「設定」の「新規」オプション
* &amp;lbrack;レイヤースタック&amp;rbrack;サムネールの読み込み状況を示すビジュアルフィードバックを追加
* &amp;lbrack;Proj&amp;rbrack；画像シーケンスを読み込むための新しい投影モード「塗りつぶし（UVタイルごとに一致）」
* &amp;lbrack；プロジェクト&amp;rbrack；特定の場合に、投影モードを「塗りつぶし（UVタイルごとに一致）」に変更
* &amp;lbrack;Content&amp;rbrack; Optimize Charcoal ブラシプリセットによる処理速度の向上
* Irayをバージョン2020.0.0に更新します。
* &amp;lbrack;Export&amp;rbrack；何も選択されていない場合に「書き出しリスト」タブを無効にする
* 自動ラップ解除
* &amp;lbrack；自動ラップ解除&amp;rbrack；自動ラップ解除プロセスの成功率を向上させる
* &amp;lbrack；自動ラップ解除&amp;rbrack；速度と安定性を向上させるパラメーター配置の改善

**修正済み：**

* &amp;lbrack;Alembic&amp;rbrack; Facesetsはファイルのインポート時に無視されます。
* &amp;lbrack;Alembic&amp;rbrack；特定のファイルの読み込み時間が無制限
* &amp;lbrack;Import&amp;rbrack;ファイル拡張子のみが異なる場合、正しくないUDIM画像シーケンスが読み込まれる
* &amp;lbrack;クラッシュ&amp;rbrack；別のプロセスによってロックされているプロジェクトを開こうとすると、クラッシュが発生する
* &amp;lbrack;投影&amp;rbrack；重複したメッシュでトライプラナー投影を使用すると斑点が生じる(&amp;rbrack;)
* &amp;lbrack;Export&amp;rbrack; EmissiveチャンネルがUSDフォーマットで書き出されない
* &amp;lbrack;Content&amp;rbrack;スマートマテリアル「Charcoal」にはペイントストロークが含まれています

**既知の問題：**

* &amp;lbrack;テクスチャセットリスト&amp;rbrack；説明を非表示にできません
* &amp;lbrack;テクスチャセットリスト&amp;rbrack; UIの問題

### 6.1.3 (2020.1.3)

*（リリース：2020年6月16日*）概要： **バグ修正**

**追加：**

* &amp;lbrack;Export&amp;rbrack; シェーダーパラメーターjsonファイルにディスプレイスメント設定を追加

**修正済み：**

* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack；既存のチャンネルを消去して置き換えようとすると、エンジン&amp;rbrack; クラッシュが発生する
* &amp;lbrack;クラッシュ&amp;rbrack; マテリアルレイヤーでマスクをペイントした後にシェーダーを変更する
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;エンジン&amp;rbrack；一部の重いプロジェクトのクラッシュ
* &amp;lbrack;ベイカー&amp;rbrack；名前による一致が、zBrushから書き出したOBJで機能しない
* &amp;lbrack;ディスプレイスメント&amp;rbrack;&amp;lbrack;SVT&amp;rbrack; テクスチャが、ディスプレイスメントがオンのときにプロジェクトを開くと表示されない
* &amp;lbrack;Export&amp;rbrack；一部のテクスチャは均一なグレーで書き出されます
* &amp;lbrack;Export&amp;rbrack；無効テクスチャセットは、DimensionおよびSketchfab書き出しプリセット用に書き出さないでください
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript APIを使用してonProjectOpenedイベントのエクスポート設定にアクセスするときのJavaScript&amp;rbrack; クラッシュ
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; onExportFinished()がエクスポート後に呼び出されない

### 6.1.2 (2020.1.2)

*（リリース：2020年5月28日*）概要： **Substance engineおよびベイカーの更新に関するバグの修正**

**追加：**

* &amp;lbrack;ベイカー&amp;rbrack；最新バージョンに更新
* &amp;lbrack;ベイカー&amp;rbrack;Ambient occlusion、曲率、Thicknessベイカーでの新しいサンプリング方式
* Substance engineの最新バージョンに更新する
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack;プロジェクトリソースのResourceIDの作成を許可する
* &amp;lbrack；スクリプト&amp;rbrack;&amp;lbrack;Python&amp;rbrack;チャネル情報の照会を許可
* &amp;lbrack；スクリプティング&amp;rbrack;&amp;lbrack;Python&amp;rbrack; テクスチャ書き出しをシミュレートするdryrun関数とコールバック関数を追加

**修正済み：**

* &amp;lbrack;ベイカー&amp;rbrack；特定のケースで正接法線マップを使用してワールド空間法線ベイカーで法線が正しくない
* &amp;lbrack;ベイカー&amp;rbrack；高ポリゴンがない場合にOptixでAmbient occlusionをベイク中にエラーが発生する
* &amp;lbrack;動的ストローク&amp;rbrack；特定のテクスチャセットを読み込むときの遅延
* &amp;lbrack;Export&amp;rbrack；無効になっているテクスチャセットをUSD、glTFにエクスポートしないでください
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack；新しいベイカー設定を編集できない
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; alg.texturesets.addChannel()がエラーを返さない場合がある
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Typo in Javascript API documentation for setProjectExportOptions()
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack；常にすべてのテクスチャセットをエクスポート
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; sys.executableは、Substance Painterではなくpython.exeへのパスを返します
* テクスチャキャッシュがMac OSとWindows/Linux間で互換性がない
* &amp;lbrack;Livelink UE4&amp;rbrack；最後のマテリアルのみが、結合メッシュ内のすべてのテクスチャセットに使用されます。

**既知の問題：**

* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;Dimension&amp;rbrack;&amp;lbrack;Skecthfab&amp;rbrack；無効になっているテクスチャセットを書き出さないでください
* &amp;lbrack;クラッシュ&amp;rbrack;マテリアルレイヤーでマスクをペイントした後にシェーダーを変更

### 6.1.1 (2020.1.1)

*（リリース： 2020年5月5日*）概要： **ホットフィックス**

**追加：**

* &amp;lbrack;Export&amp;rbrack; TextureSetの状態のビジュアルフィードバックをオーバーライド

**修正済み：**

* &amp;lbrack；書き出し&amp;rbrack; エクスポーターウィンドウのサイズが特殊解像度モニターで大きすぎて、サイズ変更できない
* &amp;lbrack;Export&amp;rbrack; Options not saved after export
* &amp;lbrack;Export&amp;rbrack; クラッシュまたは「キャッシュから」書き出しプリセットで書き出しができない
* &amp;lbrack;Export&amp;rbrack；書き出しをキャンセルすると、予期しない空のマップが追加される
* &amp;lbrack；書き出し&amp;rbrack；仮想書き出しプリセット設定の修正
* &amp;lbrack;Python&amp;rbrack; PYTHONPATH env varが考慮されない
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Python経由で書き出しをキャンセルすると例外エラーが返される
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Export&amp;rbrack; export_project_format psdファイルテクスチャの結果が正しくない
* GPU レイトレーシングを含むLinuxでの&amp;lbrack;ベイカー&amp;rbrack;クラッシュ

**既知の問題：**

* &amp;lbrack;JavaScript&amp;rbrack；新しいベイカー設定を編集できません
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;Export&amp;rbrack；常にすべてのテクスチャセットをエクスポートする
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack；無効なテクスチャセットをエクスポートしないでください
* &amp;lbrack;クラッシュ&amp;rbrack;マテリアルレイヤーでマスクをペイントした後にシェーダーを変更

### 6.1.0 (2020.1.0)

*（リリース：2020年4月22日*）概要：**新しいテクスチャとメッシュのエクスポーター（ディスプレイスメントとテセレーション）、より多くのコントロールを使用したUVラップ解除の更新、新しいベイカー、新しいスクリプティングpython API、デカールの投影と新しいコンテンツのためのUXの向上**

**追加：**

* 新しいテクスチャとメッシュのエクスポーター
* &amp;lbrack；書き出し&amp;rbrack；新規エクスポーターインターフェイス
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; テクスチャセットごとに書き出すマップチャンネルの選択を許可
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack；書き出しタブ&amp;rbrack；すべてのテクスチャセットのテクスチャセットサイズを1回の操作で変更できるようにする
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; テクスチャセットごとに異なるテンプレートを許可（USD、glTF、Sketchfab、およびDimensionを除く）
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack；書き出しタブ&amp;rbrack;マップとテクスチャセットのクイック有効化と無効化
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack；書き出しタブ&amp;rbrack；書き出し解像度8192x8192が試験的ではなくなりました
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack；書き出しタブ&amp;rbrack;マップごとのファイルフォーマットとビット深度の変更を許可
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack；書き出しタブ&amp;rbrack;デフォルトのパラメータ値にリセットできます
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack；書き出しタブ&amp;rbrack；書き出しせずに設定を保存できるようにする
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;出力テンプレートタブ&amp;rbrack; 「設定」タブを「出力テンプレート」タブに名前変更
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;出力テンプレートタブ&amp;rbrack;プリセットマップごとにファイル形式とビット深度の定義を許可
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack；書き出しリストタブ&amp;rbrack；書き出しプロセスを要約して表示する新しいプレビュータブ
* &amp;lbrack；読み込み/書き出しメッシュ&amp;rbrack；読み込み/書き出し時間の最適化
* &amp;lbrack；書き出しメッシュ&amp;rbrack; FBXの書き出しメッシュ
* &amp;lbrack;メッシュの書き出し&amp;rbrack;ディスプレイスメントとテセレーションを含むメッシュの書き出し
* &amp;lbrack;メッシュを書き出し&amp;rbrack;&amp;lbrack;UI&amp;rbrack；通常の頂点を再計算するための新しい設定、三角形化を適用
* &amp;lbrack;メッシュを書き出し&amp;rbrack；自動ラップ解除によって生成された新しいUVを使用して元のメッシュトポロジを書き出す
* より多くのコントロールを備えた更新された自動ラップ解除
* &amp;lbrack;ラップ解除&amp;rbrack;&amp;lbrack;UI&amp;rbrack；新しいプロジェクトウィンドウで自動UVラップ解除を有効にする設定を追加
* &amp;lbrack;ラップ解除&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ラップ解除ステップ(シーム、ラップ解除、パッキング)を制御する新しいオプション
* &amp;lbrack;ラップ解除&amp;rbrack;&amp;lbrack;UI&amp;rbrack；既存のラップ解除シーム/ラップ解除/パッキングの保持を許可
* &amp;lbrack;ラップ解除&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ラップ解除ステップを完全に再計算する新しいオプション
* &amp;lbrack;ラップ解除&amp;rbrack;&amp;lbrack;UI&amp;rbrack；マージンサイズを制御する新しいオプション（なし、小、中、大）
* 新しいベイカー
* &amp;lbrack;ベイカー&amp;rbrack；古い曲率をメッシュの新しい曲率に置き換える
* &amp;lbrack;ベイカー&amp;rbrack; 「Ambient occlusion」ベイカーの背面を無視する名前で一致オプションを追加
* &amp;lbrack;ベイカー&amp;rbrack; 「Ambient occlusion」ベイカーの「グリッドを追加」オプション
* 新しいスクリプティングPython API(3.7.6)
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Python用の新しいスクリプトメニュー
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ヘルプメニューの新しいPythonドキュメント
* &amp;lbrack;Python&amp;rbrack; Substance Painter Pythonモジュールの表示: substance_painter, alg, display, project.setting, project, texturesets, ui
* &amp;lbrack;Python&amp;rbrack；新しい「substance_painter」Pythonモジュールを表示
* &amp;lbrack;Python&amp;rbrack；新しいPythonサブモジュールを表示: alg, display, log, project, resource, texturesets, ui
* &amp;lbrack;Python&amp;rbrack;プロジェクトの変更用リスナー
* &amp;lbrack;Python&amp;rbrack; Pythonドキュメントの新しい例
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;UI&amp;rbrack;プラグインメニューがJavaScriptに置き換えられました
* &amp;lbrack;ビューポート&amp;rbrack; シェルフから投影を「ドラッグ/ドロップ+ ALT」してデカールの作成を許可
* 新規コンテンツ
* &amp;lbrack;Content&amp;rbrack; 5 new decal マテリアル from Substance Source
* &amp;lbrack;Content&amp;rbrack; Maxwellレンダラー用に新しいプロジェクトテンプレートを追加し、プリセットを書き出す
* &amp;lbrack;Content&amp;rbrack; Keyshot 9書き出し用のプロジェクトテンプレートを追加
* &amp;lbrack;Content&amp;rbrack; Keyshot 9書き出しプリセットを更新してディスプレイスメントとemissiveをサポート
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;エクスポーター&amp;rbrack；すべての書き出しプリセットを最新バージョンのゲームエンジンおよびレンダラーに一致するように更新
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Format&amp;rbrack；新しいエクスポーターとディザリング設定を使用するように書き出しプリセットファイルを更新
* &amp;lbrack;Content&amp;rbrack; マテリアル(VRayMtl)をサポートする新しいテンプレートおよびシェーダ
* &amp;lbrack;レイヤースタック&amp;rbrack;ゴミ箱アイコンまたはキーボードショートカットを使用してレイヤーエフェクトを削除可能Delete
* プラグインSubstance Sourceを削除（「送信先」機能を含むランチャーを使用）
* &amp;lbrack;Windows&amp;rbrack;ハイエンドGPUでTDR警告を表示しない

**修正済み：**

* 新規プロジェクトファイルダイアログの翻訳の問題
* &amp;lbrack;ベイカー&amp;rbrack; 「前処理されたシーンファイルを保存」の設定が機能しなくなりました。
* &amp;lbrack;投影&amp;rbrack;投影が繰り返しUVを含むメッシュで機能しない
* &amp;lbrack；デカール&amp;rbrack；異なる投影モードを使用した場合の通常チャンネルの動作の違い
* &amp;lbrack；指先&amp;rbrack;&amp;lbrack;クローン&amp;rbrack;アーティファクトがマスクでペイント時に表示されることがある
* &amp;lbrack;エンジン&amp;rbrack；特定のレイヤーコンテンツを含むクラッシュ
* &amp;lbrack;エンジン&amp;rbrack；ペイント時にランダムなクラッシュが発生する場合がある
* &amp;lbrack；アンカーポイント&amp;rbrack；空のマスクへの参照は常に白を返す
* &amp;lbrack；書き出し&amp;rbrack;レイヤが特定のスタック設定で考慮されない
* &amp;lbrack;メッシュを書き出し&amp;rbrack；特殊文字を含むパスでは書き出しできません
* &amp;lbrack；書き出しメッシュ&amp;rbrack; LinuxまたはMacOSから書き出すとglTFファイルを読み取れない
* &amp;lbrack；読み込みメッシュ&amp;rbrack; DAE、PLY、またはglTFの再読み込みが意図したとおりに動作しない

**既知の問題：**

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack；新しいベイカー設定を編集できない
* GPU レイトレーシングを含むLinuxでの&amp;lbrack;ベイカー&amp;rbrack;クラッシュ
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack；無効なテクスチャセットをエクスポートしないでください
* &amp;lbrack;クラッシュ&amp;rbrack;マテリアルレイヤーでマスクをペイントした後にシェーダーを変更

## バージョン5

### 5.3.3 (2019.3.3)

*（リリース：2020年2月6日*）概要： **Iray 2019.3**&#x200B;へのアップグレードに関するバグ修正

**追加：**

* Iray 2019.3へのアップグレード
* &amp;lbrack;Log&amp;rbrack; Ryzen CPUの古いBIOSがベイク中にクラッシュすることを示す
* &amp;lbrack;ABR&amp;rbrack; ABRアルファをシェルフに抽出

**修正済み：**

* &amp;lbrack;ベイカー&amp;rbrack；高ポリゴンメッシュにUVがない場合、ベイク処理が失敗する(&amp;L)
* &amp;lbrack;Linux&amp;rbrack;カスタムマウスショートカットが保存されない
* &amp;lbrack；ブラシ&amp;rbrack;アウトラインがアルファシェイプとともに消える
* &amp;lbrack；タブレット&amp;rbrack;スライダーの移動時に間違って検出される
* &amp;lbrack;Shortcuts&amp;rbrack; 「Ctrl+Alt+MouseClick」でショートカットを設定できない
* &amp;lbrack;シェルフ&amp;rbrack; ペンタブレットを使用する際にリソースのツールチップが表示されない
* &amp;lbrack;2D ビュー&amp;rbrack;&amp;lbrack；書き出し&amp;rbrack; 2D ビュープリセットで通常の情報が考慮されない
* 特定のブラシを使用してアラインメントでペイントするとフリーズする
* フィルターの下にペイントすると、進行中のストロークにアーティファクトが生じる
* &amp;lbrack;ビューポート&amp;rbrack; メッシュを再読み込みした後、ビューポートに間違ったテクスチャキャッシュが表示される
* &amp;lbrack;Photoshopに書き出した後に保存時にクラッシュ&amp;rbrack;エラーが発生する
* &amp;lbrack；リソース&amp;rbrack; クラッシュをインポートする際のプレフィックスに特殊シンボルを書き込む
* &amp;lbrack;クラッシュ&amp;rbrack;アンカーポイントプロパティで参照をクリック
* &amp;lbrack；アンカーポイントとリファレンスの間にフィルターがある場合に、アンカーポイント&amp;rbrack;チャンネルが更新されない
* ヘルプメニューのIray URLリンクが機能しない

**既知の問題：**

* &amp;lbrack;ラップ解除&amp;rbrack；高ポリゴンメッシュの処理には時間がかかる場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；まったく同じ座標の頂点がマージされます。
* &amp;lbrack;ラップ解除&amp;rbrack; UV生成が一部のメッシュパーツで失敗することがある（まれに）。
* &amp;lbrack;ラップ解除&amp;rbrack; 1回のUV アイランドで不均一または高度に歪んだテキセル比が発生する場合がある(&amp;lbrack;)
* &amp;lbrack;ラップ解除&amp;rbrack;テクスチャセット間の不均等なテキセル比
* 生成された&amp;lbrack;ラップ解除&amp;rbrack;UV アイランドは非常に長くなり、UV空間に収まらない場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；縮退面またはエッジが小さいかエッジが重なっている三角形以外のメッシュ面では、UVがラップ解除されないことがある

### 5.3.2 (2019.3.2)

*（リリース：2020年1月21日*）概要： **バグ修正**

**修正済み：**

* ソロチャンネルモードで保存されたプロジェクトを開くと、メッシュが表示されない
* コピーツールを使用してレイヤーでペイントすると、ビューポートが更新されない場合がある

**既知の問題：**

* &amp;lbrack;ベイカー&amp;rbrack; Ryzen CPUのマルチスレッドに関連するクラッシュ
* &amp;lbrack;ラップ解除&amp;rbrack；高ポリゴンメッシュの処理には時間がかかる場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；まったく同じ座標の頂点がマージされます。
* &amp;lbrack;ラップ解除&amp;rbrack; UV生成が一部のメッシュパーツで失敗することがある（まれに）。
* &amp;lbrack;ラップ解除&amp;rbrack; 1回のUV アイランドで不均一または高度に歪んだテキセル比が発生する場合がある(&amp;lbrack;)
* &amp;lbrack;ラップ解除&amp;rbrack;テクスチャセット間の不均等なテキセル比
* 生成された&amp;lbrack;ラップ解除&amp;rbrack;UV アイランドは非常に長くなり、UV空間に収まらない場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；縮退面またはエッジが小さいかエッジが重なっている三角形以外のメッシュ面では、UVがラップ解除されないことがある

### 5.3.1 (2019.3.1)

*（リリース：2019年12月20日*）概要： **ホットフィックス**

**修正済み：**

* 特定のUV 投影を持つメッシュで作業する場合のクラッシュ
* Photoshopプリセットの切り替え時に&amp;lbrack;ABR&amp;rbrack; クラッシュが発生する
* &amp;lbrack;Linux&amp;rbrack;libGLXの依存性の問題により、CentOS 7.4でSubstance Painterを開始できません
* &amp;lbrack；ファイル/クリーンアップを使用した後にベイクする際のベイカー&amp;rbrack;クラッシュ
* &amp;lbrack;ベイカー&amp;rbrack;ベイク処理の進行状況ダイアログがキャンセル後にフリーズする
* &amp;lbrack;ベイカー&amp;rbrack; テクスチャの書き出し後にメッシュをベイクできない
* &amp;lbrack;ベイカー&amp;rbrack; 「名前で一致」を使用すると黒いメッシュマップが表示される
* &amp;lbrack;ベイカー&amp;rbrack;ケージが考慮されない
* &amp;lbrack;シェルフ&amp;rbrack; PSDファイルを読み込むと画像が破損する
* &amp;lbrack;Sample&amp;rbrack; &quot;Mat&quot;サンプルプロジェクトのカメラが壊れていたり、書き出しプリセットが正しくない

**既知の問題：**

* &amp;lbrack;ベイカー&amp;rbrack; Ryzen CPUのマルチスレッドに関連するクラッシュ
* &amp;lbrack;ラップ解除&amp;rbrack；高ポリゴンメッシュの処理には時間がかかる場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；まったく同じ座標の頂点がマージされます。
* &amp;lbrack;ラップ解除&amp;rbrack; UV生成が一部のメッシュパーツで失敗することがある（まれに）。
* &amp;lbrack;ラップ解除&amp;rbrack; 1回のUV アイランドで不均一または高度に歪んだテキセル比が発生する場合がある(&amp;lbrack;)
* &amp;lbrack;ラップ解除&amp;rbrack;テクスチャセット間の不均等なテキセル比
* 生成された&amp;lbrack;ラップ解除&amp;rbrack;UV アイランドは非常に長くなり、UV空間に収まらない場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；縮退面またはエッジが小さいかエッジが重なっている三角形以外のメッシュ面では、UVがラップ解除されないことがある

### 5.3.0 (2019.3.0)

*（リリース：2019年12月17日*）概要： **手描きユーザーエクスペリエンスの向上、タブレットの操作、ベータ版(0.3.0)での自動ラップ解除、手描きのための多様な新コンテンツを備えたメジャーリリース**

**追加：**

* 0.3.0バージョンをラップ解除して自動UVをSubstance Painterに統合
* &amp;lbrack;UVのラップ解除&amp;rbrack; UVが存在しない、またはUVの一部が存在しない場合に、Substance PainterでUVを自動的にラップ解除
* &amp;lbrack;ラップ解除&amp;rbrack；アクティブ化および非アクティブ化のための1つのグローバル設定
* &amp;lbrack;ラップ解除&amp;rbrack;バージョンがログファイルに報告されました
* &amp;lbrack;ラップ解除&amp;rbrack;&amp;lbrack;UI&amp;rbrack; UVラップ解除の進行状況を示す
* &amp;lbrack;UI&amp;rbrack;ブラシのプレビューを選択するためのコンテキストツールバーの新しい設定：フルプレビュー、ブラシのアウトライン、十字
* &amp;lbrack;Tool&amp;rbrack;アルファセクションの新しい高度な描画モード：通常に加えて明るくする（最大）
* &amp;lbrack;レイヤースタック&amp;rbrack;アルファまたはマスクのレイヤーごとのガンマ補正オプション（右クリックメニュー）
* &amp;lbrack;レイヤースタック&amp;rbrack;&amp;lbrack;UI&amp;rbrack;レイヤーアルファがガンマ補正されたときに「i」アイコンを追加
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;Tool&amp;rbrack;サイズと流量の最小圧力を表示
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;UI&amp;rbrack；曲線の圧力を選択するためのコンテキストツールバーの新しい設定：線形、イージーイン、イージーインアウト
* &amp;lbrack；タブレット&amp;rbrack;&amp;lbrack;UX&amp;rbrack；追加Ctrl+Alt+クリックしてスクロール
* ブラシプリセットの読み込み（ABR形式）
* &amp;lbrack;ABR&amp;rbrack;サポートシェイプパラメータ
* &amp;lbrack;ABR&amp;rbrack;シェイプダイナミクスパラメータをサポート
* &amp;lbrack;ABR&amp;rbrack; Support Transfer parameters
* &amp;lbrack;ABR&amp;rbrack;サポートスキャッタリングパラメータ
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;動的ストローク&amp;rbrack;サポート丸みと反転
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack;フィルタエディタでブラシフォルダ構造を表示
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack;サムネールにPhotoshopアイコンを追加
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack;サポートされていないパラメータのリストをABR詳細サムネイルに追加
* &amp;lbrack；ツール&amp;rbrack;&amp;lbrack;動的ストローク&amp;rbrack；生成するランダムシードの数を制御する新しいダイナミックストローク設定
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;UI&amp;rbrack;スキャッタリングジッターに新しい分布および軸設定を追加
* &amp;lbrack;ショートカット&amp;rbrack; Ctrl+Shift+Bを追加してベイクウィンドウを開く
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Menu&amp;rbrack; 「編集」メニューにエントリを追加してベイク処理ウィンドウを開く
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Settings&amp;rbrack;ショートカットリストの改善アラインメント
* &amp;lbrack;UI&amp;rbrack；圧力コントロール（サイズと流量）アイコンをオン/オフボタンで置き換え
* &amp;lbrack;ビューポート&amp;rbrack; 2Dと3Dのビューポートを別々にフォーカスできるようにする
* QT 5.12.5にアップデートします。
* &amp;lbrack;UI&amp;rbrack; メッシュの読み込みの進行状況を示す
* &amp;lbrack;Substance&amp;rbrack;スライダで非クランプおよびソフトレンジのサポートを追加
* &amp;lbrack;Substance&amp;rbrack;Substanceパラメーターの精度を最大6桁まで増やす
* &amp;lbrack;Substance&amp;rbrack;パラメータで定義されたステップを考慮する
* &amp;lbrack;Substance&amp;rbrack; userdataの条件をサポートして動的なストローク生成を最適化する
* &amp;lbrack;Substance&amp;rbrack; userdataを介してすべてのチャンネルのマスクとしてグラフ出力を指定できるようにする
* &amp;lbrack;Content&amp;rbrack; ディスプレイスメントフレンドリのトポロジ、新しいID マップ、および新しいカメラを使用して「Mat」サンプルプロジェクトを更新
* &amp;lbrack；コンテンツ&amp;rbrack; 3つの新しいフィルターの統合(MatFx):コミックブック、水彩画、石油ペイント（Emrecan Cubukcuの作品から着想を得た）
* &amp;lbrack;Content&amp;rbrack; Kyle T. Websterのパックの102 Photoshop ブラシプリセットを統合
* &amp;lbrack;Content&amp;rbrack; 18の新しいブラシプリセットを統合：ペイントローラ矢印、ペイントローラ警告テキスト、Charcoal Fineなど
* &amp;lbrack;Content&amp;rbrack; 9つの新しいアルファの統合：ブラシメーカーのペイントローラー、ブラシメーカーのPhotoshop、ブラシパターンなど
* &amp;lbrack;Content&amp;rbrack; 2つの新しいツールプリセットを統合： Gouache DenseとGouache Faded
* &amp;lbrack;Content&amp;rbrack; Integrate 1 new generator : UVチェッカー（ハイライトUV アイランドとシーム）
* &amp;lbrack;Content&amp;rbrack; 2つの新しい書き出しプリセットを統合： Keyshot 9+およびSpark AR Studio
* &amp;lbrack;Content&amp;rbrack; Integrate 1 new project template : Spark AR Studio (Facebook)

**修正済み：**

* &amp;lbrack；タブレット&amp;rbrack;スタイラスストロークの取り消し(Ctrl+Z)は、マウスストロークの取り消しよりも遅延が大きくなります。
* &amp;lbrack;Tablet&amp;rbrack；直線を描画するときに開始圧力と終了圧力が考慮されない
* &amp;lbrack;Tablet&amp;rbrack；直線を使用すると、最初のスタンプが2回描画される
* &amp;lbrack;Tablet&amp;rbrack; Huionタブレットショートカットのサポートを改善
* &amp;lbrack;Tablet&amp;rbrack; Huion ペンボタンのサポートを改善
* &amp;lbrack;Tablet&amp;rbrack;ブラシプレビューと描画されたスタンプの間のオフセット
* &amp;lbrack;Tablet&amp;rbrack; ペンを使用してブラシを変更するショートカットにより、まれにパフォーマンスが低下する
* &amp;lbrack；特定のレイヤーでペイントする際のタブレットの遅延(&amp;R)
* ビューポートを切り替える際に、まれにぼやけたテクスチャが生じることがあります
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack；画像入力が常に表示されるわけではない
* 「消去」を実行しても、プロジェクトに読み込まれたプリセットはシェルフから削除されません
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;Dynamic Stroke&amp;rbrack;スタンプ循環数を微調整する際のパフォーマンスの問題
* 3D/2D ビューポートモードでペイントしているときに発生する問題を更新する
* 非常に長いストロークを1つペイントすると、フリーズする場合があります
* &amp;lbrack;Tool&amp;rbrack；特定の動的ストロークでペイントする際のパフォーマンスの問題
* &amp;lbrack;UI&amp;rbrack;コンテキストツールバーでフォルダーを選択しても、ブラシのプロパティが表示される
* 軸値がリセットされない
* 浮動小数点値を含むEXR テクスチャの読み込みは完全に黒になる
* 分離するチャンネルをAltキーを押しながらクリックしても、フィルターとジェネレーターで機能しない
* &amp;lbrack；書き出し&amp;rbrack；書き出し時の特定のプロジェクトクラッシュ
* &amp;lbrack;Substance&amp;rbrack;パラメータがVisible Ifによって隠されている場合、ドロップダウンのデフォルト値が正しくない
* &amp;lbrack;シェーダー&amp;rbrack; マテリアルレイヤーで定義されたチャンネルが、UIで同じように並べ替えられない
* &amp;lbrack;シェルフ&amp;rbrack;プリセットメタデータがディスクに保存されない

**既知の問題：**

* &amp;lbrack;ラップ解除&amp;rbrack；高ポリゴンメッシュの処理には時間がかかる場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；まったく同じ座標の頂点がマージされます。
* &amp;lbrack;ラップ解除&amp;rbrack; UV生成が一部のメッシュパーツで失敗することがある（まれに）。
* &amp;lbrack;ラップ解除&amp;rbrack; 1回のUV アイランドで不均一または高度に歪んだテキセル比が発生する場合がある(&amp;lbrack;)
* &amp;lbrack;ラップ解除&amp;rbrack;テクスチャセット間の不均等なテキセル比
* 生成された&amp;lbrack;ラップ解除&amp;rbrack;UV アイランドは非常に長くなり、UV空間に収まらない場合があります。
* &amp;lbrack;ラップ解除&amp;rbrack；縮退面またはエッジが小さいかエッジが重なっている三角形以外のメッシュ面では、UVがラップ解除されないことがある
* Meetmatのサンプルで、読み込んだカメラに関していくつかの問題があります

### 5.2.3 (2019.2.3)

*（リリース：2019年10月23日*）概要： **バグ修正リリース**

**追加：**

* &amp;lbrack;テクスチャセットリスト&amp;rbrack;フォーカスモードの有効化/無効化を迅速に行う「追加」ボタン
* &amp;lbrack;Log&amp;rbrack; Windows 10のバージョン番号をログファイルに追加
* Substance engineの最新バージョンへのアップデート
* &amp;lbrack;MacOS&amp;rbrack；は、新しいMacOS Catalinaの配布要件に従うようにソフトウェアを公証しました

**修正済み：**

* &amp;lbrack;Plugin&amp;rbrack; Plugin Sourceが動作しない
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;シェーダー&amp;rbrack;Mac OS 10.14.5およびAMD:マテリアルレイヤリングが意図したとおりに機能しない

**既知の問題：**

* サブディビジョンを持つアルムビックファイルは読み込めません
* 一部のAlembicファイルを読み込む際のまれなクラッシュ
* Pascal GPUでDXRを使用してベイクすると、UIが一時的に応答しない

### 5.2.2 (2019.2.2)

*（リリース：2019年9月20日*）概要： **バグ修正リリース**

**修正済み：**

* スクリプトを使用してリソースを読み込むと、クラッシュが発生する場合がある
* &amp;lbrack;Plugin&amp;rbrack;ソースからマテリアルをダウンロードすると、クラッシュが発生する可能性があります

**既知の問題：**

* サブディビジョンを持つアルムビックファイルは読み込めません
* 一部のAlembicファイルを読み込む際のまれなクラッシュ
* Pascal GPUでDXRを使用してベイクすると、UIが一時的に応答しない

### 5.2.1 (2019.2.1)

*（リリース：2019年9月17日*）概要： **バグ修正リリース**

**修正済み：**

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;USD&amp;rbrack; MacOSから書き出したUSDZファイルを開くことができない
* &amp;lbrack;テクスチャセット&amp;rbrack; ALT修飾子を使用してテクスチャセットを分離できない
* &amp;lbrack;シェルフ&amp;rbrack;プリセット、スマートマテリアル、スマートマスクは、アプリケーションの終了時に常に変更されます。
* &amp;lbrack;レイヤースタック&amp;rbrack；別のエフェクトを削除した後にエフェクトを選択できない
* ツールプロパティパネル内でスライダーを使用すると、ちらつきが発生する
* プリセットをシェルフに書き出すときにクラッシュが発生する
* 空き容量が不足しているプリセットを書き出すとクラッシュが発生する
* 空き容量が不足しているプリセットを作成するとクラッシュが発生する

**既知の問題：**

* サブディビジョンを持つアルムビックファイルは読み込めません
* 一部のAlembicファイルを読み込む際のまれなクラッシュ
* Pascal GPUでDXRを使用してベイクすると、UIが一時的に応答しない

### 5.2.0 (2019.2.0)

*（リリース：2019年7月25日*）概要： **パフォーマンスおよび新しいプリビジュアライゼーションモードと新しいコンテンツに関するベイカーの更新を含むメジャーリリース**

**追加：**

* &amp;lbrack;ベイカー&amp;rbrack; DXRおよびOptiXでのGPU レイトレーシングのサポートを追加(Ambient occlusion、Thickness)
* &amp;lbrack;ベイカー&amp;rbrack; CPU レイトレーシングの最適化と高速化
* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack；表示モード&amp;rbrack;&amp;lbrack;UI&amp;rbrack; ビューポートの新しいベイク処理表示モード
* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack；環境設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack; GPU レイトレーシングを有効/無効にする新しいベイク処理オプション
* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack;UI&amp;rbrack;プログレスバーダイアログの再操作
* &amp;lbrack;ベイカー&amp;rbrack；警告およびエラーメッセージの改善
* &amp;lbrack;ベイカー&amp;rbrack; ベイク処理プロセスの迅速なキャンセルを許可
* &amp;lbrack;ベイカー&amp;rbrack; 「キャンセル」をクリックした後、烘焙ウィンドウを再度開く
* &amp;lbrack；プロジェクト&amp;rbrack;&amp;lbrack;UX&amp;rbrack；回転マニピュレーターのユーザビリティ向上
* &amp;lbrack;Settings&amp;rbrack; HDPI画面のビューポート解像度を下げて処理速度を改善するオプション
* &amp;lbrack；スクリプト&amp;rbrack; テクスチャセットの解像度を変更
* &amp;lbrack;Scripting&amp;rbrack；選択したテクスチャセットを取得
* &amp;lbrack;Scripting&amp;rbrack; テクスチャセットの選択を許可
* &amp;lbrack;Scripting&amp;rbrack;テクスチャセットの選択範囲が変更された場合に通知する関数
* &amp;lbrack;シェルフ&amp;rbrack；新しいスマートマテリアルを40個追加
* &amp;lbrack;シェルフ&amp;rbrack；新しいスマートマスクを20個追加

**修正済み：**

* &amp;lbrack;レイヤースタック&amp;rbrack;レイヤーを複数選択したときのUIのフリーズ
* &amp;lbrack;レイヤースタック&amp;rbrack；多数のレイヤーをグループ化すると、UIが通常より長くフリーズする
* &amp;lbrack;レイヤースタック&amp;rbrack;レイヤーとエフェクトを同時に選択できる場合があります
* ペイントツール内で使用するグラフが正しい解像度で生成されない
* &amp;lbrack;ベイカー&amp;rbrack; ベイカーが選択されていない場合、「すべてのテクスチャセットをベイク」ボタンが無効にならない
* &amp;lbrack;MacOS&amp;rbrack; テセレーションに関する警告メッセージをディアクティベート
* 投影ツールをマスクと一緒に使用すると、プレビューが表示されない
* ディスク容量が不足している状態でプロジェクトを保存しようとすると、クラッシュが発生してプロジェクトが破損する
* 空き容量が不足しているシェルフを介してディスク上のシェルフを読み込むときに、&amp;lbrack；リソース&amp;rbrack;クラッシュが発生します。
* &amp;lbrack；セッションプリセットの復元時のシェルフ&amp;rbrack; クラッシュ
* &amp;lbrack;シェルフ&amp;rbrack;スペースで終わる名前のプリセットを読み込むと、クラッシュが発生する
* &amp;lbrack;シェルフ&amp;rbrack；空のスペースで終わる接頭辞を持つリソースをインポートすると、クラッシュが発生する

**既知の問題：**

* サブディビジョンを持つアルムビックファイルは読み込めません
* 一部のAlembicファイルを読み込む際のまれなクラッシュ
* Pascal GPUでDXRを使用してベイクすると、UIが一時的に応答しない

### 5.1.3 (2019.1.3)

*（リリース：2019年7月1日*）概要： **2つの新機能を使用したバグ修正**

**追加：**

* コマンドラインでVRam予算を指定できます（例： —vram-budget 4096）
* &amp;lbrack;QML&amp;rbrack; QMLボタンとチェックボックスのwrapModeとelideプロパティを表示する

**修正済み：**

* 「パスに従う」が常に機能するわけではない
* シングルチャンネルスロットで使用されているSBSARでチャンネルマッピングが機能しない。
* &amp;lbrack;レイヤースタック&amp;rbrack；非表示レイヤーでスクロールするとパフォーマンスが低下する
* &amp;lbrack;TextureSet&amp;rbrack;マスク間でクリック時のクラッシュ
* &amp;lbrack;SVT&amp;rbrack; ディスプレイスメントが正しく表示されず、ちらつく場合がある
* &amp;lbrack;Alembic&amp;rbrack;頂点法線の代わりにポイント法線を使用したメッシュとのクラッシュ(&amp;R)
* &amp;lbrack;Alembic&amp;rbrack;&amp;lbrack；読み込み時にAlembicファイルがサポートされない場合、ログにエラーを報告&amp;rbrack;

**既知の問題：**

* サブディビジョンを持つアルムビックファイルは読み込めません
* 一部のAlembicファイルを読み込む際のまれなクラッシュ

### 5.1.2 (2019.1.2)

*（リリース：2019年5月21日*）概要： **ホットフィックス**

**修正済み：**

* 画像入力で2つのリソースを選択するとクラッシュが発生する

### 5.1.1 (2019.1.1)

*（リリース：2019年5月20日*）概要： **ホットフィックス**

**追加：**

* Substance Designer 2019.1の最終リリースでSubstance engineを最新バージョンにアップデートします。

**修正済み：**

* &amp;lbrack;Substance&amp;rbrack;入力画像が考慮されていない場合に表示する
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;エンジン&amp;rbrack; テクスチャセット解像度を変更すると、クラッシュが発生する場合がある
* &amp;lbrack;エンジン&amp;rbrack;ランダムな黒のテクスチャが表示される場合がある
* &amp;lbrack;レイヤースタック&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Shiftキーを押しながらマスクを切り替えると、複数のレイヤーを同時に選択できる
* &amp;lbrack;レイヤースタック&amp;rbrack；不透明度が、パススルー描画モードのペイント効果に影響しない
* &amp;lbrack;レイヤースタック&amp;rbrack；消しゴムブラシストロークで「通常」フィルター入力へのHeightが正しく更新されない
* &amp;lbrack;LayersStack&amp;rbrack; スマートマスクのドロップを取り消すときにクラッシュが発生する
* シャドウと時間のアンチエイリアスをアクティブにしてワイヤーフレームがちらつく
* AMDで重いメッシュを使用するとディスプレイスメントが遅くなる(&amp;lbrack;lbrack;)
* ファイルエクスプローラーを使用して一部のプロジェクトを開くと、&amp;lbrack;Windows&amp;rbrack;クラッシュが発生する
* &amp;lbrack；アンカーポイントを含むマスクを削除する際のヒストグラム(&amp;rbrack;)のクラッシュ（一部）
* まれに、プレビューの生成がクラッシュすることがある
* &amp;lbrack;クラッシュ&amp;rbrack；複数のクローンツールや指先ツールを使用すると、プロジェクトを再度開くことができない
* 保存後にマテリアルモードにメッシュが表示されない場合がある
* &amp;lbrack;Scripting&amp;rbrack; alg.mapexport.documentStructure()が間違ったフォルダー値を返す

**既知の問題：**

* テクスチャセット名をダブルクリックすると、名前の変更モードに入る前に選択されます

### 5.1.0 (2019.1.0)

*（リリース：2019年4月23日*）概要： **専用の新しいコンテンツ、リアルタイムとIrayのディスプレイスメントとテセレーション、比較マスク効果、円形の対称、平面と球面投影法を備えた動的なストローク**

**追加：**

* &amp;lbrack;Tool&amp;rbrack; Dynamic stroke:ブラシストロークと一緒にSubstanceバリエーションを追加
* &amp;lbrack；ダイナミックストローク&amp;rbrack；新しいスタンプインデックスパラメータをオプションで表示
* &amp;lbrack;Dynamic stroke&amp;rbrack; $timeパラメータを考慮
* &amp;lbrack；ダイナミックストローク&amp;rbrack;ストロークおよびスタンプごとに新しい$randomsedパラメータを生成
* &amp;lbrack；ダイナミックストローク&amp;rbrack；乱数からダイナミックストロークインデックスを開始
* &amp;lbrack;Dynamic stroke&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack；専用の新しいアイコンを使用して動的なストロークリソースを見つけるヘルプ
* リアルタイムビューポートでのディスプレイスメントとテセレーション
* Irayのディスプレイスメントとテセレーション
* &amp;lbrack;シェーダー設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ディスプレイスメントとテセレーションを制御するための新しいタブ
* &amp;lbrack;レイヤースタック&amp;rbrack；新しいCompareMaskエフェクト：2つのチャンネルを比較してマスクを生成
* &amp;lbrack;レイヤースタック&amp;rbrack;&amp;lbrack;UI&amp;rbrack；右クリックメニューの「Heightの組み合わせでマスクを追加」に新しいエントリを追加して、CompareMaskエフェクトを挿入
* &amp;lbrack;対称&amp;rbrack；新規対称モード：放射状ペイント
* &amp;lbrack;対称設定&amp;rbrack; 「設定」セクションと「ディスプレイ」セクションの両方を展開
* &amp;lbrack;対称設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ラジアルペイントのプレビュー
* 2つの新しい投影モード（平面と球）を表示します。
* &amp;lbrack；プロジェクト&amp;rbrack；すべての投影の新しいシェイプ切り抜きモード
* &amp;lbrack；投影&amp;rbrack;平面モードと新しいツール：サーフェスマニピュレーター
* &amp;lbrack；プロジェクト&amp;rbrack;&amp;lbrack;ショートカット&amp;rbrack;サーフェスツールのショートカット SHIFT+W
* &amp;lbrack;Proj&amp;rbrack; 深度カリングとバックフェースカリングを使用した平面投影マスク
* &amp;lbrack;マニピュレーター&amp;rbrack;3平面の3つの軸すべてで回転マニピュレーターを改善
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Altキーを押しながらチャネルをクリックすると、そのチャネルがフォーカスされます（その他すべてのチャネルが有効または無効になります）
* &amp;lbrack;エンジン&amp;rbrack; Substance engineの最新バージョンに更新する
* &amp;lbrack;テクスチャセット&amp;rbrack；複数選択と解像度の変更
* &amp;lbrack;テクスチャセット&amp;rbrack; テクスチャセットのクイックアクティベーションとアクティベーション解除(&amp;r)
* &amp;lbrack;テクスチャセット&amp;rbrack;ソロとすべてのオプションを組み合わせて新しいメニューを作成
* &amp;lbrack;テクスチャセット&amp;rbrack;&amp;lbrack;レイヤースタック&amp;rbrack;アクティベーションとアクティベーション解除の新しいアイコン
* &amp;lbrack;レイヤースタック&amp;rbrack;&amp;lbrack;UX&amp;rbrack；既に選択されているエフェクトの上にエフェクトを挿入
* &amp;lbrack;レイヤースタック&amp;rbrack;&amp;lbrack;UI&amp;rbrack;レイヤースタックビューの選択スタイルを再調整
* &amp;lbrack;レイヤースタック&amp;rbrack;インスタンス化されたレイヤーの描画モードが、デフォルトで通過モードになりました
* &amp;lbrack;Export&amp;rbrack; ディザリングをアクティブ化および非アクティブ化するオプション
* &amp;lbrack；プラグイン&amp;rbrack;スライダの精度モディファイヤをサポート(SHIFT)
* &amp;lbrack；プラグイン&amp;rbrack;&amp;lbrack;UI&amp;rbrack；自動保存の新しいアイコン
* &amp;lbrack;Scripting&amp;rbrack;フォルダの内容を一覧表示する
* &amp;lbrack；スクリプト&amp;rbrack;ファイルの削除を許可
* &amp;lbrack;Scripting&amp;rbrack；使用済みリソースを含むすべてのスタック情報を読み取る
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Dynamic stroke&amp;rbrack；新しいツールとブラシプリセット
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Dynamic stroke&amp;rbrack; Two new gradient: Gradient Hue and Gradient Builder
* &amp;lbrack;Content&amp;rbrack; 11の新しいフィルター：MatFxピーリングペイント、MatFx水滴など
* &amp;lbrack;Content&amp;rbrack; 7つの新しいジェネレータ：自動ステッチャー、UVランダムカラー、UVテクセル密度など
* &amp;lbrack;Content&amp;rbrack; 93 new alpha: new texts, arrows and various other shapes
* &amp;lbrack;Content&amp;rbrack; 2つの新しいプロシージャ：グラデーション色相、グラデーションビルダーなど
* &amp;lbrack;Content&amp;rbrack; 21 new Tool and Tools for Tools : Pebbles, Footprints, Spray and more
* &amp;lbrack;Content&amp;rbrack; 2 New HDRis: Canopus Ground and Autumn Forest
* &amp;lbrack;Content&amp;rbrack; シェルフでランダムなシードキュレーションを使用してコンテンツを更新
* &amp;lbrack;Content&amp;rbrack; シェルフにランダムシードパラメータを表示した新規アイコン

**修正済み：**

* &amp;lbrack；レイヤースタック&amp;rbrack; レイヤースタックが永遠にドラッグし続ける
* &amp;lbrack;Mac&amp;rbrack; 「Finderで表示」を選択すると、フリーズする場合がある
* シェーダーファイルを移動すると、カスタムUIで保存したスクリプト&amp;rbrack；設定が失われる
* &amp;lbrack;Scripting&amp;rbrack; APIバージョン番号が正しくないため、最新ではありません。
* &amp;lbrack;Effect&amp;rbrack;ヒストグラムコンテンツが正しく表示されない
* &amp;lbrack;Effect&amp;rbrack;ヒストグラムエフェクトが更新されない場合がある
* &amp;lbrack;シェルフ&amp;rbrack;ステッチがマテリアル「プラスチックファブリックピラミッド」に正しく位置合わせされていません

**既知の問題：**

* テクスチャセット名をダブルクリックすると、名前の変更モードに入る前に選択されます
* &amp;lbrack;レイヤースタック&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Shiftキーを押しながらマスクを切り替えると、複数のレイヤーを同時に選択できる

## バージョン4

### 4.3.3 (2018.3.3)

*（リリース：2019年3月7日*）概要： **bugfix**

**追加：**

* &amp;lbrack;Content&amp;rbrack；新しいプロジェクトテンプレートを統合：「PBR - Alphaブレンド」
* Linux動的ライブラリの検索順序が変更され、システムにインストールされているライブラリより前のインストールディレクトリ内のライブラリに優先順位が設定される

**修正済み：**

* 3D ビューポートのメッシュが消えることがある（Fキーを押してカメラをリセット）
* 新しいSketchfabライセンスタイプでSubstance PainterのSketchfabアップローダを更新する
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; glTFファイルで定義されている入力テクスチャモジュレーションを正しく処理しない
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack;グリッドがglTFのインポートで正しく表示されない場合がある
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack；不透明度がArkitで機能しない
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;USD&amp;rbrack; USDz書き出しクラッシュ（一部のケース）
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;USD&amp;rbrack；保存せずにUSDに書き出すとクラッシュになる
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack;テクスチャのタイリングモードが正しくない、メッシュのサブディビジョンモードとシェーダの出力タイプ
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack；一部のテクスチャセットのみを、すべてのジオメトリとともにスパース書き出し
* 壊れたインスタンスレイヤーを削除しようとすると、&amp;lbrack;Instance&amp;rbrack;クラッシュが発生します。
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;Export&amp;rbrack；選択したビット深度で書き出されないマップがあります
* &amp;lbrack;Linux&amp;rbrack;ライブラリlibtbb.so.2の問題

**既知の問題：**

* AMD VEGA GPUで計算がフリーズすることがある
* Windows OSでのショートカットに関するHuionタブレットの問題

### 4.3.2 (2018.3.2)

*（リリース：2019年1月24日*）概要： **新機能を含む修正プログラム（USDZ書き出しとビューポートのテクスチャフィルタリング）**

**追加：**

* &amp;lbrack;Export&amp;rbrack; USDZへのエクスポートを許可
* &amp;lbrack;ビューポート&amp;rbrack;ディスプレイ設定でテクスチャの画質を制御できるようにします
* &amp;lbrack;ビューポート&amp;rbrack; Added mip bias setting in Display Settings
* &amp;lbrack;ビューポート&amp;rbrack;ディスプレイ設定に異方性フィルタリングを追加
* &amp;lbrack；プラグイン&amp;rbrack; Substance Painter 2018のスタイルを使用するように公式プラグインを更新
* &amp;lbrack;License&amp;rbrack;デフォルトでユーザーフォルダーにライセンスをインストール

**修正済み：**

* 減圧に関連したクラッシュ
* ソロマテリアルでのTAAの追加
* シャドウ、TAA、アルファを含むノイズテストシェーダーとディザリング
* すべてのクラシックPBRシェーダのSpecular ディザリングを削除する
* 場合によってはシェーダー設定のクラッシュ
* OpenGLとIrayレンダリングの間で散布のアクティブ化が同期されない
* 指先ツールとクローンツールが、特定のメッシュで機能しなくなった
* 一部のテクスチャセットはIrayレンダリングに表示できません
* プロジェクトを閉じた後、名前を変更したテクスチャセットが保存されない
* ID マップにマテリアルをドラッグ&amp;ドロップすると、ワイヤーフレームが正常に動作しない
* &amp;lbrack;Scripting&amp;rbrack;プロジェクトの保存時にファイルパスの作成が強制されない
* &amp;lbrack;Scripting&amp;rbrack;コールバック「onProjectAboutToSave()」が機能しない
* バグ報告ウィンドウでフォーラムリンクが破損する

**既知の問題：**

* AMD VEGA GPUで計算がフリーズすることがある
* Windows OSでのショートカットに関するHuionタブレットの問題

### 4.3.1 (2018.3.1)

*（リリース：2018年12月6日*）概要： **ホットフィックス**

**追加：**

* &amp;lbrack;対称&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack; 2D ビューの対称ペイントが元に戻り、コピーブラシプレビューが修正されました

**修正済み：**

* &amp;lbrack；書き出し&amp;rbrack; 2D ビュー書き出しで黒いテクスチャが出力されることがある
* &amp;lbrack;Iray&amp;rbrack;マテリアルレイヤーをインスタンス化した後、Iray内の通常の情報が不正確になる
* 非正方形のテクスチャセットは、場合によってはクラッシュの原因になることがあります
* &amp;lbrack；取り消し&amp;rbrack；複数のCtrl+Zキーを使用すると、まれにランダムにクラッシュが発生することがあります
* &amp;lbrack;QML&amp;rbrack; AlgScrollViewは、場合によっては（バインドループ）、ログに警告を作成できます

**既知の問題：**

* AMD VEGA GPUで計算がフリーズすることがある
* Windows OSでのショートカットに関するHuionタブレットの問題
* アンチエイリアスとシャドウを同時にアクティブにすると、予期しない結果になることがあります

### 4.3.0 (2018.3.0)

*（リリース：2018年11月20日*）概要：**ビューポートのアップグレード、適切な2D ビュー書き出し、新しいUIヘルパー、強化された対称ツール、新しいコンテンツ、およびパフォーマンスの大幅な向上**

**追加：**

* &amp;lbrack；アンチエイリアス&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack; 3Dビューポート用の新しいテンポラルアンチエイリアシングフィルタリング（[表示設定]を使用）
* &amp;lbrack；書き出し&amp;rbrack; 2D ビューポートのコンテンツを1つのテクスチャとして書き出す
* &amp;lbrack；書き出し&amp;rbrack;&amp;lbrack;ディザリング&amp;rbrack；書き出し時にディザリングを表示
* &amp;lbrack;レイヤースタック&amp;rbrack;レイヤーとフォルダーのカラー
* &amp;lbrack;レイヤースタック&amp;rbrack；複数のレイヤーやエフェクトのクイック選択とクイック選択解除
* &amp;lbrack;レイヤースタック&amp;rbrack；上下キーとマウススクロールを使用した描画モードの簡単なナビゲーション
* &amp;lbrack；プロジェクト&amp;rbrack;&amp;lbrack;UI&amp;rbrack;3平面の3つの軸すべてに追加の回転マニピュレーター
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Shorcuts&amp;rbrack; – および+を使用して、マニピュレーターのサイズを変更します。
* &amp;lbrack;シェーダー&amp;rbrack; PBRでコーティングされたシェーダーのチャンネルを使用してコーティングレイヤーパラメーターを制御
* &amp;lbrack;Substance&amp;rbrack;フィルタおよびジェネレータに新しいメッシュベースのテクスチャ入力を表示
* &amp;lbrack;対称&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack;&amp;lbrack;UI&amp;rbrack;マニピュレーターを使用して対称オフセットを制御
* &amp;lbrack;対称&amp;rbrack;&amp;lbrack；コンテキストツールバー&amp;rbrack;&amp;lbrack;UI&amp;rbrack;オプション付きの新しい対称パネル
* &amp;lbrack;対称&amp;rbrack；新しい対称線の交点モード
* &amp;lbrack;対称&amp;rbrack；新規対称クローンカーソル
* &amp;lbrack;対称&amp;rbrack;&amp;lbrack；ショートカット&amp;rbrack; Qを非表示にし、-、+を使用してサイズを変更し、shiftを使用してスナップ
* &amp;lbrack;Log&amp;rbrack; テクスチャを書き出せない場合のエラーメッセージを改善
* &amp;lbrack;Scripting&amp;rbrack; Allow to change or update the resources in Display Settings
* &amp;lbrack;Scripting&amp;rbrack; テクスチャセットのチャンネルを作成または削除できるようにします
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shaders&amp;rbrack；専用のシェーダー （pbr-metal-rough-異方性角度）との異方性のサポートを追加
* &amp;lbrack;Content&amp;rbrack;プレビュー球を異方性と角度の変更で更新
* &amp;lbrack;Content&amp;rbrack；更新されたmatFx shutline
* &amp;lbrack;Content&amp;rbrack；新しいテクスチャリング.XYZシームレスな面スキャン
* &amp;lbrack;Content&amp;rbrack；新しい異方性プロシージャ
* &amp;lbrack;Content&amp;rbrack；新しいフィルタ：ベイク済み照明環境
* &amp;lbrack；コンテンツ&amp;rbrack；新規環境マップ: studio automotive neutral
* &amp;lbrack;Content&amp;rbrack；新規プロジェクトテンプレート： PBR - Anisotropy angle（異方性チャンネル付き）
* &amp;lbrack;Content&amp;rbrack；新規プロジェクトテンプレート： PBR - メタリックラフネスコーティング
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;エンジン&amp;rbrack;スパース仮想テクスチャ(SVT)
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack；環境設定&amp;rbrack;&amp;lbrack;UI&amp;rbrack; SVTハードウェアサポートアクセラレーションオプション
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Log&amp;rbrack；スパース仮想テクスチャリング機能（例：サイズディスク）の追加情報
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;UI&amp;rbrack;ディスク上のサイズがキャッシュに対して小さすぎる場合、起動時にメッセージウィンドウを表示
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Preferences&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Substance Painterグローバルキャッシュの場所
* &amp;lbrack;SVT&amp;rbrack;Substance Painterのキャッシュのパスを指定する新しい環境変数
* &amp;lbrack;SVT&amp;rbrack; SVTハードウェアサポートアクセラレーションを有効にする新しい環境変数
* &amp;lbrack;SVT&amp;rbrack;ハードウェアによる疎サポートの検出
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack；ハードウェア疎&amp;rbrack; Nvidia GPUの最小ドライバーバージョンを上げる
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack;&amp;lbrack;UI&amp;rbrack;プロジェクトを開くときにスパースバーチャルテクスチャリングでアーティファクトが存在する場合に警告を表示

**修正済み：**

* &amp;lbrack；カラーピッカー&amp;rbrack;カラーを選択しようとするとペイントカーソルが表示される
* レイヤーを一定の順序でクラッシュまたは選択解除すると、クラッシュになる場合があります
* マスク付きのレイヤーをインスタンスとしてペーストするとクラッシュが発生する
* &amp;lbrack;User Channel&amp;rbrack;&amp;lbrack;Regression&amp;rbrack; user channelの名前を変更する際のクラッシュ
* &amp;lbrack;User Channel&amp;rbrack；グレー表示されたブラシのプレビュー
* &amp;lbrack;Alembic&amp;rbrack；読み込み後、複数のマテリアルから1つのテクスチャセットのみ
* &amp;lbrack;エンジン&amp;rbrack；書き出されたテクスチャは、ブラシスタンプのビューポートと異なります。
* &amp;lbrack;エンジン&amp;rbrack;レベル効果で反転しても、テクスチャに完全には影響しない
* マテリアルピッカーが選択中にブラシストロークを適用する
* 解像度を128x128pxに切り替えると、クラッシュが発生する
* レイヤーを再ベイクまたはインスタンス化すると、メッシュマップリンクが正しく更新されない
* &amp;lbrack;Substance&amp;rbrack; UserData ColorSpaceが、入力として要求されたベイクメッシュ Normalで動作しない
* 複数のシェーダーインスタンスを使用する場合、MDLの関連付けが一致しません
* &amp;lbrack;対称&amp;rbrack;&amp;lbrack;塗りつぶしレイヤー&amp;rbrack;対称プレーンとそのマニピュレーターが塗りつぶしレイヤー内でアクティブ
* &amp;lbrack;ビューポート&amp;rbrack；変換の基点がクリック後に必ずしも更新されない
* &amp;lbrack;UI&amp;rbrack; HDPIモニターのアイコンの修正とプレースホルダーの削除

**既知の問題：**

* AMD VEGA GPUで計算がフリーズすることがある
* Windows OSでのショートカットに関するHuionタブレットの問題
* アンチエイリアスとシャドウを同時にアクティブにすると、予期しない結果になることがあります

### 4.2.3 (2018.2.3)

*（リリース：2018年9月25日）*

**修正済み：**

* &amp;lbrack;2D ビュー&amp;rbrack; 2D ビューが、新しいプロジェクトの作成時に一部のメッシュで壊れる
* &amp;lbrack;クラッシュ&amp;rbrack; UV 投影から3平面投影に切り替えるとクラッシュが発生する
* &amp;lbrack;RayCollider&amp;rbrack; 「RayCollider」による複数のクラッシュ
* &amp;lbrack;Tool&amp;rbrack;レイヤーを切り替えると、変更されたブラシプロパティが失われる
* 消しゴムに切り替えると、ブラシ設定がリセットされる

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ
* Windows OSでのショートカットに関するHuionタブレットの問題

### 4.2.2 (2018.2.2)

*（リリース：2018年9月11日*）概要： **コンテンツの更新、新しいスクリプト機能、および自動更新を無効にできるホットフィックス**

**追加：**

* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack;スキンシェルフプリセットを追加
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack; 19スキン法線を表面化散乱用のマテリアルに変換
* &amp;lbrack；スクリプト&amp;rbrack；開いているプロジェクトからプロジェクトテンプレートを作成
* &amp;lbrack;Scripting&amp;rbrack；開いているプロジェクトの書き出し設定を取得/設定する
* &amp;lbrack；更新&amp;rbrack；設定および環境変数の自動更新ポップアップを無効にできる
* &amp;lbrack；更新&amp;rbrack;メンテナンスの古いポップアップで次のバージョンまで表示されない

**修正済み：**

* &amp;lbrack;カメラ&amp;rbrack;正投影表示から遠近法表示に切り替えると間違ったズームが発生する(&amp;r)
* &amp;lbrack;Display&amp;rbrack；一部のマップはsRGBではなくリニアで表示されます
* &amp;lbrack;ビューポート&amp;rbrack; メッシュフォーカスが正しく動作しない
* &amp;lbrack;2D ビュー&amp;rbrack;プロジェクトのカメラが壊れているため、UVシェルが消えてしまう
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Tooltip&amp;rbrack;表面化散乱ツールチップがログに表示されます
* 一部のプロジェクトは2018.2で開くことができず、エラーメッセージがnull Substanceパッケージを保存できません
* &amp;lbrack;Mask&amp;rbrack;ペイントツールのカラーが、マスクの作業中にスタックすることがある
* &amp;lbrack;マテリアル&amp;rbrack；特定の状況でマップが表示されない
* &amp;lbrack；プロジェクト&amp;rbrack;&amp;lbrack；ツール&amp;rbrack;ジェネレータでアクティブなマニピュレーター
* &amp;lbrack;Substance&amp;rbrack;パラメータのSubstanceグループがありません
* &amp;lbrack；スクリプト&amp;rbrack；文書内のソフトウェア名が正しくない
* &amp;lbrack;UDIM&amp;rbrack；複数のUVタイル上のUVシェルに関するログに情報がありません

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ
* Windows OSでのショートカットに関するHuionタブレットの問題

### 4.2.1 (2018.2.1)

*（リリース：2018年8月3日）*

**修正済み：**

* プロジェクトのアップグレード時にシェーダーパラメーターが見つからない

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ
* Windows OSでのショートカットに関するHuionタブレットの問題

### 4.2.0 (2018.2.0)

*（リリース：2018年8月2日*）概要：**サマーリリース、表面化散乱サポート、投影と塗りつぶしの機能向上、カメラの読み込みと選択、AlembicとglTFのサポート、ID マップへのドラッグ&amp;ドロップ、Substance書式サポートの向上および新しいコンテンツ**

**追加：**

* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack;&amp;lbrack;Iray&amp;rbrack；一般表面化散乱
* &amp;lbrack;SSS&amp;rbrack; MDLと表面化散乱パラメータを同期
* &amp;lbrack;SSS&amp;rbrack; Scatteringという名前の新しいグレースケールチャンネルを追加しました
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;シェーダー設定&amp;rbrack;表面化散乱のスキャッタリングタイプパラメータ（スキンまたは半透明）
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;シェーダー設定&amp;rbrack;表面化散乱の散布スケールパラメータ
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;シェーダー設定&amp;rbrack;表面化散乱の拡散カラーパラメータ
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack；ディスプレイ設定&amp;rbrack;表面化散乱の散布サンプル数
* &amp;lbrack;シェーダー&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Irayの表面化散乱 MDLを統合
* &amp;lbrack;シェーダー&amp;rbrack; resource updaterによるシェーダーの更新
* &amp;lbrack;シェーダー&amp;rbrack; Update change log APIおよびドキュメント
* &amp;lbrack；ツールプロパティ&amp;rbrack;&amp;lbrack；プロジェクト&amp;rbrack; トライプラナー投影の新しいパラメータ
* &amp;lbrack;ビューポート&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; 3Dビューの塗りつぶしレイヤープロパティをマニピュレーター(トライプラナー投影)で直接制御
* &amp;lbrack；ショートカット&amp;rbrack;&amp;lbrack；プロジェクト&amp;rbrack;マニピュレーター用の新しいショートカットQ、W、E、R、T
* &amp;lbrack;ビューポート&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; 2D ビューの塗りつぶしレイヤープロパティをマニピュレーターで直接制御(UV 投影)
* &amp;lbrack;Shortcuts&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; マニピュレーターの新しいショートカット Q
* &amp;lbrack；コンテキストツールバー&amp;rbrack;&amp;lbrack；プロジェクト&amp;rbrack；制御マニピュレーター
* &amp;lbrack；コンテキストツールバー&amp;rbrack;&amp;lbrack；プロジェクト&amp;rbrack；制御マニピュレーター
* &amp;lbrack；ツールのプロパティ&amp;rbrack; 投影とステンシルツールでテクスチャタイリングを無効にする
* &amp;lbrack;ステンシル&amp;rbrack;投影ツール/ステンシルで非正方形の画像を使用
* &amp;lbrack;ステンシル&amp;rbrack;プロパティウィンドウでタイリングモードの制御を許可
* &amp;lbrack;ステンシル&amp;rbrack;ズームがタイリングでないステンシルの中央にない
* &amp;lbrack;カメラ&amp;rbrack; Maya、Max、Blender、Modo、DAEからカメラをインポート
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack；読み込んだカメラをビューポートで選択して制御
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Iray内の読み込まれたカメラを選択して制御
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;UI&amp;rbrack;&amp;lbrack；新規プロジェクト&amp;rbrack;&amp;lbrack；プロジェクト設定&amp;rbrack；読み込みカメラは、デフォルトでオンになっています
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack；ショートカット&amp;rbrack; カメラを切り替えるショートカットを追加
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack; ビューポートにフレームを追加
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;ビューポート設定&amp;rbrack; フレームの不透明度の制御
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;カメラ設定&amp;rbrack; 500 mmの最大焦点距離
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;カメラ設定&amp;rbrack;表示比
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;カメラ設定&amp;rbrack;ロックオプションを追加
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;カメラ設定&amp;rbrack; Add a restore option
* &amp;lbrack;カメラ&amp;rbrack;&amp;lbrack;カメラ設定&amp;rbrack;フォーカス距離の追加アトリビュート
* &amp;lbrack;glTF&amp;rbrack; glTFファイルのインポート
* &amp;lbrack;glTF&amp;rbrack; ambient occlusionマップをインポート
* &amp;lbrack;Alembic&amp;rbrack；静的ジオメトリを持つAlembic 1 フレームをインポート
* &amp;lbrack;シェルフ&amp;rbrack；修飾キー付きのID マップ(Ctrl/Command)を使用して、マテリアルをメッシュに直接ドラッグ&amp;ドロップ
* &amp;lbrack;レイヤースタック&amp;rbrack;ID マップを使用してメッシュ上にマテリアルをドラッグ&amp;ドロップすることでIDマスクを自動作成
* &amp;lbrack;レイヤースタック&amp;rbrack; レイヤースタック上をドラッグ&amp;ドロップした場合のレイヤーの自動スクロール
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack；ツールのプロパティ&amp;rbrack; Substanceのプリセットを表示
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack；ヘルプメニュー&amp;rbrack;ヘルプメニューの改善
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;New Project&amp;rbrack;&amp;lbrack;Project Configuration&amp;rbrack; Reorganization of the window
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;New Project&amp;rbrack;&amp;lbrack;Project Configuration&amp;rbrack; Replace メッシュの用語by File
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; UIにSubstance属性を表示
* &amp;lbrack；ショートカット&amp;rbrack; F4で2Dビューと3Dビューを切り替え
* &amp;lbrack；ショートカット&amp;rbrack;トグルステンシルNとクイックマスクUの新しいショートカット
* &amp;lbrack;Substanceの統合&amp;rbrack;Substanceパラメータの&#39;visible if&#39;ステートメントを考慮する
* &amp;lbrack;ビューポート&amp;rbrack;シャドウがカメラの移動後に強制的に計算されない
* &amp;lbrack;Content&amp;rbrack；読み込まれたカメラでMeetMatを更新
* &amp;lbrack;Content&amp;rbrack; 表面化散乱を有効にしてサンプルを追加 – JadeToad
* &amp;lbrack;Content&amp;rbrack; 表面化散乱を有効にして新しいPBRプロジェクトテンプレートを追加
* &amp;lbrack;Content&amp;rbrack；書き出しプリセットが更新され、新しいスキャッティングチャンネルが追加されました。
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack; pbr-metal-rough-alpha-test、pbr-coated、pbr-spec-glossの表面化散乱サポートを追加
* &amp;lbrack；コンテンツ&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack；散布チャンネルを5スマートマテリアル（マーブルとスキン）に追加
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack; 1 new jade マテリアル
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;シェルフ&amp;rbrack; 1 new wax マテリアル

**修正済み：**

* &amp;lbrack;CMD&amp;rbrack；同じコマンドラインを異なるバージョンで使用すると結果が異なる
* &amp;lbrack;TDR&amp;rbrack; TdrLevelが設定されている場合、ログにエラーはありません
* &amp;lbrack;ベイカー&amp;rbrack;Ambient occlusionマップを反転する(&amp;r)
* &amp;lbrack;ID マップ&amp;rbrack；範囲0 ～ 1以外を選択するとクラッシュする
* テクスチャセットを切り替えてペイントモードに戻るときに&amp;lbrack;Iray&amp;rbrack;クラッシュ
* &amp;lbrack;ビューポート&amp;rbrack;ドラッグ&amp;ドロップ用にドロップ領域をビューポート間で同期
* &amp;lbrack;エンジン&amp;rbrack;タイリング塗りつぶしレイヤー時または小さなブラシのペイント時のモアレの斑点
* &amp;lbrack;License&amp;rbrack; License service bad software version check
* &amp;lbrack;License&amp;rbrack；認証の処理方法を変更する
* &amp;lbrack;API&amp;rbrack;テンプレートを使用して作成する場合でも、 onNewProjectCreatedスクリプトAPIイベントを呼び出す
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーファイルがコンパイルされない場合、コンパイルされたシェーダーがキャッシュからロードされない
* &amp;lbrack;シェルフ&amp;rbrack; シェルフからHDRファイルを書き出すと、値が固定されたファイルが出力される
* &amp;lbrack；書き出し&amp;rbrack; EXR書き出しでは、RGBカラー値が0 ～ 1に固定される
* &amp;lbrack；コンテンツ&amp;rbrack;ノイズ 3Dパーリンノイズフラクタルがピクセル化される

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ
* Windows OSでのショートカットに関するHuionタブレットの問題

### 4.1.3 (2018.1.3)

*（リリース：2018年6月28日）*

**追加：**

* &amp;lbrack;Preferences&amp;rbrack; Painterの再起動時にプロジェクトを保存することを提案

**修正済み：**

* &amp;lbrack；プラグイン&amp;rbrack；検索Substance Sourceが機能しない
* &amp;lbrack;スマートマテリアル&amp;rbrack; スマートマテリアルを読み込むとクラッシュが発生することがある
* &amp;lbrack;スマートマテリアル&amp;rbrack; スマートマテリアルを削除するとクラッシュが発生する場合がある
* &amp;lbrack；保存&amp;rbrack；まれにクラッシュが発生する
* &amp;lbrack;シェルフ&amp;rbrack；反転がセル 2とセル 3で機能しない
* &amp;lbrack;シェルフ&amp;rbrack；一部のAlphaで誤字
* &amp;lbrack;シェルフ&amp;rbrack；一部のSubstanceマテリアルが正しくレンダリングされない

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ

### 4.1.2 (2018.1.2)

*（リリース：2018年6月12日*）概要：**ベイク処理速度の向上、保存システムの向上、スライダーの更新、プラグインAPIの更新、中国語の翻訳、パディングの改善オプション**

**追加：**

* &amp;lbrack;ベイカー&amp;rbrack；新しいベイカーバージョンによるパフォーマンスの向上
* 互換性のないGPUを使用してディスプレイダイアログを強制する
* &amp;lbrack；保存&amp;rbrack；新規コンパクトプロジェクト機能を表示（フル/コンパクトセーブモード）
* &amp;lbrack；保存&amp;rbrack；保存エラーが発生した場合にユーザーに通知
* &amp;lbrack;Clean&amp;rbrack；次の保存をフル/コンパクトモードで実行
* &amp;lbrack；スライダー&amp;rbrack;カラー/グレースケールバーとスライダーの精度の向上
* &amp;lbrack；スライダ&amp;rbrack；上/下矢印コントロールの追加
* &amp;lbrack；スライダー&amp;rbrack;カラーおよびグレースケールバースライダーの同じ検出ゾーン
* &amp;lbrack；プラグイン&amp;rbrack；常に増分モードで自動保存
* &amp;lbrack；プラグイン&amp;rbrack;プラグインを新しいインターフェイススタイルに切り替えるオプション
* &amp;lbrack；言語&amp;rbrack；中国語の翻訳を追加
* &amp;lbrack;Padding&amp;rbrack; テクスチャセット設定で、テクスチャセットごとのUVと3Dスペースの近隣パディングを切り替えるオプション
* &amp;lbrack；スクリプト&amp;rbrack；保存モードの表示：フル/コンパクトまたはインクリメンタル
* &amp;lbrack;Script&amp;rbrack;スクリプト/QMLドキュメントを更新
* &amp;lbrack;Log&amp;rbrack;ログに保存モードを指定（フル/コンパクトまたはインクリメンタル）

**修正済み：**

* &amp;lbrack;Tool&amp;rbrack; Channel slot 変形をシングルチャンネルフィルのマテリアルスロットに挿入(&amp;R)
* マテリアルによって割り当てられていない面を含むメッシュ(FBX)を読み込むときにクラッシュが発生する
* NVIDIA グリッド 5.2を搭載したIrayを仮想マシンでクラッシュする
* マテリアルプリセットの削除を取り消すときにクラッシュが発生する
* 一部のプロジェクトを読み込み中のクラッシュ
* &amp;lbrack；コマンドライン&amp;rbrack; メッシュの新しいコマンドラインsplit-by-udim
* &amp;lbrack；ツールバー&amp;rbrack;ツールバーの縮小
* &amp;lbrack；インスタンス化&amp;rbrack；複数のテクスチャセット間でビットマップをインスタンス化できない
* &amp;lbrack;ビューポート&amp;rbrack;タイルされたUVを使用してメッシュにペイントすると、リフレッシュが完了しない(&amp;R)
* &amp;lbrack;Iray&amp;rbrack;法線マップが誘電体に2回適用される
* &amp;lbrack;シェルフ&amp;rbrack；一部のSubstanceパラメーター(alpha、procedurals、matfx)で誤字が発生する
* &amp;lbrack；ビットマップ「Authorized Personnel Only」のシェルフ&amp;rbrack;タイプミス
* &amp;lbrack；スクリプト&amp;rbrack；関数alg.shaders.マテリアル()が機能しない

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ

### 4.1.1 (2018.1.1)

*（リリース：2018年4月3日）*

**修正済み：**

* &amp;lbrack;Tablet&amp;rbrack;デフォルトのインタラクション選択を変更する際の問題
* &amp;lbrack;ベイカー&amp;rbrack; Assimpライブラリとのクラッシュ
* &amp;lbrack;ベイカー&amp;rbrack; A.O.マップを使用したパフォーマンスの回帰
* &amp;lbrack;Iray&amp;rbrack;レンズゆがみがアルファチャンネルに適用されない
* &amp;lbrack；ドライバ&amp;rbrack；最小ドライバ要件の更新
* &amp;lbrack;3Dview&amp;rbrack；法線情報のないメッシュで法線が正しく生成されない
* &amp;lbrack;Intel&amp;rbrack; クラッシュ(Substance Painter 2018.1.0)
* &amp;lbrack;Intel&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack;パディングに関する問題（黒いアーティファクト）

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ

### 4.1.0 (2018.1.0)

*（リリース：2018年3月15日）*

**追加：**

* 新しい全体的なスタイル（アイコン、カラー、ビヘイビアー）
* 新しいデフォルトレイアウト
* &amp;lbrack;Tablet&amp;rbrack;ペイント時のユーザーエクスペリエンスの向上
* &amp;lbrack；メインメニュー&amp;rbrack;ビューおよびツールバーのネイティブ項目を最初に並べ替え
* &amp;lbrack；メインメニュー&amp;rbrack; ビューポートセクションのクイックマスクアクションを移動
* &amp;lbrack；メインメニュー&amp;rbrack；右クリック操作をビューポートセクションに移動
* &amp;lbrack；メインメニュー&amp;rbrack; 「表示」メニューを「ウィンドウ」に名前変更
* &amp;lbrack；クイックメニュー&amp;rbrack; ビューポートで右クリックして新しいツールプロパティを作成
* &amp;lbrack;Dockウィジェット&amp;rbrack；縮小/呼び出しを迅速に行うための新規ドッキングツールバー
* &amp;lbrack；ディスプレイ設定&amp;rbrack; カメラとビューア設定ウィンドウを統合
* &amp;lbrack;レイヤースタック&amp;rbrack;コンテキスト右クリックメニュー
* &amp;lbrack;レイヤースタック&amp;rbrack；同じレイヤー内でエフェクトをドラッグ&amp;ドロップ
* &amp;lbrack;Toolbar&amp;rbrack;ツールバーと新しいコンテキストツールバーの再編成
* &amp;lbrack；ツールツールバー&amp;rbrack;クローンツールを2つの個別のツールに分割
* &amp;lbrack；ツールのプロパティ&amp;rbrack;プレビューの背景グレースケール値を明るくする
* &amp;lbrack；ツールのプロパティ&amp;rbrack;タブ内の編成（塗りとツール）
* &amp;lbrack;Tool&amp;rbrack;ペイント結果がステンシルと一致する
* &amp;lbrack;ビューポート&amp;rbrack; 塗りつぶしレイヤーの新しいカーソル
* &amp;lbrack;ビューポート&amp;rbrack；よりスムーズなナビゲーションとペイント（高フレーム率）
* &amp;lbrack;ビューポート&amp;rbrack; マテリアル/チャンネル/マップ選択コンボボックス(ビューポート)
* &amp;lbrack;ビューポート&amp;rbrack；回転中のちらつきを低減（シャドウオン）
* &amp;lbrack;シェルフ&amp;rbrack; Painterを開いたときのデフォルトの表示マテリアル
* &amp;lbrack;シェルフ&amp;rbrack; Substanceテクスチャとマテリアルの読み込み時間の短縮（2 ～ 6倍速）
* &amp;lbrack;シェルフ&amp;rbrack; Substance Source構造に合わせてマテリアルフォルダを再編成
* &amp;lbrack;シェルフ&amp;rbrack; ビューポートのメッシュにマテリアルを直接ドラッグ&amp;ドロップ
* &amp;lbrack;シェルフ&amp;rbrack；新しい3Dノイズ（Perlin、Perlin Fractal、SimplexおよびWorley）
* &amp;lbrack;シェルフ&amp;rbrack; メッシュ位置を使用した新しい3D Linear gradientマスクジェネレーター
* &amp;lbrack;シェルフ&amp;rbrack;非正方形拡張をサポートするように基本ノイズを更新
* &amp;lbrack;シェルフ&amp;rbrack; Lens Studio （アプリケーションをスナップ）用に新しいテンプレートと書き出しプリセットを追加
* &amp;lbrack;シェルフ&amp;rbrack；最新バージョンのマスクエディターを使用するようにスマートマテリアルとスマートマスクを更新（マイクロディテール）
* &amp;lbrack;シェルフ&amp;rbrack；シームレスなタイリングマテリアルを実現する新しいサンプルプロジェクト「TilingMaterial」
* &amp;lbrack;シェルフ&amp;rbrack；新規ブラシプリセット（カリグラフィー、ウェット、ハッチングなど）
* &amp;lbrack；スライダー&amp;rbrack；新しいスライダーとグレースケール/カラーバーのスタイルと動作
* &amp;lbrack;ベイカー&amp;rbrack; シーンのバウンディングボックスを使用してポジションマップを計算できるようにします
* &amp;lbrack;シェーダー&amp;rbrack;デフォルトのシェーダーパラメータからHeight力パラメータを削除
* &amp;lbrack;エンジン&amp;rbrack; Substanceエンジンを更新
* &amp;lbrack;エンジン&amp;rbrack; UVチャンク間の不連続性の有無(&amp;r)
* &amp;lbrack；プラグイン&amp;rbrack; Substance Sourceからダウンロードしたマテリアルの読み込みをより迅速に
* &amp;lbrack；プラグイン&amp;rbrack；新しい全体的なスタイルに合うようにすべてのプラグインを更新
* &amp;lbrack;Preferences&amp;rbrack; Preview background color changes automatically
* &amp;lbrack;Clean&amp;rbrack;プロジェクト破損のリスクを軽減
* &amp;lbrack;Open&amp;rbrack；開始プロジェクト時間の改善
* &amp;lbrack；新規プロジェクト&amp;rbrack；新規プロジェクト – メッシュ更新時間の短縮
* &amp;lbrack；保存&amp;rbrack;プロジェクト時間の短縮
* &amp;lbrack;Log&amp;rbrack;ログに報告されるライセンスの種類
* &amp;lbrack;TextureSet&amp;rbrack; 「メッシュマップをベイク」ボタンを「テクスチャをベイク」に名前変更
* 「その他のマップ」を「メッシュマップ」に名前変更

**修正済み：**

* &amp;lbrack;ビューポート&amp;rbrack；多数のサブオブジェクトを含むメッシュのパフォーマンスが低い(&amp;lbrack;)
* &amp;lbrack；ツールのプロパティ&amp;rbrack；画像をマテリアルスロットにドラッグアンドドロップするとチャンネルが無効になる
* &amp;lbrack；ツールのプロパティ&amp;rbrack;ブラシプレビューが指先ツールとクローンツールで壊れる
* &amp;lbrack;テクスチャセット&amp;rbrack;テンプレートを使用する際にチャネルの順序が間違っている
* &amp;lbrack;シェルフ&amp;rbrack; グレースケール変換ジェネレータのアイコンがありません
* &amp;lbrack;シェルフ&amp;rbrack；記号円番号のアルファが壊れています（フォントがありません）
* 起動時に統合GPUが誤って検出される
* &amp;lbrack;クラッシュ&amp;rbrack；読み込まれたリソースを#文字で指定してドラッグ&amp;ドロップする
* &amp;lbrack；統合GPUでのエンジン&amp;rbrack; Vram検出の問題
* &amp;lbrack;エンジン&amp;rbrack; Substance engineリンカーの多数のクラッシュを修正
* &amp;lbrack;エンジン&amp;rbrack；解像度を変更する際の正方形のアーティファクト
* &amp;lbrack;ポストエフェクト&amp;rbrack; ポストエフェクトがオンの時にインターフェイスのサイズ変更が遅い
* &amp;lbrack;ベイカー&amp;rbrack;シーン単位が[レイ距離]の値に正しく適用されない
* &amp;lbrack;ベイカー&amp;rbrack; メッシュオクルーダー距離からのAOは、入力値にかかわらず1にクランプされます。
* &amp;lbrack;ベイカー&amp;rbrack；名前で一致は、特定の名前を持つ一部のメッシュを無視します
* &amp;lbrack;ベイカー&amp;rbrack; メッシュのポリグループのカラーとサブメッシュのID設定は、常に黒いイメージを返す
* &amp;lbrack;ベイカー&amp;rbrack; ID ベイク処理がBlenderからのバイナリFBX メッシュで失敗する
* dota-2およびnon-pbr-spec-glossを使用した2D ビューの&amp;lbrack;シェーダー&amp;rbrack;ノイズ
* &amp;lbrack;Linux&amp;rbrack;ベイク時にCPUスレッドが1つだけ使用される
* &amp;lbrack;MacOS&amp;rbrack; クラッシュとビューポート上のブラシカーソル

**既知の問題：**

* AMD VEGA GPUでの計算フリーズ
* Iray（アルファ）への書き出し時に、ゆがみ後処理が考慮されない

## バージョン3

### 3.4.2 (2017.4.2)

*（リリース：2018年1月24日）*

**追加：**

* &amp;lbrack;Export&amp;rbrack;ステップの進捗状況を含む書き出しのステータスを取得する
* &amp;lbrack;Export&amp;rbrack；書き出しのキャンセルを許可
* &amp;lbrack；書き出し&amp;rbrack;法線マップの質を損なわずにテクスチャをSketchfabに書き出す
* &amp;lbrack；書き出し&amp;rbrack; glTFバイナリ形式(glb)で書き出し
* &amp;lbrack;Export&amp;rbrack；書き出しウィンドウの「設定」タブで列のサイズ変更を許可
* &amp;lbrack;シェーダー&amp;rbrack; シェーダー APIの変更ログを追加する
* &amp;lbrack;Scripting&amp;rbrack; テクスチャの書き出し時にコールバック関数の前と後に追加
* &amp;lbrack;Iray&amp;rbrack; SDK 2017.1にアップグレード（Volta GPUのサポート）

**修正済み：**

* メインウィンドウが表示される前にアプリケーションを終了すると、クラッシュが発生します
* &amp;lbrack;IRAYを含むグレースケールマップを読み込むときにMAC&amp;rbrack; クラッシュが発生する
* &amp;lbrack;MAC&amp;rbrack; VRAMが新しいHigh Sierra OSで正しく検出されない
* &amp;lbrack;Plugin&amp;rbrack; Substance Sourceからアセットをダウンロードできない
* &amp;lbrack；スクリプト&amp;rbrack；最小プラグインバージョン検出が正しくない
* &amp;lbrack;Export&amp;rbrack; テクスチャの書き出し後、書き出しプリセットを保存できない
* &amp;lbrack；他のマップを持たないTextureSetでインスタンス化されたジェネレータでのインスタンス化&amp;rbrack；の問題
* &amp;lbrack;ビューポート&amp;rbrack; ディザリングが4kを超える解像度では動作しない
* &amp;lbrack;ビューポート&amp;rbrack; 2D ビューマテリアルの表示がノイズで覆われている
* &amp;lbrack;シェルフ&amp;rbrack; シェルフプリセットの読み込み時間を短縮
* &amp;lbrack;エンジン&amp;rbrack;カラー選択でペイントすると正しくブレンドされない

### 3.4.1 (2017.4.1)

*（リリース：2017年12月15日）*

**追加：**

* &amp;lbrack；スクリプト&amp;rbrack;スクリプトAPIによるメッシュの書き出し
* &amp;lbrack;Import&amp;rbrack;サポートされていないメッシュファイルフォーマットのインポートを無効にする（obj、fbx、dae、plyのみ許可）
* &amp;lbrack;Log&amp;rbrack;ログファイルのTDR問題をより正確に示す

**修正済み：**

* リソースのクロールが完了する前にアプリケーションを閉じるとクラッシュが発生します
* 指先/クローンツールでプロジェクトを開く際にクラッシュが発生する
* ビューアの設定でシェーダーの変更を取り消した後にやり直しを使用すると、クラッシュが発生します
* &amp;lbrack;エンジン&amp;rbrack;テクスチャリングがPainter 2017.2と2017.4で異なる
* &amp;lbrack;ビューポート&amp;rbrack;インスタンスからID マップを選択すると、間違ったカラーがサンプリングされる
* &amp;lbrack；無効な標準モードまたはテクスチャを書き出すときにExport&amp;rbrack; クラッシュが発生する
* &amp;lbrack;Export&amp;rbrack; PSDファイルをPhotoshop CS6で開くと、グループがロックされる
* &amp;lbrack;Plugin&amp;rbrack; Photoshopプラグインは、チャンネルの選択を無視し、常にすべてを書き出す
* &amp;lbrack；レイヤー&amp;rbrack;アンカーをテクスチャセット間でコピー/ペーストすると壊れる
* &amp;lbrack;Layers&amp;rbrack；一部のアンカーの参照は、破損している場合は復元できません
* &amp;lbrack;シェーダー&amp;rbrack; pbrコーティングされた二次ラフネスパラメータが壊れています
* &amp;lbrack;Steam&amp;rbrack;バージョンチェッカーのポップアップが起動時に表示されない

**既知の問題：**

* &amp;lbrack;AMD&amp;rbrack; メッシュでペイントしようとすると、クラッシュ/フリーズする。 GPUドライバーのアップデートで修正できます。

### 3.4.0 (2017.4.0)

*（リリース：2017年11月23日）*

**追加：**

* &amp;lbrack；インスタンス化&amp;rbrack;レイヤー間でパラメーターをインスタンス化可能
* &amp;lbrack；インスタンス化&amp;rbrack;ソースレイヤーとインスタンス間のジャンプを許可
* &amp;lbrack；インスタンス化&amp;rbrack; 「テクスチャセット間でインスタンス化」操作を追加
* &amp;lbrack；インスタンス化&amp;rbrack; レイヤースタック内の再入可能なインスタンス（サイクル）を示す
* &amp;lbrack；インスタンス化&amp;rbrack;ソースが削除されたときにインスタンスを削除
* &amp;lbrack；インスタンス化&amp;rbrack;インスタンス化されたフォルダの外部からのアンカー参照を許可しない
* &amp;lbrack;UI&amp;rbrack；取り消しスタックを「ヒストリー」という名前のウィンドウに移動する
* &amp;lbrack；プラグイン&amp;rbrack; DCC live-linkプラグインを統合
* &amp;lbrack;エンジン&amp;rbrack;スパースペイントでパフォーマンスを向上させる
* &amp;lbrack；書き出し&amp;rbrack;ドラフトおよび再書き出しオプションをSketchfabエクスポーターに追加
* &amp;lbrack;シェルフ&amp;rbrack;フォントのサブスタンスに「フリップ」コントロールを追加
* &amp;lbrack;シェルフ&amp;rbrack; 20個の新しい手続きマテリアルを追加
* &amp;lbrack;シェルフ&amp;rbrack; 40個の新しいグランジマップ（ビットマップに基づくマップとプロシージャルマップ）を追加
* &amp;lbrack;ビューポート&amp;rbrack；他の可視テクスチャセットでブラシのプレビュー衝突を有効にする
* AMD GPUドライバーの最小要件を更新する

**修正済み：**

* 解像度が大きすぎる場合にSubstanceを計算するとクラッシュが発生する
* パーティクルを大量に使用してペイントする場合のクラッシュ
* &amp;lbrack;ビューポート&amp;rbrack；特定のメッシュを持つSpecularに誤った2D ビューリフレクションが含まれている
* &amp;lbrack;UI&amp;rbrack；不要なアクションがヒストリーウィンドウに表示される

**既知の問題：**

* &amp;lbrack;Layers&amp;rbrack；一部のアンカーの参照は、破損している場合は復元できません
* ビューアの設定でシェーダーの変更を取り消した後にやり直しを使用すると、クラッシュが発生します

### 3.3.3 (2017.3.3)

*（リリース：2017年12月1日）*

**修正済み：**

* &amp;lbrack;Steam&amp;rbrack;バージョンチェッカーのポップアップが起動時に表示されない
* &amp;lbrack;Export&amp;rbrack; PSDファイルをPhotoshop CS6で開くと、グループがロックされる

### 3.3.2 (2017.3.2)

*（リリース：2017年11月20日）*

**追加：**

* &amp;lbrack;UI&amp;rbrack；新規バージョンダイアログの改善と変更ログの追加
* &amp;lbrack;UI&amp;rbrack;メンテナンスが期限切れかどうかを新しいバージョンダイアログで示す
* &amp;lbrack;License&amp;rbrack;メンテナンス日を処理するためのライセンスシステムの更新
* &amp;lbrack；書き出し&amp;rbrack; Adobe Standard Material名をAdobe Dimensionに変更

**修正済み：**

* &amp;lbrack;Mac&amp;rbrack;ペイントにより黒い正方形とテクスチャの破損が生じる
* &amp;lbrack;エンジン&amp;rbrack;キャッシュがビューポートから消えることがある
* &amp;lbrack;エンジン圧縮がトリガーされると、ブロックノイズが表示される(&amp;rbrack; Memory&amp;rbrack; Blocky artifacts)
* &amp;lbrack;ベイク&amp;rbrack；特定のメッシュをベイクする際の奇妙なエラーメッセージ
* &amp;lbrack;Export&amp;rbrack; PSDが正しく書き込まれず、Photoshopで正しく認識されない
* &amp;lbrack；レイヤー&amp;rbrack；複数のプロジェクト間でレイヤーをコピー/ペーストすることはできません
* &amp;lbrack;Substance&amp;rbrack；通常入力のUserDataカラースペースが反転することがある
* &amp;lbrack;シェルフ&amp;rbrack;ジェネレータのマイクロノーマル出力の逆曲率
* &amp;lbrack;シェルフ&amp;rbrack; HSLフィルタもアルファチャンネルに影響します
* &amp;lbrack;Linux&amp;rbrack; Centosへのインストールが失敗する。依存関係が見つからないためです。
* インストーラーが以前にインストールしたすべてのリソースを削除しない場合がある

### 3.3.1 (2017.3.1)

*（リリース：2017年10月26日）*

**追加：**

* &amp;lbrack;Export&amp;rbrack;プロジェクトからメッシュをエクスポートできるようにします
* &amp;lbrack;シェルフ&amp;rbrack;タブタイトルから「サブシェルフ」を削除
* 後処理の設定をテンプレートに保存
* TDRメッセージをより理解しやすくする
* エラーを報告するための設定ウィンドウの改善

**修正済み：**

* 複数のサブシェルフを削除するときにクラッシュが発生しました
* 計算中にレベルから別のレベルに切り替えるとクラッシュが発生する
* 計算中のIntel GPUでのMacのクラッシュ(&amp;lbrack)(&amp;rbrack)
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;ビューポート&amp;rbrack; ディザリングが有効な場合のパフォーマンスが低下する
* &amp;lbrack;Mac&amp;rbrack; MacOS 10.13がログファイルで「不明なバージョン」として認識される
* &amp;lbrack;ベイカー&amp;rbrack; ケージとのベイクが機能しなくなりました。
* &amp;lbrack；レイヤー&amp;rbrack; Ctrl + C ショートカット（コピー操作）が機能しない
* &amp;lbrack；レイヤー&amp;rbrack;レイヤーをペーストしても、アンカーの参照でUIが更新されない
* &amp;lbrack；アンカー&amp;rbrack;リンクを切断するリファレンスを含むレイヤーを複製またはコピー/ペースト
* &amp;lbrack;Export&amp;rbrack; 8K exportは、場合によってはアプリケーションをクラッシュまたはデッドロックさせることがあります。
* &amp;lbrack;Export&amp;rbrack；生成されたglTFファイル形式に複数の問題があります
* &amp;lbrack;Import&amp;rbrack；同じファイル名でメッシュを再読み込みできない
* &amp;lbrack；プラグイン&amp;rbrack；自動保存ウィンドウは常にすべてに重ねて表示される
* &amp;lbrack;UI&amp;rbrack; TDRダイアログで「Esc」を押すと無限ループが発生する
* &amp;lbrack;UI&amp;rbrack; UIをリセットすると、シェルフウィンドウに2番目のタイトルバーが表示されます。

### 3.3.0 (2017.3.0)

*（リリース：2017年9月28日）*

**追加：**

* &amp;lbrack；書き出し&amp;rbrack; AdobeプロジェクトFelixのメッシュとテクスチャの書き出しを許可
* &amp;lbrack;Export&amp;rbrack; glTFファイル形式へのエクスポートを許可
* &amp;lbrack;エンジン&amp;rbrack; VRAMでブロック圧縮を使用してテクスチャサイズを最適化
* &amp;lbrack;ビューポート&amp;rbrack; ビューポートにメッシュまたはプロジェクトをドラッグ&amp;ドロップ可能
* &amp;lbrack;UI&amp;rbrack; TDRに関する警告メッセージを改善
* &amp;lbrack;UI&amp;rbrack;ログは、要求があるときにのみ表示されます。
* &amp;lbrack;UI&amp;rbrack;ログウィンドウの内容をクリアできるようにします
* &amp;lbrack;UI&amp;rbrack；警告とエラーをステータスバーに表示
* &amp;lbrack;UI&amp;rbrack;タブをWebブラウザーと同じように上部に表示
* &amp;lbrack;UI&amp;rbrack; 「非ペイント可能」のコンテキストとメッセージを改善
* &amp;lbrack;UI&amp;rbrack; [ファイル]メニューに[コピーとして保存]アクションを追加
* &amp;lbrack；画層&amp;rbrack；既定のタイリング設定を既定で1に設定
* &amp;lbrack;シェルフ&amp;rbrack; 10色のダイナミックカラーをサポートするようにグラデーションフィルターを改善
* &amp;lbrack;シェルフ&amp;rbrack;ミニシェルフのデフォルトクエリにスペースを追加する
* &amp;lbrack;シェルフ&amp;rbrack; シェルフ内のローカルリソースに「エクスプローラーで開く」アクションを追加
* &amp;lbrack;シェルフ&amp;rbrack; Adobeマテリアル標準（プロジェクトFelix）のテンプレートとシェーダーを追加
* &amp;lbrack;シェルフ&amp;rbrack;マテリアルレイヤシェーダの最大タイリングを128に増加
* &amp;lbrack;シェルフ&amp;rbrack; マスクジェネレーターのマイクロディテールにsobel曲率を追加
* &amp;lbrack；プラグイン&amp;rbrack;カスタマイズ可能な時間間隔で自動保存プラグインを追加
* &amp;lbrack；スクリプト&amp;rbrack; 「コピーとして保存」機能を追加

**修正済み：**

* &amp;lbrack;UI&amp;rbrack;レイアウトが最初の起動時に壊れる
* 書き出し時に生成された&amp;lbrack；書き出し&amp;rbrack; PSDにフォーマットエラーがある
* &amp;lbrack;Export&amp;rbrack; EXRは常に8ビットを高さマップで書き出す
* 破損した追加マップを書き出すときに&amp;lbrack;Export&amp;rbrack; クラッシュ
* &amp;lbrack；読み込み&amp;rbrack；ハードエッジがローポリメッシュで保持されない場合がある
* &amp;lbrack;Import&amp;rbrack；問題のあるメッシュを読み込む際のエラーメッセージを改善
* &amp;lbrack;ベイカー&amp;rbrack; ID マップベイクが失敗し、「名前による一致」が有効になっている
* &amp;lbrack;ビューポート&amp;rbrack; 正接空間がベイカーと同期されない
* &amp;lbrack；エフェクト&amp;rbrack;レイヤーを戻してもアンカーの参照が復元されない
* &amp;lbrack；エフェクト&amp;rbrack;アンカーを使用して2つのマスク間にリンクを作成する際のリフレッシュの問題
* &amp;lbrack;Effect&amp;rbrack;マスクの上にあるマスクアンカーを表示しないでください
* &amp;lbrack；エフェクト&amp;rbrack; 「アンカーからAlpha設定を抽出」が機能しない
* &amp;lbrack;エンジン&amp;rbrack;マスクが最初のブラシストロークの後に反転する
* &amp;lbrack；特定のプロジェクトでテクスチャセットを切り替える際のエンジン&amp;rbrack;クラッシュ
* プロジェクト内のプリセットを削除するときに発生する&amp;lbrack;シェルフ&amp;rbrack;クラッシュ
* 高度な三平面フィルターのシェルフが間違っている(&amp;lbrack;R&amp;R)
* &amp;lbrack;シェルフ&amp;rbrack; MGマスクビルダーAOノイズスケールが正しく機能しない
* &amp;lbrack;シェルフ&amp;rbrack; MGマスクビルダーで曲率パラメーターが反転されました
* &amp;lbrack;シェルフ&amp;rbrack；読み込まれたアルファは、平坦な球ではなく、マテリアルの球のプレビューを生成します

### 3.2.0 (2017.2.0)

*（リリース：2017年7月27日）*

**追加：**

* アンカーポイント – レイヤーとマスク参照システム
* &amp;lbrack；レイヤー&amp;rbrack；塗りつぶしとペイントエフェクトの名前を変更する機能
* &amp;lbrack；プラグイン&amp;rbrack；更新されたSubstance Sourceプラグイン
* &amp;lbrack;Scripting&amp;rbrack; Allow to query テクスチャセット解決
* &amp;lbrack;Scripting&amp;rbrack;ペイントエンジンのステータスを取得できるようにします
* &amp;lbrack；パフォーマンス&amp;rbrack;プロジェクトの読み込みとブラシスタンプの最適化を改善

**修正済み：**

* &amp;lbrack;Tool&amp;rbrack; マテリアルパラメーターを微調整する際のパフォーマンスの問題
* &amp;lbrack;エンジン&amp;rbrack；解像度を変更するとブラシストロークが消える(4K>2K)
* &amp;lbrack;3D ビュー&amp;rbrack; 正接空間がベイカーと同期されない
* ユーザードキュメントのシェルフパスが自動的に作成されない(&amp;lbrack;シェルフパス(&amp;rbrack;)
* &amp;lbrack;シェルフ&amp;rbrack；更新後にプリセットを以前のバージョンと互換性を持たせる
* &amp;lbrack;シェーダー&amp;rbrack；非PBR シェーダーが機能しない
* &amp;lbrack;ベイカー&amp;rbrack; ID マップベイクが失敗し、「名前による一致」が有効になっている
* &amp;lbrack;Sample&amp;rbrack; Meet Matサンプルプロジェクトテクスチャセット名が正しくない
* テンプレートを作成する前にプロジェクトを保存すると、書き込み権限エラーが返される

### 3.1.0 (2017.1.0)

*（リリース：2017年6月20日）*

**追加：**

* &amp;lbrack；プラグイン&amp;rbrack；新規Substance Sourceプラグイン（シェルフ内のアセットのダウンロードを許可）
* &amp;lbrack;シェルフ&amp;rbrack; 4つの新しいフォント（日本語+簡体字中国語、タイプライター、セグメント）
* &amp;lbrack;シェルフ&amp;rbrack; 230新しいAlpha （パターン、ブラシ、および指紋スキャンの組み合わせ）
* &amp;lbrack;シェルフ&amp;rbrack; 50 New Procedurals （中世と現代の衣服の生地のパターン）
* &amp;lbrack;シェルフ&amp;rbrack; 2つの新しい環境マップ (Mondarrain and Villa Nova Street)
* &amp;lbrack;シェルフ&amp;rbrack; 9新しいフィルタ（MatFxディテールEdge Wear、クランプ、HBAOなど）
* &amp;lbrack;シェルフ&amp;rbrack;デフォルトのパノラマ環境マップを改善
* &amp;lbrack;シェルフ&amp;rbrack；新規Arnold 5書き出しプリセット
* &amp;lbrack;Scripting&amp;rbrack;リソースをシェルフにインポートできるようにします

**既知の問題：**

* &amp;lbrack；書き出し&amp;rbrack；書き出しプリセットの編集が非常に遅い

## バージョン2

### 2.6.2

*（リリース：2017年10月20日）*

**追加：**

* &amp;lbrack;テクスチャセット&amp;rbrack；無効なテクスチャセットを削除できるようにします
* &amp;lbrack;シェルフ&amp;rbrack；複数のユーザが同じシェルフフォルダ内に書き込めるようにする
* &amp;lbrack;Scripting&amp;rbrack;プラグインフォルダーを再読み込みできる
* &amp;lbrack;Scripting&amp;rbrack；互換性を確保するために、プラグインメタデータに必要な最小限のAPIバージョンを追加する
* &amp;lbrack;Iray&amp;rbrack;イメージのエクスポートダイアログの改善

**修正済み：**

* &amp;lbrack;エンジン&amp;rbrack；解像度を変更する際に、ストロークが消える問題(4K>2K)
* &amp;lbrack;ベイカー&amp;rbrack; ID マップベイクが失敗し、「名前による一致」が有効になっている
* &amp;lbrack;ベイカー&amp;rbrack;エラーメッセージが明確ではありません
* &amp;lbrack;3D ビュー&amp;rbrack; 正接空間がベイカーと同期されない
* &amp;lbrack；ツール&amp;rbrack；指先ツール使用時の黒い斑点
* &amp;lbrack;シェーダー&amp;rbrack；非PBR シェーダーが機能しない
* &amp;lbrack;シェーダー&amp;rbrack; 「pbr-coated」が壊れています
* &amp;lbrack;シェーダー&amp;rbrack; 「pbrコーティングされた」シェーダーのコーティングラフネスに影響がありません
* &amp;lbrack;シェーダー&amp;rbrack; Spec gloss シェーダーがIrayとSDと一致しない
* 同じ名前で拡張子の異なる2つのファイルを読み込むときに&amp;lbrack;シェルフ&amp;rbrack;クラッシュが発生する
* &amp;lbrack;シェルフ&amp;rbrack; シェルフでプリセットを編集できない
* &amp;lbrack;シェルフ&amp;rbrack; シェルフに読み込まれたアセットのカスタムプレビューを設定できない
* キャッシュから読み込まれたリソースは使用を失います
* テンプレートを作成する前にプロジェクトを保存すると、書き込み権限エラーが返される
* ファイル名に2つのピリオドが含まれていると、プロジェクトが正しく保存されない。
* 複数のドット(.)を含むファイルの読み込み ファイル名に問題がある

### 2.6.1

*（リリース：2017年5月12日）*

**追加：**

* &amp;lbrack;TextureSet&amp;rbrack; マテリアルをNothingに再割り当てできません

**修正済み：**

* ベイク済みマップの交換後にTextureSetを切り替えるとクラッシュが発生する
* レイヤーの描画モードを変更した後、「取り消しとやり直し」を行うとクラッシュが発生する
* 大きなID マップで「カラー選択」エフェクトを使用するとクラッシュまたはフリーズする
* &amp;lbrack;Export&amp;rbrack；名前を変更したテクスチャセットが、書き出しウィンドウでアルファベット順に並べ替えられない
* &amp;lbrack;TextureSet&amp;rbrack;デフォルト名にリセットしても不一致がチェックされない
* &amp;lbrack;TextureSet&amp;rbrack；名前変更されたテクスチャセットは、プロジェクトを再度開くと無効になります。
* &amp;lbrack;シェルフ&amp;rbrack；見つからないデフォルトのテンプレートコンテンツ
* &amp;lbrack;シェルフ&amp;rbrack；非正方形テクスチャは正方形として表示
* &amp;lbrack;シェーダー&amp;rbrack; テクスチャセットが無効になると、関連付けられたシェーダーは破棄されます
* &amp;lbrack;Scripting&amp;rbrack; alg.ベイク.setTextureSetBakingParameters()が機能しない
* &amp;lbrack;Scripting&amp;rbrack; Typo in websocket tutorial
* &amp;lbrack;Scripting&amp;rbrack; AlgWidgetsの様々な問題
* &amp;lbrack;Log&amp;rbrack；使用可能な仮想メモリが正しく検出されない場合がある

### 2.6.0

*（リリース：2017年4月27日）*

**追加：**

* 新しいサンプルプロジェクト「Meet Mat」を追加
* &amp;lbrack；プラグイン&amp;rbrack；新規「リソースアップデーター」プラグイン
* &amp;lbrack;TextureSet&amp;rbrack；名前を変更してテクスチャセットに説明を追加できます
* &amp;lbrack;TextureSet&amp;rbrack; マテリアルの再割り当てを許可する
* &amp;lbrack;TextureSet&amp;rbrack; [テクスチャセットリスト]ウィンドウに設定ボタンを追加
* &amp;lbrack;TextureSet&amp;rbrack;リストの一番下に「無効」テクスチャセットを表示
* &amp;lbrack;Substance&amp;rbrack；現在のテクスチャセット解像度で追加のマップを使用してパフォーマンスを向上させる
* &amp;lbrack;Scripting&amp;rbrack;プロジェクトで使用するリソース（マテリアル、ジェネレータなど）を更新できるようにします。
* &amp;lbrack;Scripting&amp;rbrack; Add a way to add/remove a シェルフ
* &amp;lbrack;Scripting&amp;rbrack;プロジェクト内のリソースからの情報のクエリを許可
* &amp;lbrack；スクリプト&amp;rbrack；使用可能なシェルフのリストを取得できるようにします
* &amp;lbrack;Scripting&amp;rbrack; AlgWidgetサムネールチュートリアルの改善
* &amp;lbrack；書き出し&amp;rbrack;ファイルフォーマットのサポートに基づいてビット深度を無効/有効にする
* &amp;lbrack;Log&amp;rbrack;コンソールに印刷するプラグイン名を追加
* &amp;lbrack;Log&amp;rbrack; Remove error about hidden テクスチャセット
* サンプルの新しいアイコンとテキストで「ようこそ画面」を更新

**修正済み：**

* 特定のプロジェクトでメッシュを更新するとクラッシュが発生する
* &amp;lbrack;ビューポート&amp;rbrack;対称プレーンの内側の色が表示されなくなりました。
* &amp;lbrack;ビューポート&amp;rbrack;ソロビューを使用すると、一部の後処理エフェクトが有効になる
* &amp;lbrack；シェーダ&amp;rbrack; 「over_premult」ブレンドが正しく動作しない
* &amp;lbrack；シェーダ&amp;rbrack;デフォルトシェーダーを使用したアルファテストに関する警告
* &amp;lbrack;Substance&amp;rbrack; シェルフからのタグの解析が正しくありません
* &amp;lbrack;シェルフ&amp;rbrack; MatFX 錆風化が正しく動作しない
* &amp;lbrack;シェルフ&amp;rbrack; HSLフィルタは、不正なチャンネルでデフォルトで有効になっています。
* &amp;lbrack;シェルフ&amp;rbrack;シャープは、デフォルトではHeight/通常チャンネルで有効になっています
* &amp;lbrack;Export&amp;rbrack; Vray書き出しプリセットがOpenGL 法線マップを使用しない
* &amp;lbrack；ツール&amp;rbrack;クローン/指先ツールで斑点を作成する際の精度の問題

### 2.5.3

*（リリース：2017年3月15日）*

**修正済み：**

* &amp;lbrack；特定のメッシュでベイクする場合のベイカー&amp;rbrack;クラッシュ

**既知の問題：**

* &amp;lbrack;Mac&amp;rbrack; パーティクルがテクスチャの破損を引き起こす場合がある

### 2.5.2

*（リリース：2017年3月14日）*

**修正済み：**

* &amp;lbrack;Tool&amp;rbrack; WacomタブレットがLinuxで動作しない
* &amp;lbrack；ツール&amp;rbrack；指先ツール使用時の黒い斑点
* &amp;lbrack;ベイカー&amp;rbrack；名前で一致がケージと共に使用されている場合、ベイクが失敗する(&amp;L)
* &amp;lbrack;ベイカー&amp;rbrack; 法線マップのみでベイク中にAmbient occlusionが壊れる(&amp;r)
* &amp;lbrack;シェルフ&amp;rbrack；汎用フィルターがアルファを正しく処理しない（コントラスト/輝度、ハイパスなど）
* &amp;lbrack;ビューポート&amp;rbrack;シャドウが有効になっているプロジェクトを読み込む際のパフォーマンスの問題
* macOSの3D ビューのビューポート&amp;rbrack; ディザリングに関する問題
* &amp;lbrack;ビューポート&amp;rbrack;カラープロファイルが有効な場合にパーティクルプレビューが正しく表示されない
* Irayの初期化に失敗した場合、プロジェクトをOpenGLに戻すときに&amp;lbrack;Iray&amp;rbrack;クラッシュが発生します。
* &amp;lbrack;Iray&amp;rbrack;光沢度は、SpecGloss シェーダー/mdlのレンダリング時に無視されます。
* &amp;lbrack;シェーダー&amp;rbrack；仕様/グロスシェーダーがIrayとSDと一致しない
* &amp;lbrack;シェーダー&amp;rbrack; sRGB変換がリニアからsRGB LUT変換と異なる
* &amp;lbrack;シェーダー&amp;rbrack；古いシェーダでプロジェクトをロードすると、正しくレンダリングされない。
* &amp;lbrack;シェーダー&amp;rbrack; 「pbrコーティングされた」シェーダーが機能しない
* &amp;lbrack;Export&amp;rbrack; テクスチャセットに存在しない場合でも、一部のチャンネルが書き出される
* &amp;lbrack；レイヤー&amp;rbrack；描画モード「法線マップ逆ディテール」がグレースケールチャンネルで機能しない
* HDPIモニターおよびディスプレイズームが150%の「カラー選択ウィンドウ」でのUI&amp;rbrack；の問題(&amp;lbrack)

**既知の問題：**

* &amp;lbrack;Mac&amp;rbrack; パーティクルがテクスチャの破損を引き起こす場合がある

### 2.5.1

*（リリース：2017年2月27日）*

**修正済み：**

* &amp;lbrack;Mac&amp;rbrack; Wacomタブレットの入力が3Dと2D ビューで壊れている
* &amp;lbrack;ベイカー&amp;rbrack；名前による一致が機能しなくなった
* &amp;lbrack;ベイカー&amp;rbrack; 「平均法線」設定が機能しない
* &amp;lbrack;Iray&amp;rbrack;ベイクされた法線マップが見つからないと、正しくレンダリングされません
* &amp;lbrack;Iray&amp;rbrack; カラープロファイルがOpenGLレンダラーと異なる動作をする
* &amp;lbrack;Iray&amp;rbrack;レンダリングをビットマップとして書き出すと、カラープロファイル補正が含まれない
* &amp;lbrack;Substance&amp;rbrack; マテリアルフィルターが機能しない
* &amp;lbrack;Tool&amp;rbrack; Stroke opacity isn&#39;t stored in ブラシプリセット
* &amp;lbrack;Tool&amp;rbrack; クローンブラシのUVアラインメントが機能しない
* 整数で書き出す場合、&amp;lbrack;Export&amp;rbrack; ディスプレイスメントチャンネルの中央は0.5になるはずです。
* &amp;lbrack；テンプレート&amp;rbrack；絶対パスはテンプレートに保存されます
* &amp;lbrack;TextureSet&amp;rbrack;チャンネルを削除した後もチャンネルのテクスチャが維持される

**既知の問題：**

* &amp;lbrack;Linux&amp;rbrack; Wacomタブレット入力が3Dおよび2D ビューで機能しない
* &amp;lbrack;Mac&amp;rbrack; パーティクルがテクスチャの破損を引き起こす場合がある
* &amp;lbrack；書き出し&amp;rbrack；非常にまれですが、AMD GPUで黒い長方形が表示されることがあります

### 2.5.0

*（リリース：2017年2月21日）*

**追加：**

* AMD Radeon ProおよびAMD FirePro GPUのサポートの追加
* &amp;lbrack;Tool&amp;rbrack;ストローク不透明度のサポートを追加
* &amp;lbrack;Tool&amp;rbrack；最後のブラシストロークを継続させるモディファイヤを追加
* &amp;lbrack;Iray&amp;rbrack; Pascal GPUをサポートするためのアップデート
* &amp;lbrack;ビューポート&amp;rbrack; カラープロファイル(LUT)のサポートを追加
* &amp;lbrack;Substance&amp;rbrack；新しいフレームワークの統合(SD6エンジン)
* &amp;lbrack;UI&amp;rbrack;ファイルメニューの「最近使用したファイル」サイズリストを増やす
* &amp;lbrack；読み込み&amp;rbrack；読み込みダイアログでサブスタンスのカテゴリを使用して接頭辞を入力
* &amp;lbrack;ベイカー&amp;rbrack; 8K テクスチャのベイクを許可
* &amp;lbrack;ベイカー&amp;rbrack；非正方形の解像度のベイクを許可
* &amp;lbrack;ベイカー&amp;rbrack；重いハイポリメッシュをベイクする際のメモリ消費量を改善する
* &amp;lbrack;シェルフ&amp;rbrack；同時編集を禁止し、破損を防ぐためにシェルフ（およびプロジェクト）をロック
* &amp;lbrack;シェルフ&amp;rbrack;サブスタンスからカテゴリとキーワードを読み込み、フィルタリングに使用(&amp;lbrack;)
* &amp;lbrack;シェルフ&amp;rbrack；検索クエリの結果からリソースを除外できるようにします
* &amp;lbrack;シェルフ&amp;rbrack;サムネールの時間計算の向上
* &amp;lbrack;シェルフ&amp;rbrack;プロジェクトへのプリセットの埋め込みを許可
* &amp;lbrack;シェルフ&amp;rbrack; Shiftキーを押してツリービューをすばやく折りたたんだり展開できるようにします
* &amp;lbrack;シェルフ&amp;rbrack;アセットが読み取り専用の場合にサムネールを保存できるようにする（ローカルキャッシュ）
* &amp;lbrack;シェルフ&amp;rbrack；新規コンテンツ：新しいフィルター（変形、ミラー、トリ平面など）
* &amp;lbrack;シェルフ&amp;rbrack；新規コンテンツ：新しいLUTプロファイル（フィルムノワール、ビンテージなどのクラシックおよびアート）
* &amp;lbrack;シェルフ&amp;rbrack；新規コンテンツ:カスタムテキストを素早く生成するための10個の新しいフォントSubstance
* &amp;lbrack;シェルフ&amp;rbrack；新しいテンプレート: Unity 5およびUnreal エンジン 4
* &amp;lbrack;シェルフ&amp;rbrack; HSLフィルターが改善され、アーティストにとってより使いやすくなりました
* &amp;lbrack;シェーダー&amp;rbrack; PBRシェーダのSpecular levelチャンネルのサポートを追加
* &amp;lbrack;シェーダー&amp;rbrack; Alphaテストシェーダーのディザリングのサポートを追加
* &amp;lbrack;シェーダー&amp;rbrack; PBRシェーダでのパララックスオクルージョンマッピングのサポートを追加
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーパラメーターのカスタムUIを定義できます
* &amp;lbrack;MatLayering&amp;rbrack; マテリアルレイヤリングワークフロー用に新規マスクチャンネルを作成
* &amp;lbrack;Scripting&amp;rbrack; SPプロジェクトでのメタデータの書き込みを許可
* &amp;lbrack；スクリプト&amp;rbrack；特定の書き出しプリセットを使用して書き出すことができます
* &amp;lbrack;Scripting&amp;rbrack; シェーダーパラメーターをJSONとして取得できるようにします
* &amp;lbrack;Scripting&amp;rbrack; WebSocket接続のサポートを追加
* &amp;lbrack;Scripting&amp;rbrack; シェーダーインスタンスをロードする機能を追加
* &amp;lbrack;Scripting&amp;rbrack；新しいプロジェクトを作成する可能性を追加
* &amp;lbrack;Scripting&amp;rbrack;プロジェクトにインポートされたメッシュのURLを取得できるようにします
* &amp;lbrack；スクリプト&amp;rbrack；非正方形ベイク処理を許可
* &amp;lbrack；スクリプト&amp;rbrack;スクリプトAPIを介してデータを設定する際にエラーを報告
* &amp;lbrack;Substance&amp;rbrack; user-dataタグを追加して法線マップ形式を指定

**修正済み：**

* カラーとマテリアルを組み合わせる際のクラッシュ
* RGBA32f以外の画像を環境マップとして読み込むとクラッシュが発生します
* AMD GPUでのペイントに関連するクラッシュ
* &amp;lbrack;メッシュ&amp;rbrack; OBJの読み込みで、mtlファイルがないとマテリアルが認識されない
* &amp;lbrack;メッシュ&amp;rbrack；一部のメッシュでUDIMテクスチャセット名が正しく生成されない
* &amp;lbrack;UI&amp;rbrack；ビューアの取り消し/やり直しボタンでフォーカスを奪い、マウスのスクロールを停止を設定
* &amp;lbrack;UI&amp;rbrack；一部のラベルが高DPIで正しくトリミングされない
* &amp;lbrack；レイヤー&amp;rbrack; 「ペイント」エフェクトの置換モードがマスクで正しく動作しない
* &amp;lbrack；レイヤー&amp;rbrack; 減算描画モードでアルファが正しく機能しない
* &amp;lbrack;Tool&amp;rbrack; UV境界にペイントすると、2D ビューのブラシサイズが大きくなる
* &amp;lbrack;Tool&amp;rbrack;スナップした直線が高DPIで不安定な動作をする
* &amp;lbrack;Tool&amp;rbrack; ステンシルの解像度が正しくない場合がある
* &amp;lbrack;ベイカー&amp;rbrack; 「バウンディングボックスを基準にする」が「オフ」の場合、「最大オクルーダー距離」の値が固定される
* &amp;lbrack;シェーダー&amp;rbrack;スタックと自動パラメータチャンネルの定義が一致しません
* &amp;lbrack;3D ビュー&amp;rbrack;プロジェクト設定に応じて標準チャンネルの表示に一貫性がない
* &amp;lbrack;ビューポート&amp;rbrack；一部の法線マップは、クランプされた値を保持しており、斑点として表示されます
* &amp;lbrack;ビューポート&amp;rbrack;ポストエフェクトは、デフォルトでは常に無効になっています
* &amp;lbrack；書き出し&amp;rbrack；通常チャンネルが存在しない場合、通常のミキシング設定が正しくない
* &amp;lbrack；書き出し&amp;rbrack; AMD GPUでテクスチャが正しく生成されない場合がある
* &amp;lbrack;Export&amp;rbrack; シェーダーパラメータがグループ内にある場合、正しく書き出されない
* &amp;lbrack;Export&amp;rbrack;カスタムシェルフで書き出しプリセットを編集すると、ログエラーが出力される
* &amp;lbrack;シェルフ&amp;rbrack;ツリービューフィルタリングがフォルダ名と完全には一致しません
* &amp;lbrack;シェルフ&amp;rbrack; シェルフプリセットの名前を変更すると読みにくくなる
* &amp;lbrack;シェルフ&amp;rbrack; シェルフに読み込まれたシェーダーリソースが、再起動後に保持されない
* &amp;lbrack;シェルフ&amp;rbrack；内容：溶接ツールプリセットがありません
* &amp;lbrack;シェルフ&amp;rbrack;コンテンツ:Tile Generatorが正しく動作しない
* &amp;lbrack;シェルフ&amp;rbrack；内容：「ゴムタイヤの汚れ」スマートマテリアルのマスクが正しくない問題を修正
* &amp;lbrack;シェルフ&amp;rbrack;コンテンツ：レザーバッグマテリアルのグループ名が正しくありません
* &amp;lbrack;Iray&amp;rbrack;メッシュの半分がIrayにありません
* リソースを3D ビューの上にドラッグする際のLinux&amp;rbrack; クラッシュ(&amp;l)
* &amp;lbrack;Mac&amp;rbrack；環境設定は、Sierraで起動するたびにリセットされます。

**既知の問題：**

* &amp;lbrack；書き出し&amp;rbrack；非常にまれですが、AMD GPUで黒い長方形が表示されることがあります
* &amp;lbrack;Iray&amp;rbrack; カラープロファイルが奇妙な動作をすることがある

### 2.4.1

*（リリース：2016年10月28日）*

**修正済み：**

* テンプレートを使用したプロジェクトの作成時にクラッシュが発生する
* 書き出し中に書き出しダイアログを閉じるとクラッシュが発生する
* &amp;lbrack;Mac&amp;rbrack;プロジェクト保存時のエラー（書き出しプリセットの保存に失敗しました）
* &amp;lbrack;シェルフ&amp;rbrack；新規プリセットを作成すると、2回表示される
* &amp;lbrack;シェルフ&amp;rbrack;プリセットは、管理者権限がないと読み取り専用モードで読み込めません。

### 2.4.0

*（リリース：2016年10月27日）*

**追加：**

* &amp;lbrack;シェルフ&amp;rbrack；リソースを参照するための新しいインタフェース（ツリービュー、フィルタなど）
* &amp;lbrack;シェルフ&amp;rbrack；検索をプリセットとして保存できるようにします
* &amp;lbrack;シェルフ&amp;rbrack;プリセットから新しいウィンドウを作成できるようにします
* &amp;lbrack；リソース&amp;rbrack; シェルフを読み込むための新しいインタフェース
* &amp;lbrack;シェルフ&amp;rbrack;ドキュメントフォルダー内のデフォルトの寓意的シェルフをコピーしない
* &amp;lbrack;シェルフ&amp;rbrack；新規パーティクルプリセット: Electric Circuit, Electric Lines, Rococo, Veins Small
* &amp;lbrack;シェルフ&amp;rbrack；より使いやすい古いパーティクルプリセット（「雨」など）を改善
* &amp;lbrack;シェルフ&amp;rbrack;リソースコンテキストメニューに新しい情報を追加
* &amp;lbrack;ビューポート&amp;rbrack; 環境マップの読み込み時のパフォーマンスを向上
* &amp;lbrack;ビューポート&amp;rbrack; 2の累乗ではない環境マップのサポートを追加

**修正済み：**

* マスクを削除する際のクラッシュ
* プリセットを保存した後にペイントするとクラッシュが発生する
* 一部のGPUで環境ぼかしを使用するとクラッシュが発生する
* ミニシェルフで間違ったリソースを割り当てるとクラッシュが発生します
* &amp;lbrack;シェルフ&amp;rbrack; Clean + Saveプロジェクト内のリソースのタグとメタデータを削除
* &amp;lbrack;シェルフ&amp;rbrack;プリセットを読み込むと、そのリソースがシェルフに表示される
* Heightチャンネルから生成された書き出し&amp;rbrack;法線マップの輝度が低い(&amp;lbrack; Export&amp;rbrack;)
* &amp;lbrack；書き出し&amp;rbrack; メッシュから通常に書き出しが、最終法線マップに常に存在するとは限らない
* &amp;lbrack；書き出し&amp;rbrack；透明部分を含む拡張で透明部分が表示されないことがある
* &amp;lbrack;Scripting&amp;rbrack; &quot;alg.plugin_root_directory&quot;は、切り詰められたネットワークパスを返すことができます
* &amp;lbrack;TextureSet&amp;rbrack；非正方形プロジェクトを再度開くと、「ロック」ボタンが有効になる

### 2.3.1

*（リリース：2016年10月7日）*

**追加：**

* &amp;lbrack；プラグイン&amp;rbrack;&amp;lbrack;Photoshop&amp;rbrack；書き出すマテリアル/スタック/チャンネルを指定する
* &amp;lbrack;Scripting&amp;rbrack；関数名に矛盾があります

**修正済み：**

* &amp;lbrack;Export&amp;rbrack; Alphaは、カスタム書き出しプリセットで破棄できます
* &amp;lbrack;sRGBチャンネルで書き出し&amp;rbrack;Alphaが正しくガンマ変換されない
* &amp;lbrack；書き出し&amp;rbrack；非正方形ドキュメントは四角形として書き出されます
* &amp;lbrack;Export&amp;rbrack；追加のマップが見つからない場合、そのマップをエクスポートすることはできません。
* &amp;lbrack;Iray&amp;rbrack；一部のパラメーター（emissiveの適用度など）は無効
* NVIDIA Quadro K2200/GTX 750/760を使用すると、起動時にNVIDIA&amp;rbrack; クラッシュが発生する(&amp;lbrack;)
* &amp;lbrack;AMD&amp;rbrack;サムネールとプレビューのカラーのセットが正しくない
* &amp;lbrack;AMD&amp;rbrack；がフリーズし、新しいファイルを開くときにドライバが失敗する
* &amp;lbrack;Log&amp;rbrack; 「software-version」がログファイルにありません

### 2.3.0

*（リリース：2016年9月15日）*

**追加：**

* &amp;lbrack；プラグイン&amp;rbrack；新規「Photoshopに書き出し」プラグイン（書き出し完了レイヤースタック）
* &amp;lbrack;Export&amp;rbrack；余白の幅をピクセル単位または無限単位で指定できます。
* &amp;lbrack；書き出し&amp;rbrack; UVの外側の背景のタイプを設定できるようにします
* &amp;lbrack;シェルフ&amp;rbrack；新しいマテリアルレイヤーシェーダーを使用して10マテリアルをブレンド
* &amp;lbrack;シェルフ&amp;rbrack；新しいクレイシェーダーを使用して、Height/法線チャンネルで詳細を表示
* &amp;lbrack；環境&amp;rbrack;シェルフ入力を使用した新しいベイク照明フィルター
* &amp;lbrack;シェルフ&amp;rbrack；一部のマスクジェネレーターが更新され、非正方形の変換が追加されました
* &amp;lbrack;ビューポート&amp;rbrack；合成法線マップ（通常+Height+烘焙）をソロモードに追加
* &amp;lbrack；スクリプト&amp;rbrack；追加のマップのエクスポートを許可
* &amp;lbrack;Scripting&amp;rbrack；使用可能なクエリーを許可テクスチャセットごとの追加マップ
* &amp;lbrack;Scripting&amp;rbrack;チャネル形式の取得を許可
* &amp;lbrack;Scripting&amp;rbrack; Add examples in the ベイク documentation
* &amp;lbrack;Scripting&amp;rbrack;レイヤーの可視性を問い合わせることができます
* &amp;lbrack;Scripting&amp;rbrack;レイヤーの描画モードと不透明度を照会できるようにします
* &amp;lbrack;Scripting&amp;rbrack；変換されたマップ（最終法線マップ、混合AOなど）をエクスポートできるようにします。
* &amp;lbrack;Substance&amp;rbrack;カスタム使用状況の読み取りと接続
* &amp;lbrack；ショートカット&amp;rbrack；単独モードを逆方向に切り替えるための修飾キー(Shift)を追加
* &amp;lbrack；書き出し&amp;rbrack;アルファを無効にするデフォルトの書き出しプリセットの更新
* &amp;lbrack;UI&amp;rbrack;サムネールは、エンジンが使用可能な場合にのみ計算されるようになりました。
* &amp;lbrack;UI&amp;rbrack;サムネールの計算中にメンションを表示

**修正済み：**

* 一部の古いプロジェクトを開くとクラッシュが発生する
* テクスチャチャンネルキャッシュが破損しているクラッシュ
* マテリアルレイヤーワークフローで4つ以上のマテリアルをブレンドするとクラッシュが発生する
* ツールバーが非表示の場合にUI&amp;rbrack;ツールショートカットが機能しない(&amp;l)
* &amp;lbrack;UI&amp;rbrack; Irayツールバーは、ビューメニューで「名称未設定」とラベル付けされている
* &amp;lbrack;UI&amp;rbrack;プラグインのツールバーは、表示メニューで「Untillent」という名前になっています
* &amp;lbrack;ベイカー&amp;rbrack; 烘焙設定の編集中にEnterキーを押すと、ベイクプロセスが開始される
* &amp;lbrack;ベイカー&amp;rbrack；一部のパラメーターの範囲が正しくありません
* &amp;lbrack;Import&amp;rbrack；非常に大きな数字のため、OBJ メッシュをインポートできません
* &amp;lbrack；読み込み&amp;rbrack；読み込まれたOBJファイルのサブオブジェクトが多すぎます
* &amp;lbrack；書き出し&amp;rbrack;チャンネルの背景が、書き出し時にデフォルトカラーではなく黒で塗りつぶされる
* FOVが低すぎると&amp;lbrack;Tool&amp;rbrack; パーティクルが正しく動作しない
* &amp;lbrack;Tool&amp;rbrack;ブラシのプレビューカラーがサブスタック内のマスクで正しくない
* &amp;lbrack;ビューポート&amp;rbrack; 2D ビューの空き領域にブラシが入ると、巨大になります
* &amp;lbrack;ビューポート&amp;rbrack；標準テクスチャでペイントする際に空白のブラシがプレビューされる
* &amp;lbrack;Scripting&amp;rbrack;Incorrect documentation : &quot;ambientocclusion&quot;ではなく&quot;ao&quot;が表示される
* &amp;lbrack;Scripting&amp;rbrack; Process started with subprocess()がPainterの終了時に強制終了する
* &amp;lbrack;シェルフ&amp;rbrack;ベイク照明フィルタが誤ったAO入力を使用しています
* &amp;lbrack;MacOS&amp;rbrack；削除された消火栓プロジェクト（非互換）
* \*.sppファイルを読み込むときに（\*.sppファイルではなく）既定のプロジェクトが開く

**既知の問題：**

* &amp;lbrack;Plugin&amp;rbrack; Photoshopにより、Heightおよび通常チャンネルをそのまま移動できない

### 2.2.0

*（リリース：2016年7月22日）*

**追加：**

* &amp;lbrack;シェルフ&amp;rbrack；検索システムとクエリの改善
* &amp;lbrack;シェルフ&amp;rbrack;ミニシェルフの検索フィールドを追加
* &amp;lbrack;シェーダー&amp;rbrack;スライダーのステップ精度を定義できます
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーパラメータに[元に戻す/やり直し]ボタンを追加
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーを再読み込みしても、パラメータはリセットされません。
* &amp;lbrack;MatLayering&amp;rbrack; 動的マテリアルレイヤリングとサブスタックのサポートを追加
* &amp;lbrack;MatLayering&amp;rbrack; JSONファイルを読み込んでシェーダー設定を行えるようにします
* &amp;lbrack;MatLayering&amp;rbrack;テクスチャサンプラー制限のロック解除（バインドレステクスチャに切り替え）
* &amp;lbrack;Scripting&amp;rbrack; ベイカーの設定と計算の起動を許可する
* &amp;lbrack;Substance&amp;rbrack; 識別子に加えて入力/出力コネクションに「使用法」を使用
* &amp;lbrack;Tool&amp;rbrack;投影ツールのビューポートでプレビューチャンネルを選択できるようにします

**修正済み：**

* 物質が間違ったフォルダーに配置されている場合の起動時のクラッシュ
* ログファイルが正しくないために、クラッシュレポートが機能しない場合があります
* &amp;lbrack;Irayの一時停止時にIrayのポストエフェクトが更新されない(&amp;rbrack;)
* &amp;lbrack;Iray&amp;rbrack；自動焦点ショートカットが機能しない
* &amp;lbrack;Iray&amp;rbrack;アセットのサイズに応じてアパーチャスライダーの動作が変わる
* &amp;lbrack;Layers&amp;rbrack；最初のマテリアルチャンネルがすべて無効になっている場合、初期設定では有効になりません。
* &amp;lbrack;シェーダー&amp;rbrack; 「param auto」が正しくない場合、エラーは出力されません。

**既知の問題：**

* &amp;lbrack;Mac&amp;rbrack; テクスチャサンプル数の上限が16でロックされる（GPUドライバーの問題）

### 2.1.1

*（リリース：2016年7月1日）*

**追加：**

* &amp;lbrack;License&amp;rbrack;ライセンスファイルの場所を変更できます
* &amp;lbrack;ビューポート&amp;rbrack; 「B」ショートカットを追加して別のマップに切り替える
* &amp;lbrack;Import&amp;rbrack; FBX 2016/2017を正しくインポートできるようにします
* &amp;lbrack;Tool&amp;rbrack; クイックマスク使用時にチェックを外す
* &amp;lbrack;Iray&amp;rbrack; シーンの寸法情報を追加
* &amp;lbrack;Iray&amp;rbrack；サンプルの最大数とレンダリング時間を増やすことができます。
* &amp;lbrack;UI&amp;rbrack;スライダーで+/ – ボタンを使用すると結果をすぐに更新
* &amp;lbrack;UI&amp;rbrack;グレースケールスライダーの精度を向上
* &amp;lbrack;Export&amp;rbrack; RGBのみのテクスチャにアルファチャンネルを書き出さない
* &amp;lbrack；書き出し&amp;rbrack; Dota 2書き出しプリセットを更新
* &amp;lbrack;シェルフ&amp;rbrack；新規「六角形タイル」パターン
* &amp;lbrack;シェルフ&amp;rbrack；新規「溶接」ツール
* &amp;lbrack;シェルフ&amp;rbrack；方向コントロールを提供する仕上げフィルターを更新

**修正済み：**

* &amp;lbrack；書き出し&amp;rbrack; PSDファイルを8ビットで書き出すことはできません
* &amp;lbrack;Export&amp;rbrack; 8K exportは、一部のハードウェア構成では使用できません
* &amp;lbrack;Export&amp;rbrack; Sketchfabウィンドウがトリミングされている
* &amp;lbrack；書き出し&amp;rbrack；仕様/グロス書き出しプリセットのラフネスマップが正しくない
* &amp;lbrack;UI&amp;rbrack;グレースケールスライダーでの入力が機能しない
* &amp;lbrack;UI&amp;rbrack; GeneratorsなどのSubstance入力にフィルターを挿入できません。
* &amp;lbrack;UI&amp;rbrack；一部のスライダーのビヘイビアーが奇数
* &amp;lbrack;UI&amp;rbrack; DeltaTime +/- パーティクルのステップが大きすぎます
* &amp;lbrack;Iray&amp;rbrack; Irayに切り替えると、一部のプロジェクトでアプリケーションがブロックされる
* &amp;lbrack；ハードウェア検出時のIray&amp;rbrack; クラッシュ
* マスクモードでブラシのプレビューカラーが正しくない（&amp;lbrack；ツール&amp;rbrack;）
* &amp;lbrack;Tool&amp;rbrack; マテリアルピッカーは、互換性のないツールと共に使用できます
* &amp;lbrack;Tool&amp;rbrack; 投影プレビューがSpec/GlossワークフローのDiffuseに切り替わらない
* &amp;lbrack;シェルフ&amp;rbrack;デフォルトのシェーダーを変更すると、スマートマット/スマートマスクのプレビューが壊れる
* &amp;lbrack;シェルフ&amp;rbrack；一部のスマートマテリアルの名前が正しくない
* &amp;lbrack;シェルフ&amp;rbrack；その他のアルファシェイプが破損しているため、ロードされません
* &amp;lbrack;ビューポート&amp;rbrack; 「追加マップ」モードに切り替えると、「その他」が最初に表示される
* &amp;lbrack;ビューポート&amp;rbrack；追加のマップが存在しない場合、ビューポートを「その他」に切り替え
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;クラッシュレポートがUbuntu(Steam)で機能しない
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; Web URLリンクがUbuntu(Steam)で機能しない
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Substanceのpainterが実行されなくなったときに「crashwatcher」を削除
* &amp;lbrack;クラッシュ&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; クラッシュレポートシステムが正しく動作しない
* &amp;lbrack;クラッシュ&amp;rbrack; メッシュの読み込み中にメッシュを読み込むと、クラッシュが発生する
* 再起動後にテクスチャセット選択ショートカットがリセットされて何も表示されない

### 2.1.0

*（リリース：2016年6月2日）*

**追加：**

* &amp;lbrack;UDIM&amp;rbrack; メッシュからUDIM タイルをテクスチャセットとして読み込む
* &amp;lbrack;Linux&amp;rbrack; CentOS 6.6とUbuntu 12.4のサポートを追加
* &amp;lbrack；書き出し&amp;rbrack; 8K解像度を追加（試験的）
* &amp;lbrack;Export&amp;rbrack；書き出し時にビット深度を選択できるようにします
* &amp;lbrack;ベイカー&amp;rbrack；複数のテクスチャセットを一度にベイク可能
* 高解像度モニターのサポート（高DPIスケーリング）
* &amp;lbrack;Scripting&amp;rbrack；書き出し時にテクスチャごとにカスタム解像度とパディングを設定
* &amp;lbrack;ビューポート&amp;rbrack; メッシュをクリックしてテクスチャセットを切り替えることができます（Ctrl+Alt+クリック）
* &amp;lbrack;ビューポート&amp;rbrack;マウスホイールでズームするときにマウスカーソルがある場所に移動する
* &amp;lbrack;UI&amp;rbrack;デフォルトの背景色と環境マップ表示を更新
* &amp;lbrack;UI&amp;rbrack;ユーザチャネルの元の名前でツールチップを追加する
* &amp;lbrack;UI&amp;rbrack；名前を変更できないチャンネルの背景色を変更
* &amp;lbrack;Tool&amp;rbrack; クイックマスク使用時にチェックを外す
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーパラメーターとマテリアル/マスクのグループを定義できます
* &amp;lbrack;エンジン&amp;rbrack；小さいサイズのスタンプの最適化
* &amp;lbrack;ステンシル&amp;rbrack;マスクを一時的に切り替えるためのショートカットとして「W」を追加
* &amp;lbrack;シェルフ&amp;rbrack;クロスボタンを追加して検索フィールドをクリア
* &amp;lbrack;シェルフ&amp;rbrack;ワンクリックでAlphaをロード
* &amp;lbrack;シェルフ&amp;rbrack；新規書き出しプリセット: Vray UDIM、Arnold UDIM、メタル/粗さから仕様/光沢
* &amp;lbrack;シェルフ&amp;rbrack; New alpha ：幾何学的シェイプ、静脈、標識
* Substance Painterの実行可能ファイルのプロパティに名前とバージョンを追加する

**修正済み：**

* &amp;lbrack;Substance&amp;rbrack；通常チャンネルと追加マップを同時に使用することはできません
* &amp;lbrack;Iray&amp;rbrack; MDL屈折および吸収設定が機能しない
* &amp;lbrack;Iray&amp;rbrack；元のシーンスケールが保持されない
* &amp;lbrack;シェルフ&amp;rbrack; Specular/光沢度テンプレートが誤ったシェーダーを使用する
* &amp;lbrack；書き出し&amp;rbrack;デフォルトの書き出しプリセットで、一部のマップ（AOなど）が書き出されない
* &amp;lbrack;ビューポート&amp;rbrack;ピボットポイントが、2D ビュー内のUVの外側をクリックしても更新されない
* &amp;lbrack;UI&amp;rbrack;スライダーの値が丸められます
* &amp;lbrack;UI&amp;rbrack;スライダーの値を編集するときに、非常に小さな空き領域が存在することがあります
* &amp;lbrack;New Project&amp;rbrack; Templateドロップダウンリストが正しく更新されません（1.xから2.x）
* &amp;lbrack；スクリプト&amp;rbrack;カスタムボタンの「ホバー」動作を修正
* &amp;lbrack;Mac&amp;rbrack；空のプロジェクトで元に戻すとカメラがロックされる

**既知の問題：**

* クラッシュレポートはUbuntuでは利用できません
* 一部のurlボタンが機能しない場合があります。回避策については、FAQを参照してください

### 2.0.5

*（リリース：2016年4月29日）*

**追加：**

* &amp;lbrack;シェルフ&amp;rbrack; pbr以外のテンプレート、シェーダー、書き出しプリセットを追加/更新
* &amp;lbrack;シェルフ&amp;rbrack;Ambient occlusionを含めるようにUE4書き出しプリセットを更新

**修正済み：**

* 破損したリソースを含む一部のプロジェクトを開いて保存するときにクラッシュが発生する
* &amp;lbrack;ビューポート&amp;rbrack; ワイヤーフレームが2D ビュー内で壊れて表示される
* &amp;lbrack;シェルフ&amp;rbrack；一部のスタジオ環境マップのパフォーマンスを向上
* &amp;lbrack;シェルフ&amp;rbrack；一部のstudio 環境マップが複製されています
* &amp;lbrack;シェルフ&amp;rbrack; 「ベイク照明マテリアル」がありません
* &amp;lbrack;シェルフ&amp;rbrack; 「グレースケール変換」ジェネレータがありません

### 2.0.4

*（リリース：2016年4月26日）*

**追加：**

* メッシュのコリジョンの改善とワイヤーフレームレンダリングの最適化
* 大規模なプロジェクトでパフォーマンスとメモリ管理を向上
* スライダーの精度とステッピングの向上
* &amp;lbrack;UI&amp;rbrack; エンジンを検証するときのみ更新する（値を入力するときには更新しない）
* &amp;lbrack;UI&amp;rbrack; Irayスイッチをメインツールバーの専用ボタンに移動し、そのショートカットを変更する
* &amp;lbrack；ツール&amp;rbrack;クローンツールソースの位置動作の設定を追加
* &amp;lbrack;シェーダー&amp;rbrack;カスタムシェーダのメッシュ頂点の色を読み込むことができます
* &amp;lbrack;Scripting&amp;rbrack; テクスチャセット、チャンネル、レイヤーのリストを取得できるようにします
* &amp;lbrack;Scripting&amp;rbrack;パス関数を追加（urlからヘルパー、プロジェクトから書き出しパスを取得）
* &amp;lbrack;Mac&amp;rbrack;ログファイル内でMac Os「El Capitan」バージョンを検出

**修正済み：**

* Substance shareへの2回目の書き出し後のクラッシュ
* クイックマスクデータを含むテクスチャセット間でレイヤーをコピーするとクラッシュが発生します。
* 一部のプロジェクトには、大量のメモリを消費する非常に長いアップデーターがあります
* クローンツールまたは指先ツールでパーティクルプリセットを選択すると、&amp;lbrack；ツール&amp;rbrack; クラッシュが発生する
* &amp;lbrack;ベイカー&amp;rbrack; FBXファイルの読み込みに時間がかかり、大量のメッシュが発生する。
* &amp;lbrack;ビューポート&amp;rbrack；一部のコンピューターで環境マップを伸縮
* &amp;lbrack;ビューポート&amp;rbrack;ブラシのアルファのガンマ変換が正しくありません
* &amp;lbrack；書き出し&amp;rbrack;Alphaは、Tiffファイルを含む個別のチャンネルではなく、透明度として保存されます。
* &amp;lbrack;Export&amp;rbrack；通常チャンネルは常にOpenGLとしてエクスポートされます
* &amp;lbrack;Iray&amp;rbrack; Iray設定のスライダ名がありません
* &amp;lbrack;Iray&amp;rbrack;レンダリングがRetina/高DPIで間違った解像度で行われる
* &amp;lbrack;Irayモードでインターフェイスのサイズを変更すると、Iray&amp;rbrack; クラッシュが発生する
* &amp;lbrack;Iray&amp;rbrack；低解像度でのレンダリング時にパフォーマンスが大幅に低下する
* &amp;lbrack;Iray&amp;rbrack；一時停止が機能しない（Irayはバックグラウンドで計算されます）
* 通常のチャンネルに黒い正方形のアーティファクトが生じることがあります
* 法線チャンネルがグレースケールフィルターによって反転される
* スタックにアルファが含まれていると、通常のチャンネルが正しくブレンドされない
* プロジェクトを開くと、まだ保存されていなくても、ディスク上でプロジェクトが編集される
* 一部のプロジェクトでメッシュを再読み込みすると、GPUパフォーマンスが非常に低下する
* メッシュに触れていないと、ブラシの向きが正しくない
* ようこそ画面にSubstance shareのロゴが表示されない

### 2.0.2

*（リリース：2016年3月25日）*

**追加：**

* &amp;lbrack;Iray&amp;rbrack；仕様/グロステンプレートとシェーダーを更新してIrayと互換性を持たせる
* &amp;lbrack;Export&amp;rbrack;スクリーンショットをArtStationに書き出せる
* &amp;lbrack；スクリプト&amp;rbrack;プラグインディレクトリからの実行をサポート
* &amp;lbrack；スクリプト&amp;rbrack; 「別名で保存」を許可
* &amp;lbrack;UI&amp;rbrack；値を編集するスライダーをダブルクリックできるようにします
* VelaサンプルをSubstance shareに移動
* 新規サンプルプロジェクト：球プレビュー
* シェル拡張の競合についてユーザーに警告する

**修正済み：**

* インストーラーがSubstance Painter 1.xのインストールを上書きする
* &amp;lbrack;UI&amp;rbrack;チャンネルリストレイアウトがフィルターで壊れている
* &amp;lbrack;UI&amp;rbrack; シェーダーパラメータが表示されない
* &amp;lbrack;UI&amp;rbrack;レイヤーウィンドウのサイズを変更すると、コンテンツが正しく切り抜かれる
* &amp;lbrack;Tool&amp;rbrack；不透明度チャンネルが常に正しく使用されるとは限らない
* &amp;lbrack；ツール&amp;rbrack；指先/クローンが対称で機能しない
* &amp;lbrack;Tool&amp;rbrack; Brush preview opacity is incorrect with some channels
* Irayがまだ作成されていないときにIrayを使用すると、&amp;lbrack；データ&amp;rbrack;クラッシュが発生する。
* &amp;lbrack;Iray&amp;rbrack;プロジェクトから光線設定データを読み込めません
* &amp;lbrack;Iray&amp;rbrack; Irayが一時停止後に設定変更を処理しない
* &amp;lbrack;シェルフ&amp;rbrack; マテリアルのシェルフへの読み込みが機能しない
* ステンシルが通常チャンネルで機能しない
* 一部のプロジェクトでペイント中にクラッシュが発生する
* 一部のプロジェクトでパーティクルを使用してペイントするとクラッシュが発生する
* 一部の計算におけるピクセルプロセッサークラッシュ

### 2.0.0

*（リリース：2016年3月16日）*

**追加：**

* メインツールバーのSubstanceストアへのショートカット
* 表示モードとスクリーンショットの書き出しを備えたIrayレンダラー
* 「スマートマスク」の作成と使用のサポート
* Specular/光沢PBRワークフローのサポート（新しい拡散反射光チャンネルを使用）
* チェーンSubstance（物質をSubstance画像入力に差し込む）
* カスタムプラグインによるスクリプトのサポート
* Sobelフィルターを使用して、Heightから標準への変換を改善します
* ステンシル/投影のプレビュー解像度を2Kに切り替え
* 新規プロジェクトの標準チャンネルをデフォルトで追加
* 出力ノードからユーザーデータタグを読み込み、デフォルトでサブスタンスのチャンネルを有効/無効にする
* テクスチャセット設定で法線/AOブレンドを表示する
* &amp;lbrack；ツール&amp;rbrack;カラーをブレンドして広げる新しい指先ツール
* &amp;lbrack;Tool&amp;rbrack; テクスチャの一部をコピーするための新しいクローンツール
* &amp;lbrack;Tool&amp;rbrack；指先、クローン、消しゴムツールのチャンネルを選択できるようにする
* &amp;lbrack;Layer&amp;rbrack; Add Substance名for Fill effect name
* &amp;lbrack；レイヤー&amp;rbrack;マスクをクリップボードに書き出せる
* &amp;lbrack;ビューポート&amp;rbrack; 遠近法モードと正投影モードを切り替え
* &amp;lbrack;ビューポート&amp;rbrack; 遠近法モードで視野を制御できるようにします
* &amp;lbrack;ビューポート&amp;rbrack; Ctrl+中クリックでフィールドの距離の深度を設定できます
* &amp;lbrack;ビューポート&amp;rbrack; 3D ビュー内の環境マップをドラッグ&amp;ドロップできるようにします。
* &amp;lbrack;ビューポート&amp;rbrack; エンジンが強力な計算を行っている場合のフィードバックを改善
* &amp;lbrack;Export&amp;rbrack; JSONファイルにシェーダーパラメーターを書き出すことができます
* &amp;lbrack;UI&amp;rbrack；新しいアイコン、カラー、レイアウトでインターフェイスを更新
* &amp;lbrack;UI&amp;rbrack;ミニシェルフにアセット名を追加
* &amp;lbrack;UI&amp;rbrack;デフォルトで「チャンネルマッピング」を折りたたむ
* &amp;lbrack;シェーダー&amp;rbrack; シェーダーテクスチャパラメーターのカスタムカラーを選択
* &amp;lbrack；リソース&amp;rbrack; シェルフをドラッグアンドドロップするときに、ファイルのインポート先を確認する(&amp;R)
* &amp;lbrack;シェルフ&amp;rbrack; スマートマテリアルとジェネレータの新しいプレビュー球
* &amp;lbrack;シェルフ&amp;rbrack; Specular光沢度シェーダーを追加
* &amp;lbrack;シェルフ&amp;rbrack; New Hard Surface shapes
* &amp;lbrack;シェルフ&amp;rbrack；新しいAlphaテクスチャとシェイプ
* &amp;lbrack;シェルフ&amp;rbrack；新規スキンテクスチャ
* &amp;lbrack;シェルフ&amp;rbrack；新しいスキャンベースのマテリアルとスマートマテリアル
* &amp;lbrack;シェルフ&amp;rbrack；新しいスマートマテリアルと古いフォントの仕様/グロスのサポート
* &amp;lbrack;シェルフ&amp;rbrack;メタリックサーフェスシミュレーション用の新しい仕上げフィルタ
* &amp;lbrack;シェルフ&amp;rbrack；新しい強力なマスクジェネレーター「Mask Editor」
* &amp;lbrack;シェルフ&amp;rbrack；古いマテリアルを修正してクリーニングしました
* 新しい「Vela」サンプルプロジェクト

**修正済み：**

* &amp;lbrack；設定&amp;rbrack; カメラの回転とズーム速度はプロジェクトによって上書きされます
* &amp;lbrack;ビューポート&amp;rbrack;デフォルトの通常テクスチャでの精度の問題により、間違った反射が発生する
* &amp;lbrack;ビューポート&amp;rbrack;ビネットはデフォルトで有効になっています
* &amp;lbrack;ビューポート&amp;rbrack;アーティファクトが環境マップ境界(Nvidia GPU)に表示される
* 投影/ステンシルモードの&amp;lbrack;ビューポート&amp;rbrack；サムネールの読み込みに時間がかかる。
* &amp;lbrack;ベイカー&amp;rbrack;ベイクしたテクスチャを32ビットではなく16ビット整数で保存する
* &amp;lbrack;Layer&amp;rbrack；古いサブスタンスがスタックで正しく表示されない
* 一部のチャンネルのデフォルトカラーとビット深度が正しくない（Specular、光沢度など）
* パススルーモードで描画を無効にする消しゴムの動作を修正しました。

**既知の問題：**

* 指先ツールとクローンツールで対称が機能しない
* ArtStationの書き出しがありません

## バージョン1

### 1.7.3

*（リリース：2016年3月1日）*

**追加：**

* &amp;lbrack;Export&amp;rbrack;パディングを無効にするオプションを追加
* &amp;lbrack;シェルフ&amp;rbrack; シェルフフォルダ内のサブシェルフ階層をサポート

**修正済み：**

* 以前の読み取り専用ファイルを上書き保存するとクラッシュが発生する
* 2つ目のプロジェクトを開く際に発生するクラッシュ
* 一部のサムネール（シェルフ、レイヤー、ツールチップ）を読み込むときにクラッシュが発生する
* 「メッシュ時にストロークの位置を保持」を無効にしても機能しない
* &amp;lbrack；書き出し&amp;rbrack;ビットマップのアップスケールが最も近いフィルタリングで行われる
* &amp;lbrack;シェルフ&amp;rbrack;リソースの検出が非常に遅い
* &amp;lbrack;シェルフ&amp;rbrack；ぼかしフィルターは16ビット互換ではありません
* 古いツールプリセットをロードすると&amp;lbrack;Tool&amp;rbrack; 対称が機能しない
* Specularチャンネルのカラーダイアログでカラースペースが変換されない

### 1.7.2

*（リリース：2016年1月13日）*

**追加：**

* &amp;lbrack；レイヤー&amp;rbrack; 塗りつぶしレイヤーのデフォルトのタイリングを許可

**修正済み：**

* &amp;lbrack；書き出し&amp;rbrack; Sketchfabの書き出しが機能しない
* &amp;lbrack;Layer&amp;rbrack;フィルタリングは、変形なしで塗りつぶしに対しても適用されます。
* &amp;lbrack;Tool&amp;rbrack; 投影モードでSubstanceと画像入力を使用するとパフォーマンスが低下する
* &amp;lbrack;Tool&amp;rbrack; マテリアルピッカーが壊れています

### 1.7.1

*（リリース：2015年12月18日）*

**修正済み：**

* テクスチャセット切り替え時のクラッシュ
* ペイント時のパフォーマンスの低下

### 1.7.0

*（リリース：2015年12月17日）*

**追加：**

* &amp;lbrack；パフォーマンス&amp;rbrack;レイヤーコンテンツとそのサムネールを同時に計算
* &amp;lbrack；書き出し&amp;rbrack;プロジェクトの横に書き出しパスを相対パスとして保存
* &amp;lbrack；レイヤー&amp;rbrack；新しい描画モードを追加：削除および追加/サブ
* &amp;lbrack;Layers&amp;rbrack; 塗りつぶしレイヤーの新しいバイリニアHQ フィルタリング
* &amp;lbrack;シェーダー&amp;rbrack；環境設定でサムネール生成用のデフォルトシェーダーを設定します。
* &amp;lbrack;シェーダー&amp;rbrack; テクスチャセットごとにシェーダーを指定できるようにします
* &amp;lbrack;シェーダー&amp;rbrack; シェルフからテクスチャをサンプリングできるようにします
* &amp;lbrack；ツール&amp;rbrack;ペイント用の新しい「ラップ」ブラシ動作
* &amp;lbrack;Tool&amp;rbrack;ペイント時のフィルタリングの改善とエイリアスの削減
* &amp;lbrack；ツール&amp;rbrack;サブピクセルのペイント品質を向上
* &amp;lbrack;Tool&amp;rbrack;ブラシ設定の「基本」表示を削除し、フレームを開く/閉じるアイコンを改善
* &amp;lbrack;Menu&amp;rbrack；右クリックメニューにエフェクトアイコンを追加
* プロジェクトからのテンプレートの作成
* &amp;lbrack;シェルフ&amp;rbrack；新規テンプレート: PBR、Dota 2
* &amp;lbrack;シェルフ&amp;rbrack；新規書き出しプリセット: Dota 2
* &amp;lbrack;シェルフ&amp;rbrack；新規シェーダ: Dota 2、PBR Car ペイント、PBR Coated、PBR Velvet
* &amp;lbrack;シェルフ&amp;rbrack；新規マテリアル ：鉄鋼の錆と摩耗、スタイライズされた照明
* &amp;lbrack;シェルフ&amp;rbrack；新しいフィルター：ぼかし方向、スタイライズされた照明
* &amp;lbrack;シェルフ&amp;rbrack；新規ブラシ：デフォルトのソフトとデフォルトのハードを、新しいアルファを使用して硬さコントロールを向上させた状態にします。
* &amp;lbrack;シェルフ&amp;rbrack；新しいジェネレータ: 3D距離とライト
* &amp;lbrack;シェルフ&amp;rbrack;ラップ投影とバックフェースカリングを使用して更新されたブラシ（デフォルトで有効）
* &amp;lbrack;シェルフ&amp;rbrack；より高速な計算を実現するために、ホワイトノイズをピクセルプロセッサーバージョンに更新

**修正済み：**

* &amp;lbrack；ようこそ画面&amp;rbrack;Tutorialsリンクが古いビデオに送信されます。
* &amp;lbrack;Channels&amp;rbrack; AOを使用した塗りつぶしレイヤー作成に「いいえ」と言ってもレイヤーは作成される
* &amp;lbrack；チャネル&amp;rbrack; UserXチャネル名がインターフェイスに伝搬されない
* &amp;lbrack;ビューポート&amp;rbrack;ソロチャンネルのリストでマスクエントリが空です
* &amp;lbrack;Share&amp;rbrack;アルファをSPから共有に書き出すと、読み取り不可能な.imageファイルが作成される
* &amp;lbrack;License&amp;rbrack；非ASCII文字を含むユーザー名のアクティベーションを修正
* &amp;lbrack;シェーダー&amp;rbrack;カラーを選択すると、カラーパラメーターダイアログが消える
* &amp;lbrack;シェルフ&amp;rbrack;サムネールが未使用の場合、メモリからアンロードされない
* &amp;lbrack;シェルフ&amp;rbrack；固定グラデーションフィルター
* &amp;lbrack;Tool&amp;rbrack; 対称がステンシル/投影で機能しない
* &amp;lbrack;Tool&amp;rbrack；新規ブラシプリセット作成時の名前が間違っています
* 「線を保持」設定は、メッシュを再読み込みする場合でも無効のままです
* 大きなサイズのパーティクルを計算する場合のドライバリセット(TDR)。

### 1.6.1

*（リリース：2015年11月9日）*

**修正済み：**

* 2D ビューが表示されている場合にプロジェクトを開くとクラッシュが発生する
* 現在のシェルフが存在しない場合、新しい書き出しプリセットを作成するとクラッシュが発生する
* &amp;lbrack;Tool&amp;rbrack; マテリアルピッカーアイコンの表示を維持
* &amp;lbrack;Tool&amp;rbrack; マテリアルピッカーで同時にペイントすると、マウスカーソルが非表示になる
* &amp;lbrack;シェルフ&amp;rbrack;メタデータは、終了するたびにディスクに書き込まれます

### 1.6.0

*（リリース：2015年10月29日）*

**追加：**

* Windows 10の公式サポート
* &amp;lbrack;Substance&amp;rbrack; Substanceパラメータグループをデフォルトで折りたたむ
* &amp;lbrack;Substance&amp;rbrack；新しいフレームワークを追加（ピクセルプロセッサーのパフォーマンスを向上）
* &amp;lbrack;ビューポート&amp;rbrack; 対称モードで対称プレーン表示をディアクティベートできるようにします。
* &amp;lbrack;ビューポート&amp;rbrack;シャドウのレンダリングとパフォーマンスの向上
* &amp;lbrack;ビューポート&amp;rbrack；描画時にシャドウ計算を一時停止
* &amp;lbrack;ビューポート&amp;rbrack; ワイヤーフレームレンダリングのパフォーマンスを向上させる
* &amp;lbrack;エンジン&amp;rbrack; Vramメモリ管理を改善してフットプリントを削減
* &amp;lbrack;エンジン&amp;rbrack; AMD GPUのテクスチャ更新を改善してパフォーマンスを向上
* &amp;lbrack;エンジン&amp;rbrack; NVIDIA GPUのスレッド最適化設定を無効にして、パフォーマンスを向上させる(&amp;L)
* &amp;lbrack;Effect&amp;rbrack;タグを追加して「埋め込まれた」画像入力を要求
* &amp;lbrack；レイヤー&amp;rbrack；塗りつぶしのUV オフセット/拡大・縮小の精度を上げる
* &amp;lbrack;Layer&amp;rbrack；塗りつぶしでスケールスライダーを指数にします
* &amp;lbrack;Layer&amp;rbrack; マテリアルをレイヤースタックに直接ドラッグ&amp;ドロップできます。
* &amp;lbrack;Layer&amp;rbrack;フィルターをレイヤースタックに直接ドラッグ&amp;ドロップできます
* &amp;lbrack；レイヤー&amp;rbrack;マスクブラシのカラーを新しく作成されたマスクカラーに調整する
* &amp;lbrack;シェーダー&amp;rbrack；複数のテキストコードを表示
* &amp;lbrack;シェーダー&amp;rbrack;カスタム関数を使用するためのガンマ/トネマッピング関数の表示
* &amp;lbrack;ベイカー&amp;rbrack; TriPlanar使用時のデフォルトの位置ベイカー設定を変更
* &amp;lbrack;Tool&amp;rbrack; 「ジオメトリデカール」を「ポリゴンフィル」に名前変更
* &amp;lbrack;シェルフ&amp;rbrack; TriPlanarをサポートするようにジェネレータを更新： MG Metal edge wear, MG Mask builder, MG Fiber glass, MG Glass
* &amp;lbrack;シェルフ&amp;rbrack；新しいマテリアルでマテリアルを更新し、使用されていない設定を削除する
* &amp;lbrack;シェルフ&amp;rbrack; 22の新しいスマートマテリアル （プラスチック、鉄、布地、鉄鋼など）
* &amp;lbrack;シェルフ&amp;rbrack;シームを避けるために、画像の入力を埋め込んで、シャープ、ぼかし、ワープフィルターを更新
* &amp;lbrack;シェルフ&amp;rbrack;ワープ設定を改善して使いやすくする
* &amp;lbrack;シェルフ&amp;rbrack; 2つの新しいプロシージャルノイズ : 3Dパーリンノイズと3Dワーリーノイズ

**修正済み：**

* Macで、専用GPUのVRAM量検出が正しく行われない(&amp;lbrack;エンジン&amp;rbrack;)
* &amp;lbrack;エンジン&amp;rbrack; テクスチャがビューポート内で暗いバージョンに変わる(&amp;rbrack;)
* &amp;lbrack;エンジン&amp;rbrack；複数のレイヤーの下にペイントするとパフォーマンスが低下する(&amp;R)
* &amp;lbrack;エンジン&amp;rbrack;プロジェクトを開いたときに計算されたレイヤーがキャッシュされたバージョンと異なる
* Macで&amp;lbrack;Substance&amp;rbrack；の結果が4Kになる間違い
* &amp;lbrack;Substance&amp;rbrack;パラメータの順番が間違っています
* &amp;lbrack;シェーダー&amp;rbrack;トーンシェーダとピクセル化されたシェーダが完全に黒くなる
* &amp;lbrack;シェーダー&amp;rbrack; env-mapの変更後にパラメータが消える
* pngファイルをgeneratorフォルダーに入れるときにクラッシュが発生する&amp;lbrack;シェルフ&amp;rbrack;
* &amp;lbrack;シェルフ&amp;rbrack;サムネールが低ラフネスで生成される
* Windowsでブラシアルファにビットマップを使用すると、&amp;lbrack;Tool&amp;rbrack;クラッシュが発生する。
* &amp;lbrack;Export&amp;rbrack；追加のマップ書き出しプリセットが位置用のRGBマップを書き出すようになりました

### 1.5.7

*（リリース：2015年9月24日）*

**修正済み：**

* クラッシュレポートが機能しない

### 1.5.6

*（リリース：2015年9月21日）*

**追加：**

* &amp;lbrack；サムネール&amp;rbrack; シェルフのレンダリング品質を向上（1K テクスチャを使用）

**修正済み：**

* &amp;lbrack;Share&amp;rbrack；別のアカウントで署名することはできません
* &amp;lbrack;シェルフ&amp;rbrack;サムネールがディスク上で重すぎます
* &amp;lbrack;シェルフ&amp;rbrack; スマートマテリアルの読み込みが非常に遅い
* &amp;lbrack;Windows&amp;rbrack;ライセンスサービスのインストールを修正
* &amp;lbrack；チャンネル&amp;rbrack; Transmissiveマップは、デフォルトではG8として作成されます。

### 1.5.5

*（リリース：2015年9月15日）*

**追加：**

* &amp;lbrack;シェルフ&amp;rbrack;アセットをSubstance shareにエクスポート
* &amp;lbrack;シェルフ&amp;rbrack; マテリアルの新しい球プレビューを追加
* &amp;lbrack;シェルフ&amp;rbrack;サムネールの生成に環境マップ「ガラスのパティオ」を使用
* &amp;lbrack;シェルフ&amp;rbrack;サムネールサイズの解像度を512 x 512ピクセルに上げる
* &amp;lbrack;3D ビュー&amp;rbrack；環境回転値の表示
* &amp;lbrack;Windows&amp;rbrack;アプリケーションに署名

**修正済み：**

* &amp;lbrack;ベイカー&amp;rbrack；同時にマップをベイクすると間違った結果になる
* &amp;lbrack;3D ビュー&amp;rbrack;プロジェクトが開かれていない場合、環境マップが表示されます
* &amp;lbrack;Layers&amp;rbrack; マスクジェネレーターがレイヤーコンテンツで機能しない
* &amp;lbrack；画層&amp;rbrack；非表示の画層にペイントを設定できます
* &amp;lbrack;シェルフ&amp;rbrack;Dirt_5とDirt_6 ノイズが同一です
* &amp;lbrack;シェルフ&amp;rbrack；一部のマスクジェネレーターはピクセル化されているか低画質です
* &amp;lbrack;Tool&amp;rbrack；特定の角度でギズモが正しく回転しません。
* &amp;lbrack;Tool&amp;rbrack;チャンネルが多すぎると、チャンネルボタンが切り抜かれます。
* &amp;lbrack;Tool&amp;rbrack; クイックマスクのマスクショートカットを反転が機能しない
* &amp;lbrack;Export&amp;rbrack; Sketchfab:キャンセルボタンが正しく考慮されません
* &amp;lbrack;License&amp;rbrack;ライセンスをコピーできないときにアクティベーションに失敗しました
* フレームレートのリミッターがUIで機能しない

### 1.5.0

*（リリース：2015年8月20日）*

**追加：**

* &amp;lbrack;シェーダー&amp;rbrack; シェーダーコンパイルエラーメッセージに行番号を追加
* &amp;lbrack;シェルフ&amp;rbrack;サムネールのプレビュー画質を向上
* &amp;lbrack;シェルフ&amp;rbrack; スマートマテリアルのサムネール生成を自動化
* &amp;lbrack;Tool&amp;rbrack; substanceの硬さ設定を制御するためのショートカット
* &amp;lbrack；ツール&amp;rbrack;マスク上でジオメトリデカールにグレースケールウィジェットを使用
* &amp;lbrack;Tool&amp;rbrack;グレースケールマップでペイントする際にペイントの色を反転するショートカット
* &amp;lbrack;ビューポート&amp;rbrack; ワイヤーフレームの表示と色の変更を許可する
* &amp;lbrack;ビューポート&amp;rbrack；環境の背景をぼかす
* &amp;lbrack；コントロール&amp;rbrack;ブラシマウスショートカットに回転を追加
* &amp;lbrack；エクスポート&amp;rbrack; Sketchfabにエクスポート
* &amp;lbrack;Export&amp;rbrack;レンダラーの書き出しプリセットを作成
* &amp;lbrack；書き出し&amp;rbrack；変換されたマップ反射、F0および1/IORを追加
* &amp;lbrack;UI&amp;rbrack；ようこそ画面を追加
* &amp;lbrack;UI&amp;rbrack；既定のレイアウトを更新
* &amp;lbrack;UI&amp;rbrack；見つからないツールチップを追加し、一部のメニュー項目の名前を変更
* &amp;lbrack；レイヤー&amp;rbrack；現在選択されているマスクをビットマップとして書き出し
* &amp;lbrack;Layers&amp;rbrack；右クリックメニューに「マスクを反転」アクションを追加

**修正済み：**

* &amp;lbrack;Project&amp;rbrack; FBXでメッシュピボットが異なる場合、読み込み時にメッシュが展開される
* 投影ツールで使用されるSubstanceが256\*256でロックされている(&amp;lbrack;Substance&amp;rbrack;)
* &amp;lbrack;Layers&amp;rbrack; clear mask使用時のクラッシュ
* &amp;lbrack；書き出し&amp;rbrack；非常に暗いテクスチャでガンマ変換が正しく行われない
* &amp;lbrack;Export&amp;rbrack; Position mapは、書き出しプリセットでグレースケールマップとしてのみ使用できます
* &amp;lbrack;Tool&amp;rbrack; Geometryデカールの開始色がマスクで使用されると黒くなる
* &amp;lbrack;Tool&amp;rbrack；回転ショートカットが、アルファに硬さがない場合に機能しない

### 1.4.2

*（リリース：2015年7月15日）*

**修正済み：**

* &amp;lbrack；ジオメトリデカールとクイックマスクを使用する際のツール&amp;rbrack;クラッシュ
* プロジェクトを1.4.0から1.4.1に更新すると、すべてのコンピューターメモリが消費されます
* 古いプロジェクト形式が正しく読み込まれない
* カスタムシェルフは階層全体を解析し、アセットをどこにでも複製します

### 1.4.1

*（リリース：2015年6月23日）*

**追加：**

* &amp;lbrack;ビューポート&amp;rbrack;パネルを並べてドッキングできるようにします
* &amp;lbrack;Effect&amp;rbrack;レベルエフェクトの背景と定規を追加
* &amp;lbrack;Effect&amp;rbrack；他のエフェクトを処理できるペイントエフェクトを追加する

**修正済み：**

* &amp;lbrack;シェルフ&amp;rbrack;プロジェクトが開かれていない場合、サムネールの生成が壊れる
* &amp;lbrack;シェルフ&amp;rbrack;マテリアルプリセットプレビューが生成されない
* &amp;lbrack;シェルフ&amp;rbrack;マテリアルプレビューは、法線が反転したメッシュ上に生成される
* &amp;lbrack;シェルフ&amp;rbrack;サムネールは、不正なハッシュ関数のために常に再計算されます。
* &amp;lbrack;シェルフ&amp;rbrack; Substance マテリアルをクリックしても他のマップに接続されない
* &amp;lbrack;Tool&amp;rbrack; マテリアルピッカーでサンプリングした値が正しくない
* &amp;lbrack;Tool&amp;rbrack;カラーピッカーでビューポートカーソルの色を選択
* &amp;lbrack;2D ビュー&amp;rbrack；非常に低いフレームレート/パフォーマンス
* &amp;lbrack；書き出しウィンドウを開いたときに、最近使用した書き出しプリセットが原因で&amp;rbrack；書き出し&amp;rbrack;クラッシュが発生する。
* &amp;lbrack；書き出し&amp;rbrack;Heightチャンネルから法線マップへの変換が間違ったスペースに変換される
* &amp;lbrack;Mac&amp;rbrack; SubstanceエフェクトのBaseColorは、リニアとして表示されます
* &amp;lbrack;Mac&amp;rbrack；直線ウィジェットがRetinaで正しく描画されない
* 直線は、ショートカットを放しても有効のままになります。
* 環境マップを回転すると直線ギズモが消える
* サブスタンスからのAmbient occlusion出力は、AOチャンネルに自動的に接続されません
* ユーザー名に特殊文字が含まれているwindowsでのライセンスコピーの問題を修正

### 1.4.0

*（リリース：2015年6月10日）*

**追加：**

* &amp;lbrack;Export&amp;rbrack；使用可能な入力マップのリストにマップを追加
* &amp;lbrack;シェルフ&amp;rbrack; sbsar マテリアルをマテリアルプリセットとして使用
* &amp;lbrack;シェルフ&amp;rbrack;カスタムライブラリパスの使用を許可
* &amp;lbrack;シェルフ&amp;rbrack；最小サイズを変更
* &amp;lbrack;シェルフ&amp;rbrack；新規コンテンツ: 20個の新規スマートマテリアル
* &amp;lbrack;シェルフ&amp;rbrack；新規コンテンツ：新規プロシージャル物質（織り、メッシュ）
* &amp;lbrack;シェルフ&amp;rbrack；更新されたぼかしフィルター
* 修飾キーを使用した直線の描画
* ambient occlusionチャンネルを追加し、レイヤースタックでアオ/通常のビヘイビアーを再調整
* Substanceユーザーデータで定義された画像入力からデフォルトカラーを読み取る
* ヘルプメニューからログの書き出しを許可

**修正済み：**

* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; メッシュベイカーから通常にクラッシュ
* &amp;lbrack;ケージファイルにUVがない場合にベイカー&amp;rbrack;クラッシュ
* &amp;lbrack;ベイカー&amp;rbrack；名前による一致が、zBrushから書き出したOBJで機能しない
* &amp;lbrack；複数のテクスチャセットを使用し、UVをオーバーラップしている場合、ケージを使用したベイクによって烘焙が上書きされる&amp;rbrack; ベイカー&amp;rbrack;
* &amp;lbrack;ベイカー&amp;rbrack；特定のOBJファイルで黒いテクスチャが表示される
* &amp;lbrack;シェルフ&amp;rbrack；読み取り専用に設定されている場合、リソースを読み取れません
* &amp;lbrack;シェルフ&amp;rbrack;アセットファイルがプロジェクトで使用されている場合、そのファイルはPainterで書き込まれています。
* &amp;lbrack;シェルフ&amp;rbrack;サブスタンスの再読み込みでもレイヤーが更新される
* &amp;lbrack;Export&amp;rbrack; Tiffは、Photoshopやゲームエンジンで正しく読み取れない32 bitの画像を書き出します
* &amp;lbrack;Export&amp;rbrack;デフォルトチャンネルプリセットは常にRGBとして書き出される
* &amp;lbrack;マテリアル&amp;rbrack; DiffuseチャンネルがBaseColorマッピングをサブスタンスで上書き(&amp;r)
* &amp;lbrack;3D ビュー&amp;rbrack；特定の環境マップでDiffuseが正しく照らされない。
* &amp;lbrack;Tool&amp;rbrack;ブラシを特定の角度に回転できません
* テキストフィールドへの入力中にビューポートにカーソルを合わせると、フォーカスが移動する
* プリセットを含むクラッシュがシェルフの現在のバージョンに対して新しすぎる
* メッシュ交換後のクラッシュ
* 入力の数が異なるサブスタンスをリロードするとクラッシュが発生する
* Cinema4DからのFBX メッシュが間違ったマテリアル名で読み込まれる

### 1.3.5

*（リリース：2015年5月29日）*

**追加：**

* 既存のライセンスファイルがある場合に&amp;lbrack;License&amp;rbrack;アクティベーションの問題
* &amp;lbrack；特定のFBXファイルを読み込むときのMac&amp;rbrack; クラッシュ
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;3D ビュー&amp;rbrack；統合GPUの誤ったリフレクション
* &amp;lbrack;3D ビュー&amp;rbrack; クイックマスクフォントが壊れています
* &amp;lbrack;3D ビュー&amp;rbrack; マテリアルピッカーでビューポートを真っ黒にする(&amp;r)
* 1.3.3で作成したプロジェクトを開くとクラッシュが発生する
* アルファ付きのシェーダを使用すると、マテリアルプレビューが空になる
* 特定のメッシュでペイントが機能しない
* OBJのメッシュによっては、パフォーマンスが大幅に低下する
* エフェクトの使用時にユーザーチャンネルがマッピングされない
* 一時フォルダーが起動時にクリーンアップされない

**修正済み：**

* プロジェクトの読み込みに非常に時間がかかる計算時間の短縮
* 「GPUトラブルシューティング」ウィンドウをわかりやすいように変更します。
* &amp;lbrack;Layers&amp;rbrack; 塗りつぶしレイヤーの縦横比ロックのステータスを保存し、デフォルトで「オン」にします
* &amp;lbrack;ベイカー&amp;rbrack；名前による一致で区切り文字として接尾辞を使用するようになりました

### 1.3.4

*（リリース：2015年4月27日）*

**追加：**

* Mac OS X Yosemite (10.10)とのMacのクラッシュ(&amp;lbrack;&amp;rbrack)
* &amp;lbrack;Mac&amp;rbrack;フルスクリーンモードを終了できません
* &amp;lbrack;ベイカー&amp;rbrack；名前で一致をベイクオプションが機能しない
* &amp;lbrack;ベイカー&amp;rbrack; SPで使用されているMikk 正接スペースがUE4で機能しない
* &amp;lbrack;ベイカー&amp;rbrack; ID ベイカーがマテリアル IDカラーをベイクできない
* &amp;lbrack;2D ビュー&amp;rbrack; ワイヤーフレームがジオメトリデカールツール使用時に表示されない
* &amp;lbrack;Tool&amp;rbrack;ブラシアルファチャンネルが、マテリアル付きの透明度ではなくチェッカーとして表示される
* &amp;lbrack;Tool&amp;rbrack; クラッシュとジオメトリデカール
* &amp;lbrack;Layers&amp;rbrack; マテリアルスロットが塗りつぶしレイヤー時にデフォルトで折りたたまれます
* &amp;lbrack;テクスチャセット解像度より高いサイズで書き出すと、書き出し&amp;rbrack;クラッシュが発生する
* Specularチャンネルがフィルターで認識されません。
* クリーン+保存で、sppアーカイブからリソースが正しく削除されない
* ローポリゴン変換をハイポリゴンのアッシンべンファイルに保存しない
* 読み込まれたFBXファイルのテクスチャセット数が多すぎます

**修正済み：**

* 効果：「クラシック」レベルを模倣するには、「クランプレベル」がデフォルトでオンになっている必要があります
* レイヤー：塗りつぶしアクションでタイリングの最小値と最大値を変更
* レイヤー：スタックステータスの保存と復元
* ベイカー:HPが指定されていない場合は、AO ベイカーが法線マップを考慮します。
* ベイカー:ベイク処理ウィンドウにツールチップと詳細情報が追加されました
* プロジェクト保存時のバックアップファイルの作成

### 1.3.3

*（リリース：2015年4月1日）*

**追加：**

* タイトルバーへのソフトウェアバージョンとプロジェクト名の追加
* テクスチャセット名とスマートマテリアル名をサニタイズ
* エンジンをV5に更新
* &amp;lbrack;シェルフ&amp;rbrack；新しい環境マップを追加： Corsica beach, studio 05, Tornoco studioなど
* &amp;lbrack;シェルフ&amp;rbrack; MGマスクビルダを新しいパラメータで更新する
* &amp;lbrack;シェルフ&amp;rbrack；古い環境マップの更新とキャリブレーション

**修正済み：**

* 書き出しウィンドウを開く際のクラッシュ
* ドッキングを解除するとUIウィジェットをドラッグ&amp;ドロップできない
* 「アップデートの有無をチェック」が機能しない
* &amp;lbrack；レイヤー&amp;rbrack; Altキーを押しながらクリックしてもマスクを選択しない
* &amp;lbrack;Tool&amp;rbrack; Tri-平面が通常チャンネルで機能しない
* &amp;lbrack;3D ビュー&amp;rbrack；環境マップからのDiffuse照明が正しくない
* &amp;lbrack;3D ビュー&amp;rbrack；露光量計算がDesignerと異なる
* &amp;lbrack;3D ビュー&amp;rbrack；影が100%メタリックサーフェス上に表示されない
* &amp;lbrack;3D ビュー&amp;rbrack;ミラーされたUVを持つメッシュが正接/バイノマルを反転しました
* &amp;lbrack;3D ビュー&amp;rbrack;シャドウが特定のメッシュで不正確な結果を生成する
* &amp;lbrack;ベイカー&amp;rbrack; assbinファイルによって作成された「.alg_meta」フォルダを削除
* &amp;lbrack;ベイカー&amp;rbrack; PainterがTextureSetを同時に再計算する場合のベイク時のクラッシュ
* &amp;lbrack;Mac&amp;rbrack;アプリケーション起動時のホワイトボックスUIの不具合

### 1.3.2

*（リリース：2015年3月6日）*

**修正済み：**

* &amp;lbrack;3D ビュー&amp;rbrack;プロジェクトとともに保存されたenvマップを再ロードできない

### 1.3.1

*（リリース：2015年3月5日）*

**追加：**

* &amp;lbrack;ベイカー&amp;rbrack;キャッシュされたhigh-poly メッシュを追加して計算を高速化する
* &amp;lbrack;ベイカー&amp;rbrack；高ポリゴンメッシュがロードされていない場合に警告アイコンを表示
* &amp;lbrack;ベイカー&amp;rbrack; high-poly メッシュがロードされていない場合は、代わりにプロジェクトメッシュを使用します

**修正済み：**

* &amp;lbrack;ベイカー&amp;rbrack;スライダの値を編集する際に「Enter」を押すとウィンドウが閉じる
* &amp;lbrack;ベイカー&amp;rbrack;ボタンの有効化/無効化もベイカーをトリガーします。
* &amp;lbrack;ベイカー&amp;rbrack; 「all/none」ボタンを使用するとベイクできません
* &amp;lbrack;ベイカー&amp;rbrack; ベイカーボタンの並べ替えが正しい順序ではありません
* &amp;lbrack;ベイカー&amp;rbrack;チェックボックスは無視され、すべてのベイカーが常に処理されます。
* &amp;lbrack;ベイカー&amp;rbrack；進行状況バーの進行状況を固定

### 1.3.0

*（リリース：2015年3月4日）*

**追加：**

* &amp;lbrack;ベイカー&amp;rbrack;&amp;lbrack;3D ビュー&amp;rbrack;正接/従法線が見つからない場合はMikkkt 正接空間計算を使用
* &amp;lbrack;ベイカー&amp;rbrack；新しいベイカーを追加：通常、ID、オクルージョン、曲率、Thickness、配置
* &amp;lbrack;Effects&amp;rbrack;エフェクトスタックが反転され、上から下に表示されるようになりました（レイヤーと同様）
* &amp;lbrack；エフェクト&amp;rbrack;エフェクトスタックに新しいアイコンを追加
* &amp;lbrack；エフェクト&amp;rbrack;エフェクトスタックで塗りつぶしアクション間に描画モードを追加
* &amp;lbrack；エフェクト&amp;rbrack;エフェクト名を変更（substance effect = filterなど）
* 保存プロセス中に「ロック」ファイルを追加
* &amp;lbrack；エフェクト&amp;rbrack;エフェクトスタックに塗りつぶしアクションを追加
* 新しいリソースを追加：スマートマテリアル
* &amp;lbrack;Layers&amp;rbrack;レイヤーエフェクトの並べ替えを許可
* &amp;lbrack;Tool&amp;rbrack; Add Tri-平面 投影
* &amp;lbrack;3D ビュー&amp;rbrack;シャドウのサポートを追加
* &amp;lbrack;3D ビュー&amp;rbrack；必要なOpenGLステートをカスタムシェーダに設定する機能
* &amp;lbrack;3D ビュー&amp;rbrack；新しいシェーダによるアルファのサポート
* &amp;lbrack;3D ビュー&amp;rbrack;シェーダがバージョン管理され、プロジェクトに完全に保存されるようになりました。
* &amp;lbrack;3D ビュー&amp;rbrack; シェーダーがコンパイルされなくなった場合に警告する

**修正済み：**

* &amp;lbrack;Layers&amp;rbrack；折りたたまれたフォルダのドロップを修正
* &amp;lbrack;シェルフ&amp;rbrack;ミニシェルフのコンテンツフィルタリングを修正
* &amp;lbrack;シェルフ&amp;rbrack;カテゴリ名の変更とタブの再編成

### 1.2.1

*（リリース：2015年2月12日）*

**追加：**

* エクスプローラーをダブルクリックして\*.sppファイルを開けるようになりました
* &amp;lbrack；書き出し&amp;rbrack；書き出しプリセット用の新しい「$project」タグ
* &amp;lbrack；書き出し&amp;rbrack；各テクスチャセットの下にマップリスト（命名規則あり）を追加
* &amp;lbrack;Export&amp;rbrack; Add a button All/Noneをクリックしてテクスチャセットを選択
* &amp;lbrack;Export&amp;rbrack；空のマップは書き出し中に破棄されます

**修正済み：**

* &amp;lbrack;Export&amp;rbrack; Unity5プリセットには反転したマップがあります
* &amp;lbrack;Export&amp;rbrack;フォルダーにスラッシュを追加すると、プリセット名ーが破損します
* &amp;lbrack；書き出し&amp;rbrack; Heightチャンネルを32ビット形式で書き出すと、正しくクランプされない。
* &amp;lbrack；書き出し&amp;rbrack; テクスチャセットリストがプロジェクトのように並べ替えられない
* &amp;lbrack;Tool&amp;rbrack; バックフェースカリングが機能しない
* パスに特殊文字が含まれていると、「保存」が機能しない

### 1.2.0

*（リリース：2015年1月28日）*

**追加：**

* 法線マップデータをペイントして結果を組み合わせることができる新しい通常チャンネル
* &amp;lbrack;Export&amp;rbrack;カスタムパッキングを作成してカスタム名を設定できる新しい書き出しウィンドウ
* プロジェクトファイル形式が、フォルダーではなく単一ファイルになりました
* &amp;lbrack；書き出し&amp;rbrack；は異なる標準フォーマット(DirectX、OpenGL)をサポートします
* &amp;lbrack；書き出し&amp;rbrack；書き出し時に一時的な「ロック」ファイルを作成
* &amp;lbrack;Layers&amp;rbrack; Shift+LeftMouseクリックでマスクを切り替え
* &amp;lbrack;Parameters&amp;rbrack;イメージ入力の下部のカラースペースを表示する
* &amp;lbrack;シェルフ&amp;rbrack;エフェクト「MGマスクビルダー」が新しい設定になりました
* &amp;lbrack;3D ビュー&amp;rbrack;Ambient occlusionマップが、Specularではなく、拡散反射光の成分を遮断するようになりました

**修正済み：**

* マテリアル/ステンシルのプレビューがビューポートーに正しく表示されない
* &amp;lbrack;3D ビュー&amp;rbrack; 「S」(ステンシル)ショートカットを使用する際にショートカットツールチップが表示されない
* &amp;lbrack;シェルフ&amp;rbrack；効果「MatFxスキンスケール」の低解像度でのパフォーマンスが向上しました
* 大きな文書サイズを指定すると、書き出しの書き出しテクスチャがアップスケールされる(&amp;lbrack;Export&amp;rbrack;)

### 1.1.2

*（リリース：2015年1月15日）*

**追加：**

* 追加：塗りつぶしレイヤーに新しい「移動」、「回転」、「拡大・縮小」が追加されました
* ブラシと塗りつぶしレイヤーの拡張フィルタリング
* 体験版はフル機能（書き出し可能）になりましたが、時間が限られています。

**修正済み：**

* 非常に小さな精度のOBJ メッシュを読み込むことが不可能
* Windows 7および8でライセンスをアクティベートする際の問題
* プロジェクトの「別名で保存」中のクラッシュ
* テクスチャセットの最後のチャンネルを削除するときにクラッシュが発生しました
* 特定のコンテキストでレイヤーを削除すると、クラッシュが発生する

### 1.1.1

*（リリース：2014年12月25日）*

**追加：**

* &amp;lbrack；レイヤー&amp;rbrack;プロジェクトを開く/テクスチャセットを切り替える際に、一番上のレイヤーを選択する
* 新しい圧縮アルゴリズムにより、「保存」および「別名で保存」の速度が向上
* プロジェクトを開いたときにエラーが表示され、Painterでは表示されすぎる

**修正済み：**

* &amp;lbrack；ツール&amp;rbrack；ジオメトリデカールがメモリ破損を生じる
* &amp;lbrack;Brush&amp;rbrack;ブラシサイズに1より小さい浮動小数点値を手動で入力できません
* &amp;lbrack；レイヤー&amp;rbrack;カラー選択効果を作成してもレイヤースタックに追加されない
* &amp;lbrack；レイヤー&amp;rbrack;レイヤーの上にマウスを移動すると、Painterがタスクバーでフリックする
* &amp;lbrack；レイヤー&amp;rbrack;ビットマップをマスクとして追加すると、クラッシュが発生する場合がある
* HeightチャンネルでソロモードのGUIが正しくない
* 「プロジェクトを保存」が失敗してプロジェクトが破損する可能性がある
* 古いシェーダーを含むプロジェクトを読み込んだ後にプロジェクトを開くとクラッシュが発生する

### 1.1.0

*（リリース：2014年12月16日）*

**追加：**

* &amp;lbrack；エフェクト&amp;rbrack；新規マテリアル IDマスククリエーター
* ブラシギズモに新しい覆い焼きの白/黒の線が追加されました
* 新しい角度フォローのパラメータ
* 新しいバックフェースカリングパラメーター
* 新しいレイジーマウスパラメーター
* &amp;lbrack；画層&amp;rbrack；複数選択と管理のサポート
* &amp;lbrack；画層&amp;rbrack；あるフォルダから別のテクスチャセットにコピーして貼り付ける
* &amp;lbrack；書き出し&amp;rbrack; Adobe PhotoshopのPSDフォーマット
* &amp;lbrack;シェルフ&amp;rbrack；新しいツール：ファー、メタルステッチ、ジッパー
* &amp;lbrack;シェルフ&amp;rbrack；新規ブラシ:モールド、鉛筆、シャープライン、ステッチ
* &amp;lbrack;シェルフ&amp;rbrack；新規アルファ:ガウスノイズ、鋭角ライン、モールド、ペン、スプラッシュ、ステッチ、ジッパー
* 必要なテクスチャの一部のみを更新することで、ペイントパフォーマンスを向上

**修正済み：**

* &amp;lbrack;シェルフ&amp;rbrack；同一のラベルを持つグラフを含むサブスタンスをロードできない
* &amp;lbrack；レイヤー&amp;rbrack；通過描画モードがマスクで機能しない
* &amp;lbrack;ステンシル&amp;rbrack；尺度が2D ビューで壊れています
* Mac OS Yosemiteの問題とクラッシュ

### 1.0.2

*（リリース：2014年11月9日）*

**追加：**

* サブスタンスを使用したマテリアルプレビューのパフォーマンスの向上
* ドキュメントの更新時におけるブラシストロークプレビューのパフォーマンスの向上
* 非作業領域の更新速度を下げてビューポートのパフォーマンスを向上させます。
* &amp;lbrack；設定&amp;rbrack;ポストエフェクトを管理するための改善されたUI
* &amp;lbrack;ポストエフェクト&amp;rbrack;デフォルト値にリセット
* 右クリックメニューでのSubstanceエフェクトおよびレイヤーの操作
* サブスタンスの事前乗算入力/出力のサポート

**修正済み：**

* &amp;lbrack;3D ビュー&amp;rbrack;カスタムシェーダーパラメータは大きなスペースで区切られます
* &amp;lbrack;Export&amp;rbrack;Unity4プリセットのsRGB変換がありません
* FBXメッシュの読み込み時に考えられるクラッシュ
* 単純なobj メッシュを読み込むときにクラッシュが発生することがある
* コンピューターのバーは読み込み時に100%ブロックされたままになる
* サブスタンスを再ロードすると、すべてのカテゴリーに入ります
* DirectX/OpenGLスイッチが壊れています

### 1.0.1

*（リリース：2014年10月27日）*

**追加：**

* &amp;lbrack;Tool&amp;rbrack；改善されたマテリアルパラメーターの使用
* ヘルプメニューでuservoice webサイトに新しいショートカットを表示
* エンジンでの様々なパフォーマンスの向上

**修正済み：**

* パラメーター値は、パーティクルに対して2桁までに制限されています
* キャッシュから読み込まれたSubstanceが古くなったとしてUIに表示されない
* ネットワークurlからメッシュを読み込むときにクラッシュが発生しました
* PainterがMac OS Xで署名済みとして認識されるようになりました

### 1.0.0

*（リリース：2014年10月15日）*

**追加：**

* カスタムシェーダーサポート
* 4K解像度のサポート
* キャラクターのサンプルプロジェクト
* 長い計算時間の進捗バーを表示する
* &amp;lbrack；書き出し&amp;rbrack;拡散のポストプロセスの前に拡張パスを追加
* SPのコマンド・ライン引数（単純な操作の場合）
* 新しいマテリアルとエフェクト
* ツールプレビュー（リアルタイムマテリアルプレビューとストロークテスト領域を分離）
* Painterの起動時にデフォルトの文書を作成しない
* &amp;lbrack;Tool&amp;rbrack;グレースケール値を手動で編集する機能を追加
* ステンシルの様々な機能強化（スナップ、リセット）
* パーティクルは、ペイントブラシ、消しゴム、投影ツールのサブツールになりました
* &amp;lbrack;3D ビュー&amp;rbrack;ベイクしたAOをビューポートレンダーで使用する
* 2Dビューと3Dビューの間でステンシルコントロールを分割
* ライブラリでの小さなサムサイズの微調整
* 検索フィールドは各ウィンドウに固有です
* UIの微調整

**修正済み：**

* &amp;lbrack;Susbtance&amp;rbrack; Switch does not work
* &amp;lbrack；カラーダイアログ&amp;rbrack；色相グラデーションが更新されない
* ファイル名が同一の場合、メッシュを更新できない
* 小さすぎる場合、ツールがビューに表示されない
* Retinaディスプレイのデカールツールが正しく動作しない
* &amp;lbrack;Substance&amp;rbrack; Int1はfloat1として表示されます。
* &amp;lbrack;Substance&amp;rbrack;ベースカラーの入出力が認識されない
* &amp;lbrack;Substance&amp;rbrack;フィルタを再読み込みできない
* &amp;lbrack;Tool&amp;rbrack;グレースケールウィジェットが常に折りたたまれます

## ベータ版

### 0.12.1-beta

*（リリース：2014年9月18日）*

**追加：**

* Unity 5書き出しプリセット

**修正済み：**

* PBR シェーダー、レンダリング品質が大幅に向上します
* デフォルトでは、フォーカス機能が機能しなくなり、メッシュが切り抜かれる

### 0.12.0-beta

*（リリース：2014年9月17日）*

**追加：**

* スポイトツール
* バウンディングボックスが変化した場合のメッシュの再読み込みに、「ストロークの位置を保持」オプションが追加されました。
* Cymoulaiデフォルトメッシュの法線マップ
* ツールビューインターフェイスの改善（カラーはWIP）
* メニューの「ヘルプ/設定」を「編集/設定」に移動
* 「すべてのチャンネルを書き出し」ウィンドウで書き出しパスを保存します
* ヒストグラム表示機能を備えた新しいレベルのGUI
* アセット管理の向上（ドラッグ&amp;ドロップ、リソースの再読み込み、未使用のアセットの削除）
* 「拡散」から「ベースカラー」への切り替え
* スライダーの編集調整 – コンマに加えてドットを許可
* 塗りつぶしレイヤー：最大タイリング値を増やす
* 既定の環境マップ

**修正済み：**

* 極端な角度での不適切な反射アーティファクト
* 壊れたSpecular/グロスの書き出し
* painterの「バージョン情報」ウィンドウのリンクが機能しない
* OSXヨセミテとのクラッシュ
* メッシュは三角パッチで保存されます
* ツールウィンドウのカラーショートカットがグレースケールではなくエミッタに送られる
* レイヤーからマスクに切り替えても、カラーピッカーが開いたままになる
* 塗りつぶしレイヤーからマテリアルを保存できない
* シェルフの3つの領域のサイズ変更を有効にする

### 0.11.0-beta

*（リリース：2014年9月4日）*

**追加：**

* 3Dビューと2Dビューの間に分割を追加する
* 2D/3Dビューでのグラデーション背景の使用
* レベル補正ヒストグラムのインターフェイス
* シェルフとライブラリを結合
* プリセットの作成または更新時には、保存アクションは必要ありません
* ドラッグ&amp;ドロップによるシェルフへのアセットの読み込み

**修正済み：**

* ボタンの名前がメインツールバーに表示されます

### 0.10.2-beta

*（リリース：2014年8月28日）*

**修正済み：**

* すべてのチャンネルを書き出すと、間違った結果が生成される

### 0.10.1-beta

*（リリース：2014年8月26日）*

**修正済み：**

* シェーダーは低ラフネスで黒い結果を出す
* GPUチェック：「Quadro」カードを処理し、すべてのデバイスを検出して、それに応じてユーザーメッセージを調整
* Beta 9では、ほとんどのSubstance マテリアルの上限は256です
* ビットマップとして書き出すと、Heightが固定される
* ブラシプレビューは、Macの投影オーバーレイとは異なります
* ジオメトリツールでマスクを作成しても、ビューポートに表示されない
* クイックマスクが壊れています
* 古いmac proでのブレンドの問題の修正

### 0.10.0-beta

*（リリース：2014年8月7日）*

**追加：**

* ステンシルマスク

**修正済み：**

* （クアッドカードのサポート）
* シェーダーは低ラフネスで黒い結果を出す
* マテリアルの上限は256です
* 法線マップの書き出しによってグリーンチャンネルが削除される

### 0.9.0-beta

*（リリース：2014年7月17日）*

**追加：**

* Yebis 2後処理
* 「新規プロジェクト」ウィザードでは、入力マップ（AO、曲率など）を読み込むことができます。
* 入力マップ（AO、曲率など）を自動的に接続 Substanceエフェクトへ
* 塗りつぶしレイヤーに適用されたマテリアルの拡大縮小コントロール

### 0.8.2-beta

*（リリース：2014年7月11日）*

**修正済み：**

* 色相スライダーのデフォルトは白
* マテリアル名に特殊文字が含まれている場合にプロジェクトをリセットする
* 1つのマテリアルオブジェクトでマテリアル名を変更しても、プロジェクトは無効になりません。
* プロジェクトを保存して再度開くと、UVが正しく処理されない

### 0.8.1-beta

*（リリース：2014年7月4日）*

**修正済み：**

* 複数のGPU クラッシュ
* チャンネルを書き出すときのクラッシュ

### 0.8.0-beta

*（リリース：2014年6月28日）*

**追加：**

* マルチマテリアル – 同じ文書内の複数のマテリアルでペイントできるようになりました
* 対称ペイント
* すべての描画モードが使用可能になりました

**修正済み：**

* 複数のGPU クラッシュ
* マテリアル名に特殊文字が含まれている場合にプロジェクトをリセットする
* プロジェクトを保存して複数のUVで再度開くと、UVが正しく処理されない

### 0.7.0-beta

*（リリース：2014年6月18日）*

**追加：**

* レイヤー効果
* 新しいステンシルマテリアル
* マスクをクリア
* レイヤー/マスクのコピー/ペーストを許可
* レイヤーの複製を許可
* レイヤーマスク編集時の変更ツール
* SubstanceはGPUを利用するようになりました

**修正済み：**

* 高さマップペイントでは、負の値はペイントされません。
* マテリアルピッカーの表示では、サンプルした法線マップは考慮しないでください
* パーティクルの決定性が壊れています
* 2D ビューのステンシル行列
* objファイルのN値
* 様々なクラッシュ

### 0.6.0-beta

*（リリース：2014年6月4日）*

**追加：**

* ラフネスチャンネルとメタリックチャンネルの合成からSpecularマップを書き出す新しい書き出しオプション

**修正済み：**

* Windows Vistaとの互換性
* 高さマップは負の値をペイントしません

### 0.5.0-beta

*（リリース：2014年5月7日）*

**追加：**

* 3D/2D ビュースイッチ
* UVチャンク選択ツール
* マスクにペイントすると、ツールが自動的に変更されます。
* Substanceの解像度は、文書の

**修正済み：**

* 起動時のクラッシュ
* ASCIIメッシュを使用したクラッシュ
* 2D ビューの固定ステンシル行列
* 消しゴムとのクラッシュ

### 0.4.0-beta

*（リリース：2014年4月17日）*

**追加：**

* シームレスな2D ビュー
* ビットマップレイヤーマスク
* 環境露出制御
* 塗りつぶしレイヤーは、ツールウィンドウを使用してプロパティを設定するようになりました
* マテリアルは塗りつぶしレイヤーに適用できる
* ステンシルライブラリにステンシルを追加
* 計算を高速化するために更新されたパーティクルプリセット
* 低品質設定のためのPBR シェーダーの最適化と品質向上

**修正済み：**

* レイヤーサムネールは、現在選択されているチャンネルにリンクされます
* 多くのクラッシュ

### 0.3.0-beta

*（リリース：2014年4月4日）*

**追加：**

* カラーセレクターで高さマップペイントに負の値を使用できるようにする
* 選択したマテリアル/カラーのプレビューを表示
* ツールバーにツールのショートカットを追加(1、2、3、4)
* プロジェクトで標準フォーマット（OpenGLとDirectX）をグローバルに切り替える
* 新規プロジェクトウィザード
* 間隔スライダーがクランプされなくなりました
* 更新されたスライダースタイル
* カラーピッカーをモーダルにしない
* ライブラリにマテリアルを選択し、ツールの種類を設定します

**修正済み：**

* 修正：読み込みメッシュのパスが保持されない
* 修正：間違ったテクスチャの生成
* 修正：起動時のクラッシュ

### 0.2.0-beta

*（リリース：2014年3月17日）*

**追加：**

* マテリアルスポイト(Pショートカット)
* 3Dツールプレビューのサムネール
* スタンドアロンバージョンのライセンスシステム
* ブラシサイズの&amp;lbrack；および&amp;rbrack;ショートカット
* 書き出されたマップのパディング
* ツールウィンドウのスタイルを更新
* 更新されたスライダースタイル
* デフォルトのHDR環境の更新

**修正済み：**

* ステンシル:3D ビュー分岐点のフロー値を52に変更します。
* ストロークに0圧キーを追加すると、エンジンに無限ループが発生する問題が修正されました。
* ツール：角度ジッターで+/- 90%を超える値が返されない
* レイヤーマスク選択時の3D ビュー表示の変更
* 反転ズーム

### 0.1.0-beta

*（リリース：2014年3月2日）*

**追加：**

* 新しいライブラリ管理
* 新しいブラシとパーティクルのコンテンツ
* 3Dブラシのプレビュー
* ツールウィンドウのスタイルを更新
* 更新されたスライダースタイル
* 更新されたキャッシュパフォーマンス

**修正済み：**

* カメラコントロール
* ブラシの回転
