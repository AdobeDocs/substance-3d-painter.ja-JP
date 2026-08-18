---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/project-creation.html"
breadcrumb-title: ''
description: Substance 3D Painterで新規プロジェクトを作成し、3Dモデルにテクスチャをペイントする方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Project Creation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: プロジェクトの作成
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 1%

---


# プロジェクトの作成

![](../assets/v12_banner_project_window.jpg)

<b>新しいプロジェクトウィンドウ</b>では、3Dモデルとそのテクスチャリング情報を保存するプロジェクトファイルを作成できます。

読み込まれた3Dモデルで見つかったマテリアル定義ごとに、新しい[テクスチャセット](../interface/texture-set/texture-set.md)が作成されます。 つまり、異なるマテリアルを持つ複数のオブジェクトは、単一のファイルを介して（重なり合うUVを含む場合でも）読み込むことができます。

## 新規プロジェクトの作成

新しいプロジェクトを作成するには、<b>ファイル/新規</b>をクリックするか、キーボードショートカット<b>Ctrl + N</b>を使用します。

「新規プロジェクト」ウィンドウで使用できるすべてのパラメータを以下に説明します。

### 基本設定

| *パラメーター* | *説明* |
| --- | --- |
| **ファイル** | 「選択」ボタンをクリックして、ロードする3Dモデルファイルを指定します。 [サポートされているファイル形式の一覧はこちらから入手できます。](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats) |
| **テンプレート** | プロジェクトのデフォルト設定を定義するテンプレートを指定します。 テンプレートには、次のパラメーターが含まれています。<ul data-preserve-html="true"> <li data-preserve-html="true">テクスチャセット設定。</li> <li data-preserve-html="true">表示設定。</li> <li data-preserve-html="true">ベイク処理の設定</li> <li data-preserve-html="true">シェーダリソース（アタッチされたテクスチャを含む）。</li> <li data-preserve-html="true">環境マップファイル。</li> </ul>  **注意：**&#x200B;テンプレートは、[ファイルメニュー](../interface/main-menu/file-menu.md)を使用して既存のプロジェクトから作成され、アセットフォルダー内に保存されてチームメンバーと簡単に共有できる<b>\*.spt</b>ファイルです。 |
| <b>解決策</b> | 各テクスチャセットのプロジェクトのデフォルトのテクスチャ解像度を定義します。 アプリケーション内で作業する場合の解像度は最大4K（4096 x 4096ピクセル）、書き出す場合の解像度は8K（8192 x 8192ピクセル）です。 解像度は、後で[テクスチャセット設定](../interface/texture-set/texture-set-settings.md)を使用していつでも変更できます。  **注意：** 8Kの書き出しを行うには、GPUで2.5GB以上のVRamが必要です。 |

### ファイルタイプ特有の設定

USDを選択すると、他のファイルタイプ固有の設定が使用できるようになります。

| *パラメーター* | *説明* |
| --- | --- |
| <b>スコープとバリアント</b> | USDファイルの特定の部分を選択します。 デフォルトでは「ルート」に設定されているため、Painterプロジェクトの作成にはUSDファイル全体が使用されます。  <b>変更…</b>では、USDの内容を表示する新しいウィンドウが開きます。 バリアントが検出された場合は、プロジェクト作成用に特定のバリアントを選択できます。 スコープとバリアントは、[プロジェクト構成](../interface/project-configuration.md)設定でプロジェクトを作成した後に変更できます。 注意：<ul data-preserve-html="true"> <li data-preserve-html="true">モデリングバリアントの選択のみが、プロジェクトに影響を与えます。</li> <li data-preserve-html="true">バリアント内にネストされたバリアントは、現在検出されません。</li> </ul> |
| <b>再分割レベル</b> | この設定を使用すると、分割する必要があるジオメトリについて、Painterでテクスチャリング用にメッシュをどの程度分割するかを指定できます。 USDファイル内でサブディビジョンが明示的に「なし」に設定されている場合、この設定はグレー表示されます。  サブディビジョンはUVのアンラップ後に適用されるため、メッシュのUVのシェイプは変更されません。 再分割レベルは、[プロジェクト構成](../interface/project-configuration.md)設定でプロジェクトを作成した後に変更できます。 |
| <b>フレーム</b> | アニメーションが検出されたUSDファイルの場合、この設定を使用すると、Painterプロジェクトの作成に使用するフレームを選択できます。 選択したUSDファイルにアニメーションがない場合、この設定はグレー表示されます。 フレームは、[プロジェクト構成](../interface/project-configuration.md)設定でプロジェクトを作成した後に変更できます。 |

### 詳細設定

| *パラメーター* | *説明* |
| --- | --- |
| **法線マップ形式** | プロジェクトの法線マップ形式を定義します。次のいずれかを実行できます<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (X+、Y-、Z+)</li><li data-preserve-html="true"><strong>OpenGL</strong> (X+、Y+、Z+)</li></ul>  **注意：**&#x200B;お知らせ：<ul data-preserve-html="true"> <li data-preserve-html="true"><b>アンリアルエンジン</b>は、既定でDirectXを使用します。</li> <li data-preserve-html="true"><b>Unity</b>では、既定でOpenGLが使用されます。</li> </ul> |
| **フラグメントごとの接線空間の計算** | 有効にすると、Bitangentsは頂点シェーダではなくフラグメント（ピクセル）シェーダで計算されます。 このパラメータは、ビューポート内のシェーダによる法線マップのデコード方法に影響を与えます。 この設定を変更するには、法線マップを再ベイクする必要があります。  **注意：**&#x200B;お知らせ：<ul data-preserve-html="true"> <li data-preserve-html="true"><b>アンリアルエンジン</b>では、この設定を有効にする必要があります。</li> <li data-preserve-html="true"><b>Unity</b>では、この設定を無効（またはHDRPワークフローを使用している場合は有効）にする必要があります</li> </ul> |

### UV タイル設定 (UDIM)

>[!NOTE]
>
> プロジェクトを作成した後で、これらの設定を変更することはできません。

| *パラメーター* | *説明* |
| --- | --- |
| **UVタイルワークフローを使用** | チェックすると、読み込まれたメッシュは、通常のUV範囲(0～1)外でペイントできるように異なる方法で処理されます。 UDIMを使用するプロジェクトでは、この設定を有効にする必要があります。 メッシュの処理は、設定によって異なる場合があります。   詳細については、[UVタイルのドキュメント](../features/uv-tiles/uv-tiles.md)を参照してください。 |
| <b>マテリアルごとにUVタイルのレイアウトを保持し、タイル間でのペイントを有効にする</b> | UVタイル(UDIM)が読み込まれ、メッシュ上のマテリアル割り当てごとにグループ化されます。 つまり、1つのテクスチャセットに、2Dビューで並んで表示される複数のUVタイルを含めることができます。 同じテクスチャセット内にあるUVタイルは、シームレスにペイントすることができます。  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c1_image_copy" src="../assets/uvtiles-paintacross.jpg" width="500px"/></div> |
| <b>UVタイルを個別のテクスチャセットに変換（従来）</b> | UVタイル(UDIM)は、個々のテクスチャセットに分割され、マテリアルの割り当てを無視して名前が変更されます。 各UVタイルは、ペイント可能なUV [0-1]範囲に移動されます。  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c1_image" src="../assets/uvtiles-legacy.jpg" width="500px"/></div> |

### 読み込み設定

| ***パラメーター*** | ***説明*** |
| --- | --- |
| **カメラの読み込み** | カメラがメッシュファイルに存在する場合、それらはプロジェクトに読み込まれ、視覚化のためのプリセットとしてアクセスできます。  **注意：** Substance 3D Painterは、特定の条件下では一部のカメラをサポートしていません。<ul data-preserve-html="true"><li data-preserve-html="true">3DS Maxの物理カメラ</li><li data-preserve-html="true">Alembicファイル(&#42;.abc)に保存されている正射投影カメラ。</li></ul> |
| **自動ラップ解除** | 有効にすると、インポートされたメッシュ上の欠落しているUVが生成されます。 処理は、[**オプション**]ボタンで選択した設定によって変わる場合があります。詳細については、[UVの自動アンラップのドキュメント](../features/automatic-uv-unwrapping.md)を参照してください。 |

### ベイク済みマップを読み込み

<b>[追加]</b>ボタンを使用して、テクスチャファイルをメッシュマップとして読み込み、[テクスチャセット設定](../interface/texture-set/texture-set-settings.md)で自動的に割り当てます。 特定の命名規則に従って、メッシュマップを自動的にテクスチャセットに割り当てる必要があります。 メッシュマップは、アプリケーション内で直接ベイク処理することもできます。ベイク処理に関するドキュメントを参照してください。

命名規則： <b> TextureSetName\_MeshMapName</b>

例：<b> DefaultMaterial\_ambient\_オクルージョン.png </b>

サポートされているメッシュマップとその名前のリスト：

| *メッシュマップ* | *ファイル名変換* |
| --- | --- |
| **環境オクルージョン** | ambient\_オクルージョン |
| **曲線** | 曲率 |
| **標準** | normal\_base |
| **ワールド空間標準** | world\_space\_normals |
| **ID** | id |
| **位置** | 位置 |
| **Thickness** | 厚み |

### 物理サイズ

物理サイズを設定すると、Painterがメッシュの物理サイズを実際の単位で決定する方法を調整できます。 これは、マテリアルがリアルな尺度で適用されていることを確認するのに便利です。

* メッシュファイルの内部単位スケールを使用：ほとんどのファイルタイプには、3Dモデリングアプリケーションから書き出されたオブジェクトの物理サイズに関する情報が含まれています。 このオプションを選択すると、Painterは読み込まれたファイルからこの情報を使用します。
* カスタム単位スケール：読み込んだファイルの単位スケールを上書きします。単位スケールが含まれていない場合は、カスタム入力ボックスを使用して1つの「単位」のサイズを調整します。
* マテリアルを割り当てるときに塗りつぶしレイヤーの拡大・縮小を物理サイズに切り替え：このオプションを有効にすると、物理サイズに関する情報を持つマテリアルが、適用されるサーフェスの物理サイズに合わせて拡大・縮小を調整できます。

### カラーマネジメント

![](../assets/newproj-cm.png)

このセクションでは、プロジェクトのカラーマネジメント設定を制御します。 デフォルトでは、「レガシー」（sRGB /リニアワークフロー）に設定されています。

このワークフローの使用方法と設定の機能について詳しくは、[カラーマネジメント](../features/color-management/color-management.md)のドキュメントを参照してください。
