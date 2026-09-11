---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Substance 3D PainterのUVを使用して、2D ビュー空間でテクスチャを表示および編集し、正確にテクスチャをペイントする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Viewport > 2D view
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 2D ビュー
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 1%

---


# 2D ビュー

![](../../assets/2d-view.jpg){width="450px"}

2D ビューには、現在選択されている[テクスチャセット](../texture-set/texture-set.md)のメッシュUV アイランドが表示されます。 これにより、レイヤースタックからのテクスチャだけでなく、メッシュUV アイランドに関するペイントも表示できます。

## 表示モード

![](../../assets/display-mode-1.png)

ビューポートの右上には、表示モードのドロップダウンがあります。 このコントロールを使って、ビューポートに表示する情報を変更できます。 これにより、シングルチャンネル、メッシュマップ、または最終的なマテリアル結果を照明で表示できます。

## 軸情報

![](../../assets/2d-axis.png)

ビューポートの右下には、**軸情報**&#x200B;があります。これは、2次元軸の向きを示します。 2D ビューの場合、軸はUとVです。

## UV タイル情報

![](../../assets/2d-view-button.png)

**表示モード**&#x200B;の横には、**UV タイル情報**&#x200B;ボタンがあり、UV タイルに関する情報の表示/非表示を切り替えることができます。 このボタンは、通常のプロジェクトでは表示されません。

## プロジェクトワークフロー

プロジェクトの作成時に定義したワークフローによっては、2D ビューの外観と動作が異なる場合があります。

| *プロジェクトワークフロー* | *ビヘイビアー* |
| --- | --- |
| **通常のプロジェクト** | 通常のプロジェクトでは、UV範囲[0-1]のUVのみをペイントすることができます。 この範囲外は表示されますが、インタラクティブにはなりません。この例では、左側のUV アイランドのみ（背景が明るいグレー）にペイントできます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **UV タイルプロジェクト** | UV タイルプロジェクトでは、各UV範囲はテクスチャの新しいセットで、ペイントすることができます。 各タイルがどのように構成されているかを確認するために、2D ビューとグリッドが表示されます。 各タイルには、UDIM番号が割り当てられます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
