---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/painting/fill-projections/planar-projection.html"
breadcrumb-title: ''
description: Substance 3D Painterの平面投影を使用して、テクスチャをフラットな平面から投影し、簡単にテクスチャを適用することができます。
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Planar projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 平面投影
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 2%

---


# 平面投影

![](../../assets/planar-proj-1.jpg)

塗りの平面投影は、イメージを平面として投影する3D投影です。 サーフェス上または3Dモデルを通して標識、デカール、その他のパターンを投影するために使用できます。

## プロパティ

| *設定* | *説明* |
| --- | --- |
| **フィルター** | テクスチャまたはマテリアルのフィルタリング方法をコントロールします。 この設定は、テクスチャを複数回繰り返したときの外観に影響する場合があります。 デフォルトとは異なるフィルタリングを使用してスケーリング値を大きくすると、見栄えが良くなる場合があります。 現在の設定：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>バイリニア | HQ</strong> （既定値）:タイル値が高い場合にテクスチャの品質を向上させる、高度なバイリニアフィルタリングです。</li><li data-preserve-html="true"><strong>バイリニア |シャープ</strong>:テクスチャをわずかに滑らかにしながら、ディテールを保持する単純なバイリニアフィルタリングです。</li><li data-preserve-html="true"><strong>最も近い</strong>:フィルター処理なし。バイリニアフィルターの結果がぼやけて、細かいディテールが見えなくなる場合に便利です。 テクスチャにエイリアスを作成できます。</li></ul> |
| **UV ラップ** | 投影内でテクスチャがどのように繰り返されるかを制御します。 指定可能な値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>なし</strong>:テクスチャは繰り返されません。 テクスチャの外側にあるものは黒/透明です。</li><li data-preserve-html="true"><strong>水平方向に繰り返す</strong>:テクスチャは水平方向でのみ繰り返されます。</li><li data-preserve-html="true"><strong>垂直方向に繰り返す</strong>:テクスチャは垂直方向にのみ繰り返されます。</li><li data-preserve-html="true"><strong>繰り返し</strong> （既定）:テクスチャは両方の軸で繰り返されます。</li></ul>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_image" src="../../assets/planar-repeat.jpg" width="500px"/></div> |
| **図形の切り抜き** | 投影されたテクスチャを投影領域の外側に表示するかどうかを定義します。 指定可能な値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>プロジェクトがシェイプに切り抜かれました</strong>：投影は投影領域内に限定されます。</li><li data-preserve-html="true"><strong>投影がシェイプの外側に広がっています</strong> （既定）：投影は投影領域を超えて続けられます。</li></ul>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_image" src="../../assets/shape-crop-toggle.gif" width="600px"/></div> |
| **深度カリング** | 有効にすると、投影は無限ではなく、投影軸に沿ってフェード/カットされます。  <ul class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">    <strong>有効</strong>:<br/>       <img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c1_procedure_proc_par_proc_step_step_par_image" src="../../assets/depth-culling-on.jpg" width="300px"/>   </li> <li class="step" data-preserve-html="true">    <strong>無効</strong>:<br/>       <img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c1_procedure_proc_par_proc_step1_step_par_image" src="../../assets/depth-culling-off.jpg" width="300px"/> </li> </ul>  次の1つのパラメーターを使用できます。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>硬さ</strong>の設定は、投影軸に沿った深度カリングの硬さまたは柔らかさを制御します。</li></ul>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c1_image" src="../../assets/depth-culling-hardness.gif"/></div> |
| **裏面カリング** | 有効にすると、投影は投影軸から離れた3Dモデルの面には表示されません。次の2つのパラメーターを使用できます。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>角度</strong>：向こうを向いている面を無視する最小の角度を定義します。</li><li data-preserve-html="true"><strong>硬さ</strong>:トランジションの硬さまたは柔らかさを定義します。</li></ul>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c1_image" src="../../assets/backface-culling.gif"/></div> |

>[!NOTE]
>
> 変形スケールを調整すると、投影の深度も制御できます。
> 
> ![](../../assets/planar-fade-optim.gif)

### UVトランスフォーム

UVトランスフォーメーション設定は、投影内のテクスチャ/マテリアルを制御します。

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 40.0%;"/> <col style="width: 20.0%;"/> <col style="width: 40.0%;"/> </colgroup><tbody><tr><th>スケールモード</th><th>設定</th><th>説明</th></tr><tr><td><p><strong>並べて表示</strong> （既定）<strong> <br/></strong></p><p>現在のテクスチャの繰り返し量を手動で設定できます。</p></td><td><strong>タイリング</strong></td><td>テクスチャを繰り返す回数を制御します。</td></tr><tr><td rowspan="2"><br/><br/></td><td colspan="1"><strong>回転</strong></td><td colspan="1">テクスチャをメッシュに投影する角度を制御します。</td></tr><tr><td colspan="1"><strong>オフセット</strong></td><td colspan="1">テクスチャの投影元をコントロールします。 デフォルト値は、テクスチャの中心がメッシュのUVの中心にあることを意味します。</td></tr><tr><th colspan="1"><br/></th><th colspan="1"><br/></th><th colspan="1"><br/></th></tr><tr><td rowspan="4"><p><strong>物理サイズ</strong></p><p>メッシュサイズと埋め込み物理サイズに従ってテクスチャを自動調整します。 幅と長さ（XおよびYの測定値）を使用して、正しい物理サイズを計算します。 Z値は考慮されません。</p><p>(詳しくは、専用の[ドキュメントページ](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/features/physical-size)を参照)</p></td><td><strong>カスタムサイズ</strong></td><td><p>有効にすると、アセットを手動で入力し、物理サイズで提供されているアセットを上書きできます。</p><p>物理サイズが検出されない場合、または異なる物理サイズを持つ複数のアセットが同じレイヤー/エフェクト内で使用されている場合は、自動的に選択されます。</p></td></tr><tr><td colspan="1"><strong>サイズ(cm)</strong></td><td colspan="1">埋め込まれた物理サイズはセンチメートル単位で表されます。 異なる測定単位で作成されたメッシュファイルで作業することができます。正しい縦横比を維持します。 ただし、アセットサイズは現在、センチメートル単位でのみ表示されています。</td></tr><tr><td colspan="1"><strong>回転</strong></td><td colspan="1">テクスチャをメッシュに投影する角度を制御します。</td></tr><tr><td colspan="1"><strong>オフセット</strong></td><td colspan="1"><p>テクスチャの投影元をコントロールします。 デフォルト値は、テクスチャの中心がメッシュのUVの中心にあることを意味します。</p></td></tr></tbody></table>

### 3D 投影設定

3D投影設定は、3D空間での投影の変換を制御します。

| 設定 | 説明 |
| --- | --- |
| **オフセット** | 3D空間での投影原点の位置。 単位は、シーン全体のバウンディングボックスに基づきます。 0がこのボックスの中心です。 |
| **回転** | 各軸上で投影全体を回転する角度。 |
| **スケール** | 各軸の投影全体のサイズ。 |

## コンテキストツールバー

ビューポートの上部にある[コンテキストツールバー](../../interface/toolbars.md)から、マニピュレータとプロジェクションを制御する複数の設定とツールを使用できます。

| アイコン | 名前 | 説明 |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | マニピュレーターを表示 / 非表示 | 有効にすると、マニピュレータがビューポートに表示され、制御可能になります。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | マニピュレータの設定 | このメニューには、次の3つの設定があります。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>マニピュレータのサイズ</strong>:ビューポート内のマニピュレータの大きさを制御します。</li><li data-preserve-html="true"><strong>グリッドステップ</strong>：制約を使用して変換するときのステップのサイズを定義します。</li><li data-preserve-html="true"><strong>角度ステップ</strong>：拘束を使用して回転するときのステップの角度を定義します。</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | 移動マニピュレータ | シーン内の投影を主軸(X、Y、Z)に沿って移動します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | 回転マニピュレータ | シーン内の投影を主軸(X、Y、Z)に沿って回転させます。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | スケールマニピュレータ | シーン内の投影を主軸(X、Y、Z)に沿ってスケールします。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | サーフェスマニピュレータ | 投影を3Dモデルのサーフェスにスナップして移動できるようにします。  **注意：**&#x200B;このマニピュレータは、投影タイプが[平面]または[ワープ]の場合のみ使用できます。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | マニピュレータスペース | 変換を実行するスペースを定義します。 指定可能な値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ローカル空間</strong>：軸は現在の変換に合わせられます。</li><li data-preserve-html="true"><strong>ワールド空間</strong>：軸はシーンに合わせられます。</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | X軸でミラー | 変換をX軸に沿って反転します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Y軸にミラー | 変換をY軸に沿って反転します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Z上でミラー | 変換をZ軸に沿って反転します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-reset.png" width="50px"/></div> | 変形をリセット | 投影変換をデフォルトの状態に戻します。 |

## マニピュレータ

この投影マニピュレータは、[3Dビューポート](../../interface/viewport/3d-view.md)でのみ使用できます。

| アクション | ショートカット | 説明 |
| --- | --- | --- |
| **翻訳** | マウスクリック | 移動マニピュレータで、軸をクリックして投影を移動します。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>1つの軸</strong>:プロジェクションの一方向にのみ移動します。</li><li data-preserve-html="true"><strong>2つの軸</strong>：軸に合わせてプラン上で投影を移動します。</li><li data-preserve-html="true"><strong>3つの軸</strong>:カメラの空間で投影を移動します（平面の方向）。</li></ul>   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_image_794965934" src="../../assets/3d-translate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_image_1473363445" src="../../assets/3d-translate-2axes.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_image" src="../../assets/3d-translate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **翻訳は制限されています** | SHIFT+マウスクリック | 移動マニピュレータを使用して、選択した軸に沿って、特定の間隔（ステップ）でのみ投影を移動します。 間隔のサイズは、マニピュレータの設定によって定義されます。  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_image" src="../../assets/3d-translate-step.gif" width="200px"/></div> |
| **回転** | マウスクリック | 回転マニピュレータで、1つの軸をクリックすると、投影が回転します。 軸の間をクリックすると、すべての軸を同時に回転できます。   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_image" src="../../assets/3d-rotate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_image_1485982924" src="../../assets/3d-rotate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **回転が制限されています** | SHIFT+マウスクリック | 回転マニピュレータで、1つの軸をクリックして投影を回転させると、特定の間隔でのみ投影が実行されます。 ステップは、マニピュレータ設定を介して角度で定義されます。  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_image" src="../../assets/3d-rotate-step.gif" width="200px"/></div> |
| **スケール** | マウスクリック | スケールマニピュレータで、1つの軸ハンドルをクリックして、指定した軸に沿って投影のサイズを変更します。   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_image" src="../../assets/scale-one-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_image_322064801" src="../../assets/scale-two-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_image_49230186" src="../../assets/scale-3-axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **スケールの制約** | SHIFT+マウスクリック | スケールマニピュレータを使用して、ショートカットを維持しながら1つの軸ハンドルをクリックすると、手順に従って投影のサイズが変更されます。 ステップサイズは、移動マニピュレータのステップサイズと同じです。  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_image" src="../../assets/scale-1-axis-constrained.gif" width="200px"/></div> |
| **サーフェス** | マウスクリック | サーフェスマニピュレータを3Dモデル上でクリックしてドラッグすると、サーフェス上にスナップします。  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_image" src="../../assets/surface.gif" width="200px"/></div>  **注意：**&#x200B;このマニピュレータは、**平面**&#x200B;投影タイプおよび&#x200B;**ワープ**&#x200B;投影タイプでのみ使用できます。 |
