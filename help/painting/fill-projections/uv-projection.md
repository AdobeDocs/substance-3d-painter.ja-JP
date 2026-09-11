---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/painting/fill-projections/uv-projection.html"
breadcrumb-title: ''
description: Substance 3D PainterのUV 投影を使用して、UV座標に基づいてテクスチャを投影し、テクスチャを正確に配置します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > UV projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV 投影
user-guide-description: ''
user-guide-title: ''
source-git-commit: 2903c7fdf6a9fe0da149b61fa9064033bb88926a
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 4%

---


# UV 投影

![](../../assets/uv-proj.png)

塗りつぶしのUV 投影は、2D テクスチャスペースでのみ機能する2D投影です。 画像の移動、回転、拡大・縮小を行うコントロールがあります。

## プロパティ

| *設定* | *説明* |
| --- | --- |
| **フィルタリング** | テクスチャまたはマテリアルをフィルタリングする方法をコントロールします。 この設定は、何度も繰り返すときのテクスチャの見え方に影響する可能性があります。 拡大/縮小値が大きい場合は、デフォルトとは異なるフィルタリング方式を使用すると、見栄えが良くなる場合があります。 現在使用可能な設定：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>バイリニア`\|` HQ </strong>: （既定）タイリング値が高い場合にテクスチャの質を向上させる高度なバイリニアフィルタリングです。</li><li data-preserve-html="true"><strong>バイリニア`\|`シャープ</strong> :テクスチャを少し滑らかにしますが、詳細は保持しようとします。単純なバイリニアフィルタリングです。</li><li data-preserve-html="true"><strong>最も近い</strong>: フィルタリングがありません。バイリニアのフィルタリングの結果がぼやけて、細かいディテールが壊れている場合に便利です。 テクスチャにエイリアスが発生する可能性があります。</li></ul> |
| **UV ラップ** | 投影されたマテリアルやイメージが投影のシェイプ内でどのように繰り返されるかを制御します。 指定可能な値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>なし</strong> :投影の繰り返しがありません。</li><li data-preserve-html="true"><strong>水平方向に繰り返す</strong> ：水平方向でのみ繰り返します。</li><li data-preserve-html="true"><strong>縦方向に繰り返す</strong> ：縦方向にのみ繰り返します。</li><li data-preserve-html="true"><strong>繰り返し</strong> （既定） ：水平方向と垂直方向の両方で繰り返します。</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-repeat.jpg" width="500px"/></div> |

### UV変換

UV変換の設定は、投影内のテクスチャ/マテリアルを制御します。

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 40.0%;"/> <col style="width: 20.0%;"/> <col style="width: 40.0%;"/> </colgroup><tbody><tr><th>スケールモード</th><th>設定</th><th>説明</th></tr><tr><td><p><strong>タイリング</strong> （既定）<strong> <br/></strong></p><p>現在のテクスチャの繰り返し量を手動で設定できます。</p></td><td><strong>タイリング</strong></td><td>テクスチャの繰り返し回数を制御します。</td></tr><tr><td rowspan="2"><br/><br/></td><td colspan="1"><strong>回転</strong></td><td colspan="1">テクスチャをメッシュに投影する角度をコントロールします。</td></tr><tr><td colspan="1"><strong>オフセット</strong></td><td colspan="1">テクスチャの投影元をコントロールします。 デフォルト値は、テクスチャの中心がメッシュのUVの中心であることを示します。</td></tr><tr><th colspan="1"><br/></th><th colspan="1"><br/></th><th colspan="1"><br/></th></tr><tr><td rowspan="4"><p><strong>物理サイズ</strong></p><p>メッシュサイズと埋め込み物理サイズに応じてテクスチャを自動調整します。 幅と長さ（XおよびYの測定値）を使用して、正しい物理サイズを計算します。 Z値は考慮されません。</p><p>(詳しくは、専用の[ドキュメントページ](https://experienceleague.adobe.com/ja/docs/substance-3d-painter/using/features/physical-size)を参照)</p></td><td><strong>カスタムサイズ</strong></td><td><p>有効にすると、アセットを手動で入力し、物理サイズで提供されているアセットを上書きできます。</p><p>物理サイズが検出されない場合、または異なる物理サイズを持つ複数のアセットが同じレイヤー/エフェクト内で使用されている場合は、自動的に選択されます。</p></td></tr><tr><td colspan="1"><strong>サイズ(cm)</strong></td><td colspan="1">埋め込まれた物理サイズはセンチメートル単位で表されます。 異なる単位のメッシュファイルで作業することができます。正しい縦横比が維持されます。 ただし、アセットサイズは現在、センチメートル単位でのみ表示されています。</td></tr><tr><td colspan="1"><strong>回転</strong></td><td colspan="1">テクスチャをメッシュに投影する角度をコントロールします。</td></tr><tr><td colspan="1"><strong>オフセット</strong></td><td colspan="1"><p>テクスチャの投影元をコントロールします。 デフォルト値は、テクスチャの中心がメッシュのUVの中心であることを示します。</p></td></tr></tbody></table>

## コンテキストツールバー

ビューポートの上部に表示される[コンテキストツールバー](../../interface/toolbars.md)から、マニピュレーターと投影を制御する複数の設定とツールを使用できます。

| アイコン | 名前 | 説明 |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-manipulator-2d-hide.png" width="50px"/></div> | マニピュレーターを表示 / 非表示 | 有効にすると、マニピュレーターがビューポート内で表示およびコントロール可能になります。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings-2d.png" width="50px"/></div> | マニピュレーターハンドルサイズ | このメニューには、ビューポート内での変形のハンドルの大きさを指定する3つの設定が含まれています。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>小</strong></li><li data-preserve-html="true"><strong>中</strong></li><li data-preserve-html="true"><strong>ラージ</strong></li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | X軸でミラー | X軸の変形を反転します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Y軸にミラー | Y軸の変形を反転します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_image" src="../../assets/icon-pivot.png" width="50px"/></div> | 回転軸をリセット | ピボットポイントを変換の途中に戻します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_image" src="../../assets/icon-reset.png" width="50px"/></div> | 変形をリセット | 投影変換をデフォルトのステートに戻します。 |

## マニピュレーター

このUV 投影では、[2D ビュー](../../interface/viewport/2d-view.md)でしか使用できないマニピュレーターが使用されています。

| アクション | ショートカット | 説明 |
| --- | --- | --- |
| **移動** | マウスクリック | 変形内の任意の領域をクリックしてドラッグし、移動します。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-translate.gif"/></div> |
| **制約付きで移動** | SHIFT+マウスクリック | ショートカットを押したまま変形内の任意の領域をクリックしてドラッグし、1つの軸に沿ってのみ動かします。 軸は水平方向または垂直方向のいずれかにすることができ、マウスの向きに基づいてカメラに合わせられます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-translate-constrained.gif"/></div> |
| **回転** | マウスクリック | 変形の外側からクリックしてドラッグすると、変形を回転できます。 ピボットを移動すると、回転の原点も変更できます。   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-rotation.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-rotation-pivot.gif"/></div>  </td> </tr> </table> |
| **回転が制限されています** | SHIFT+マウスクリック | ショートカットを押したまま、変形の外側からクリックしてドラッグすると、45度ごとに回転させることができます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-rotation-constrained.gif"/></div> |
| **スケール** | マウスクリック | 変形のハンドルをクリックしてドラッグすると、マニピュレーターを変形できます。   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-free.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-middle.gif"/></div>  </td> </tr> </table> |
| **スケールの制約** | SHIFT+マウスクリック | ショートカットを押しながらハンドルをドラッグすると、縦横比を維持したまま変形することができます。   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-ratio.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-middle-ratio.gif"/></div>  </td> </tr> </table> |
| **ミラー化されたスケール** | CTRL+マウスクリック | ショートカットを押しながらハンドルを動かすと、他のハンドルも同様の動きをします。 これにより、ピボットポイントの周囲で対称に変換を変形できます。   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-mirror.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-mirror-pivot.gif"/></div>  </td> </tr> </table> |
| **ミラー化および制約付きで拡大・縮小** | SHIFT+CTRL+マウスクリック | 両方のショートカットキーを組み合わせて使用すると、縦横比を維持しながら対称に合わせて変形できます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r8-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-mirror-ratio.gif"/></div> |
