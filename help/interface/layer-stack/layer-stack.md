---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/layer-stack.html"
breadcrumb-title: ''
description: Substance 3D Painterのレイヤースタックを使用して、複数のテクスチャペイントレイヤーを整理および管理する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: レイヤースタック
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 5%

---


# レイヤースタック

![](../../assets/layer-stack.png)

**レイヤースタック**&#x200B;を使用すると、テクスチャセットのレイヤーを操作できます。 レイヤーには、シーンの3Dオブジェクトにテクスチャを作成するペイントと効果が含まれます。 レイヤーの表示と非表示を切り替えたり、レイヤーをフォルダーに入れたり、不透明度や描画モードを変更したりすることができます。

詳しくは、次のページを参照してください。

* [レイヤーの作成](creating-layers.md)
* [レイヤーの管理](managing-layers.md)
* [マスクとエフェクト](masking-and-effects.md)
* [描画モード](blending-modes.md)
* [レイヤーのインスタンス化](layer-instancing.md)
* [ジオメトリマスク](geometry-mask.md)

## 概要

レイヤースタックには、特定の階層のレイヤーが表示されます。一番下のレイヤーが最初にメッシュに描画され、一番上のレイヤーが後に続きます。 したがって、一番上のレイヤーが最後の項目で、一番下のレイヤーが最初の項目です。 フォルダーも同じ原則ですが、フォルダーの内容が優先されます。 つまり、フォルダーの内容は、同じレベルのレイヤーよりも先に処理されます。

**共通の特徴：**

* 各レイヤーは&#x200B;**マルチチャンネル**&#x200B;です。
* ペイントツールでは、マテリアルの設定に応じて&#x200B;**対応するすべてのチャンネル**&#x200B;にペイントされます（レイヤースタックで現在表示しているチャンネルには影響しません）。
* 各レイヤーには、**描画モード**&#x200B;とチャンネルごとの&#x200B;**不透明度**&#x200B;があります（左上のドロップダウンメニューでチャンネルを切り替えることができます）。

**レイヤーの種類：**

* **ペイントレイヤー** ：このタイプのレイヤーは、ブラシやパーティクルでペイントできます
* **レイヤーを塗りつぶし** ：このレイヤーにペイントすることはできません。代わりに、レイヤーにマテリアルを読み込んで、チャンネルを塗りつぶすことができます。 （たとえば、変形を操作してマテリアルを繰り返すこともできます）。
* **フォルダー** ：このタイプのレイヤーは、他のレイヤーを含むことを目的としているため、主にレイヤースタックを整理するために使用されます

各レイヤーで、**マスクを追加**&#x200B;できます。マスクでは、現在のテクスチャセットのチャンネルの特定の部分にのみコンテンツを適用できます。\
マスクは手動で（ブラシを使用してグレースケールで）ペイントすることも、フィルターやサブスタンスを使用して、よりダイナミックでプロシージャルな結果を得ることもできます。

## Viewmode

![](../../assets/switch-viewmode-optim.gif)

レイヤースタックの左上のドロップダウンは、レイヤースタックの表示モードを制御します。 レイヤーは複数のチャンネルをカバーできるため、すべてのプロパティを一度に表示することはできません。 したがって、ビューモードを使用して現在の表示コンテキストを定義できます。 このドロップダウンを使用すると、レイヤーサムネールでの表示に使用するチャンネルを指定したり、このチャンネルのみの描画モードと不透明度を制御したりできます。

このドロップダウンの一覧は、[テクスチャセット設定](../texture-set/texture-set-settings.md)で使用できるチャンネルの一覧に基づいています。

## アクション

![](../../assets/image2020-9-30-12-2-13.png)

アイコンの右上のリストは、レイヤースタックで実行できる一般的なアクションです。

| アクション | 説明 |
| --- | --- |
| エフェクトの追加 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-effect.png"/></div> | 新しいエフェクトを作成し、現在選択されているレイヤーに追加します。 効果の詳細については、[専用ページ](../../features/effects/effects.md)を参照してください。 |
| マスクの作成 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-mask.png"/></div> | 次の項目を含むマスクアクションメニューを開きます。<ul data-preserve-html="true"><li data-preserve-html="true">ホワイトマスクの追加</li><li data-preserve-html="true">ブラックマスクの追加</li><li data-preserve-html="true">ビットマップマスクの追加</li><li data-preserve-html="true">カラー選択によるマスクの追加</li><li data-preserve-html="true">高さを組み合わせたマスクの追加</li></ul> |
| ペイントレイヤーを新規作成 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-11-52-41.png"/></div> | 現在選択されているレイヤーの上に新しいペイントレイヤーを作成します。 |
| 塗りつぶしレイヤーを新規作成 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-0-49.png"/></div> | 現在選択されているレイヤーの上に新しい[塗りつぶしレイヤー](../../painting/fill-projections/fill-projections.md)を作成します。 |
| 新しいスマートマテリアルを追加 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-smartmat.png"/></div> | 現在選択されているレイヤーの上に新しいスマートマテリアルを挿入します。このボタンをクリックするとミニシェルフが開き、現在の[アセット](../../interface/assets/assets.md)で使用可能なスマートマテリアルのリストを参照できます。 |
| 新規フォルダーを追加 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-1-13.png"/></div> | 現在選択されているレイヤーの上に空のフォルダーを新規作成します。 |
| レイヤーを削除 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-trash.png"/></div> | 現在選択されているアイテム（レイヤー、フォルダー、エフェクト）を削除します。 |
