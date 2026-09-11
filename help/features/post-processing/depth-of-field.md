---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/post-processing/depth-of-field.html"
breadcrumb-title: ''
description: Substance 3D Painterでフィールド後処理の深度を使用して、リアルなカメラフォーカスブラーエフェクトを作成する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Depth of Field
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 被写界深度
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '132'
ht-degree: 4%

---


# 被写界深度

![](../../assets/dof-example.jpg)![](../../assets/dof.png)

**フィールドの深度** (DOF)に直接パラメーターがありません。 有効にすると、**Iray**&#x200B;のDOFが&#x200B;**上書き**&#x200B;されます。

カメラでは、ビューポートの自由度の外観をコントロールするために、次の2つの設定を利用できます。

| *設定* | *説明* |
| --- | --- |
| **焦点距離** | フォーカスポイントが位置する距離を定義します。  このポイントは「フィールドの深度」エフェクトで使用されます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **注意：** メッシュのポイントをショートカット **CTRL +マウスの中央ボタンでクリックすると、フォーカス距離を自動で設定できます。** |
| **アパーチャ** | フィールドの深度の幅を指定します。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **注意：** Irayがこのパラメーターを制御している場合、このパラメーターを変更すると計算が再トリガーされます。 |
