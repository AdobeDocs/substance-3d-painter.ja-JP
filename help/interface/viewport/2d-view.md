---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Substance 3D Painterの2Dビューを使用して、UV空間でテクスチャを表示および編集し、正確にテクスチャペイントを行う方法について説明します。
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

2Dビューには、現在選択されている[テクスチャセット](../texture-set/texture-set.md)のメッシュUV アイランドが表示されます。 レイヤスタックのテクスチャを表示するだけでなく、メッシュUV アイランド上にペイントすることもできます。

## 表示モード

![](../../assets/display-mode-1.png)

ビューポートの右上に、表示モードドロップダウンがあります。 このコントロールを使用すると、ビューポートに表示する情報を変更できます。 これにより、単一のチャンネル、メッシュマップ、または最終的なマテリアル結果を照明で表示できます。

## 軸の情報

![](../../assets/2d-axis.png)

ビューポートの右下には、**軸情報**&#x200B;があります。これは、2つの次元の軸の方向を示します。 2Dビューの場合、軸はUとVです。

## UVタイル情報

![](../../assets/2d-view-button.png)

**表示モード**&#x200B;の横には、**UVタイル情報**&#x200B;ボタンがあり、UVタイルに関連する情報を表示または非表示にすることができます。 このボタンは、通常のプロジェクトでは表示されません。

## プロジェクトワークフロー

プロジェクトの作成時に定義したワークフローによっては、2Dビューの外観と動作が異なる場合があります。

| *プロジェクトワークフロー* | *ビヘイビアー* |
| --- | --- |
| **通常のプロジェクト** | 通常のプロジェクトでは、UV範囲[0-1]のUVのみにペイントできます。 この範囲外は表示されますが、インタラクティブにはなりません。この例では、左側のUV アイランドのみ（背景が明るいグレー）にペイントできます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **UVタイルプロジェクト** | UVタイルプロジェクトを使用すると、各UV範囲はペイント可能な新しいテクスチャセットになります。 2Dビューとグリッドが表示され、各タイルの構成がわかりやすくなります。 各タイルにはUDIM番号が割り当てられます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
