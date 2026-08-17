---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/workflow-issues/shelf-issues/thumbnails-in-the-shelf-look-incorrect.html"
breadcrumb-title: ''
description: Substance 3D Painterシェルフで不正確なサムネール表示を修正して、リソースのプレビューが正確になるようにする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Shelf Issues > Thumbnails in the shelf look incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: シェルフのサムネールが正しく表示されない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# シェルフのサムネールが正しく表示されない

シェルフ内のサムネールが通常とは異なるように見える場合は、プレビューのレンダリングに使用されたシェーダが原因である可能性があります。

| サムネールの破損 | 標準のサムネール |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-broken-preview.png"/></div> | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-normal-preview.png" width="300px"/></div> |

## 1 – メイン設定ウィンドウを開きます。

**編集**&#x200B;に移動して、**設定**&#x200B;をクリックします。

![](../../../assets/pref-menu.png)

## 2 – シェルフプレビューシェーダを削除する

**一般**&#x200B;表示で、「プレビューオプション」セクションが表示されるまで下にスクロールします。\
「**マテリアルプレビューシェーダー**」の前にある「**クロス**」ボタンをクリックして、指定した現在のシェーダを削除します。

![](../../../assets/remove-preview-shader.png){width="450px"}

## 3 - Substance 3D Painterを再起動する

サムネールを再生成して正しく表示されるようにするには、Substance 3D Painterを再起動する必要があります。
