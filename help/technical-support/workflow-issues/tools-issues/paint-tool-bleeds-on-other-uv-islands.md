---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/tools-issues/paint-tool-bleeds-on-other-uv-islands.html"
breadcrumb-title: ''
description: Substance 3D PainterでUV アイランド間のペイントツールのにじみを補正して、テクスチャの境界線をきれいに保つ方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Paint Tool bleeds on other UV islands
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ペイントツールが他のUV アイランドでブリードする
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%

---


# ペイントツールが他のUV アイランドでブリードする

[ペイントツール](../../../features/effects/paint.md)の既定の動作の中には、特定の状況で直感的に感じられないものがあります。 Substance 3D Painterは主に3D空間で動作するアプリケーションです。これはペイントにも適用されます。 ペイントブラシのデフォルト設定は、ペイント時にUVをまたいでシームレスになるようにすることです。 そのため、2D ビューを操作すると、予期しない結果が生じることがあります。

2D ビューをペイントするときに他のUV アイランドににじみが発生しないようにするには、ツールパラメーターの&#x200B;**アラインメント**&#x200B;の設定を変更します。

| *アラインメントモード* | *プレビュー* |
| --- | --- |
| **正接ラップ** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-tangent-optim.gif"/></div> |
| **UV** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-uv.gif" width="450px"/></div> |
