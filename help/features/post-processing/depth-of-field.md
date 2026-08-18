---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/depth-of-field.html"
breadcrumb-title: ''
description: Substance 3D Painterでフィールド深度の後処理を使用して、カメラにフォーカスしたぼかし効果をリアルに作成する方法を説明します。
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

**フィールドの深度** (DOF)に直接パラメーターがありません。 有効にすると、**Iray**&#x200B;からの自由度が&#x200B;**上書き**&#x200B;されます。

ビューポート内の自由度の外観をコントロールするには、カメラを使用して次の2つの設定を使用できます。

| *設定* | *説明* |
| --- | --- |
| **焦点距離** | フォーカスポイントが位置する距離を定義します。  このポイントは「フィールドの深度」エフェクトで使用されます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **注意：**&#x200B;フォーカス距離は、ショートカット&#x200B;**Ctrl +マウスの中ボタンでメッシュのポイントをクリックすることで自動的に設定できます。** |
| **絞り** | フィールドの深度の幅を指定します。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **注意：** Irayがこのパラメーターを制御している場合、このパラメーターを変更すると計算が再トリガーされます。 |
