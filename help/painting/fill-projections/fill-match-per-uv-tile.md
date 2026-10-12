---
breadcrumb-title: ""
description: Substance 3D PainterでUVタイルごとの塗りつぶし一致を使用して、UVタイル間でテクスチャパターンを一致させることにより、シームレスなタイリングを実現します。
title: 塗り（UV タイルごとに一致）
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 1%
---

# 塗り（UV タイルごとに一致）

**塗りつぶし（UV タイルごとに一致）**&#x200B;は、[UV タイル](../../features/uv-tiles/uv-tiles.md)のプロジェクトに役立つ特殊な2D 投影です。 これにより、各UV タイルのシーケンスからUDIMテクスチャを割り当てることができます。

各UV タイルに1つ以上の画像が割り当てられているため、この投影には専用の設定はありません。 設定がないので、このモードはパフォーマンスにも優れています。

| モード | 説明 |
| --- | --- |
| **UV 投影** | 1つの画像またはシーケンスから最初に取得した画像が、すべてのUVタイルに適用されます。 これにより、変形コントロールも提供されます。詳細については、[UV 投影](uv-projection.md)を参照してください。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-3.jpg" width="700px"/></div> |
| **入力（UV タイルごとに一致）** | シーケンスの各画像は、専用UV タイルに割り当てられます。 変形コントロールはありません。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/fill-match.jpg" width="700px"/></div> |
