---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/effects/compare-mask.html"
breadcrumb-title: ''
description: Substance 3D Painterのマスク比較エフェクトを使って、テクスチャの比較処理にもとづいてマスクを作成する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Compare Mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 比較マスク
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---


# 比較マスク

![](../../assets/compare-mask.png)

このエフェクトを使用すると、2つのチャンネルをすばやく簡単に比較し、結果としてマスクを作成できます。 このエフェクトは、レイヤーのマスクでのみ使用できます。

このエフェクトで使用可能な設定は次のとおりです。

| 設定 | 説明 |
| --- | --- |
| **チャネル** | ソースとターゲットを比較してマスクを作成するチャンネル。 このLISは、[テクスチャセット設定](../../interface/texture-set/texture-set-settings.md)で使用可能なチャンネルに基づいています。 |
| **比較** | ここでは、マスクの計算方法を選択するための3つのパラメーターを使用できます。 中央のドロップダウンは、比較操作を定義します（より小さい、許容値内、より大きい）。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/compare-mode.png"/></div> ソースモードとターゲットモード:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>下のレイヤー</strong> ：現在のレイヤーの下にあるすべてのレイヤーの統合されたバージョンを考慮します。</li><li data-preserve-html="true"><strong>このレイヤー</strong> ：このレイヤーのみを考慮します。</li><li data-preserve-html="true"><strong>このマスク</strong> :マスクの既存の内容を考慮します（例えば、塗りつぶし効果またはジェネレーター効果が既に存在する場合）。</li><li data-preserve-html="true"><strong>定数</strong> ：均一な値。</li></ul>操作は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>より小さい</strong> :ソース（左のドロップダウン）の値がターゲット（右のドロップダウン）の値より小さい場合、マスクに白い値が出力されます。</li><li data-preserve-html="true"><strong>許容範囲内</strong> :ソース（左のドロップダウン）の値がターゲット（右のドロップダウン）の値と類似している場合、マスクに白い値が出力されます。</li><li data-preserve-html="true"><strong>より大きい</strong> :ソース（左のドロップダウン）の値がターゲット（右のドロップダウン）の値より大きい場合、マスクに白い値が出力されます。</li></ul> |
| **定数** | 比較設定が「定数」に設定されている場合に比較する値。 |
| **硬さ** | マスクを比較して得られるSmoothness/硬さを制御します。 |
| **ソースチャンネルのヒストグラム** | ソースとターゲットのヒストグラムビューを提供します。 ヒストグラムが少し重なっているかどうか（重なっていない場合はマスクが空になります）を知っておくと便利です。ヒストグラムの機能の詳細については、[レベル](https://experienceleague.adobe.com/ja/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/atomic-nodes/levels)を参照してください。 |

>[!NOTE]
>
> レイヤーを右クリックし、ショートカット「**Heightの組み合わせでマスクを追加**」を選択すると、この新しい効果をレイヤーにすばやく追加できます。 この操作を行うと、Heightチャンネル&#x200B;**描画モード**&#x200B;が、デフォルトの「**覆い焼き（リニア）**」ではなく「**通常**」に切り替わります。\
> ![](../../assets/compare-shortcut.png)
