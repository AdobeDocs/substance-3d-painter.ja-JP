---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/iray-renderer/viewer-and-mdl-settings.html"
breadcrumb-title: ''
description: Substance 3D PainterでIrayレンダラーのビューアとMDLを設定して、マテリアルレンダリングをカスタマイズする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Iray Renderer > Viewer and MDL Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ビューアとMDLの設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---


# ビューアとMDLの設定

![](../../assets/display-settings-iray.png){width="400px"}

## 環境

通常のビューポートと同じように、Irayで使用される環境マップによって照明が制御されます。\
環境マップを変更するには、ボタンをクリックするか、HDR テクスチャをドラッグ&amp;ドロップします。

* **環境の露出** :HDR 環境マップの露出レベルを制御します。
* **Environment Rotation** :テクスチャをシフトし、周囲の光を回転させます。

>[!NOTE]
>
> Irayは物理的なレンダラーであるため、environmentテクスチャはシーンの照明と外観を大幅に決定します。

## ドーム

ドームは、バックグラウンドで環境マップを投影するシェイプです。\
シーンに応じて3種類のドームを使用できます。

![](../../assets/dome-type.png)

* **無限球体** ：球体上の背景に環境が投影され、地平線をシミュレートしています。これは常にシーンから遠い場所です
* **球** ：環境は通常の球に投影され、スケーリングできます
* **地面付き球体** ：前のシェイプと同様に、このシェイプにも、床をシミュレートするために球の底を平坦にするコントロールがあります。

>[!NOTE]
>
> 地面付き球体には床のサイズ/半径を定義するコントロールがありますが、大きな半径を設定するとゆがみが生じます。\
>  選択したタイプに応じて、照明が影響を受けます。

追加の設定を利用できます。

| *設定* | *説明* |
| --- | --- |
| **半径** | 球のサイズ（無限でない場合） |
| **テクスチャスケール** | **地面付き球体**&#x200B;の種類で伸縮されるテクスチャの量です。 |
| **色のクリア** | 有効になっている場合は、環境マップの背景画像を均一カラーに置き換えます。 これにより、照明が影響を受けます。 |

### 地面の設定

地面の設定では、床の位置を指定できます。\
デフォルトでは、値はシーンのバウンディングボックスの下部を固定するように設定されています。

| ***設定*** | ***説明*** |
| --- | --- |
| **X、Y、Z値** | 3つの軸で床の場所を定義します。   0,0,0の値は、シーンのバウンディングボックスの中央に対応します。 |
| **反射率** | 地盤反射の強度とカラーを定義します。   白の明るさの値は、グランドの反射が100%であることを意味し、黒の値は反射がないことを意味します。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/reflectivity-optim.gif"/></div> |
| **光沢** | 反射の光沢（ラフ）の度合いを定義します。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/glossiness-optim.gif"/></div> |
| **シャドウの適用度** | このパラメーターは、照明が計算された後のシャドウの最終的な不透明度を定義します。 |
| **下から表示** | 地面が下から見えるかどうかを定義します。 オンにすると、その上にある要素が地面によって隠されます。 |

## MDLおよびシェーダー・パラメータ

Iray MDLを使用して、オブジェクトのレンダリングに使用するマテリアルを定義します。 詳しくは、[形式の公式Nvidiaページ](http://www.nvidia.com/object/material-definition-language.html)を参照してください。

Substance 3D Painterのデフォルトでは、MDLはGLSL シェーダーに関連付けられており、何も設定しなくても通常のビューポートとIrayを切り替えることができます。\
MDLのパラメータがビューア設定の下部に表示されます。 デフォルトのMDLのパラメータを次に示します（PBRメタリック/ラフネスシェーダーと互換性があります）。

>[!NOTE]
>
> カスタムMDLを読み込むには、カスタムglsl シェーダーが必要です。\
>  シェーダーにmdlパスを指定するメタデータを追加することができます。
> 
> // – このシェーダーで使用するiray mdl マテリアルを宣言します。 //:メタデータ{ //: &quot;mdl&quot;:&quot;mdl::alg::materials::physically\_メタリック\_ラフネス::physically\_メタリック\_ラフネス&quot; //: }
> 
> * **mdl** : シェーダーで使用するIray mdl マテリアルを定義します。 パスの構文は次のとおりです。*mdl::folder1::folder2::mdl\_filename::folder\_name*&#x200B;ここで、*マテリアル1::folder2::mdl\_filename*&#x200B;は、シェルフー&#x200B;*mdl*&#x200B;フォルダー内のmdlファイルへのパスで、*::マテリアル\_name*&#x200B;はこのmdlファイル内で宣言されたマテリアルーの名前です。 （例： &quot;mdl&quot; : &quot;mdl::alg::materials::physically\_メタリック\_ラフネス::physically\_メタリック\_ラフネス&quot;）

>[!NOTE]
>
> プロジェクト内のマテリアルインスタンスごとに、MDLが設定されます。 そのため、マテリアルのプロパティをテクスチャセット間で分けるには、新しいマテリアルのインスタンスを設定して、MDLを直接構成します。

![](../../assets/mdl.png)

Substance 3D PainterのデフォルトMDLでは、次のプロパティをサポートしています。

| *設定* | *説明* |
| --- | --- |
| **Emissiveの適用度** | emissiveチャンネルのマルチプライヤ。 値を大きくすると、光が放出され始めます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/emissive-optim.gif"/></div> |
| **屈折** | 屈折の量を制御します。 |
| **IOR** | マテリアルの屈折率を指定します。   注：空気= 1.0、水= 1.2、ガラス= 1.5。 |
| **散布** | サーフェス全体に拡散する光の量を制御します。 |
| **吸収** | サーフェスを通して吸収される光の量をコントロールします。 |
| **吸収カラー** | 光がサーフェスを通過するときに色が変化するようにシミュレートします。 |
