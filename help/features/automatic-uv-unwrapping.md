---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/automatic-uv-unwrapping.html"
breadcrumb-title: ''
description: Substance 3D Painterで自動UVラップ解除を使用して、3DモデルのUVレイアウトを自動的に生成する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Automatic UV Unwrapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UVの自動ラップ解除
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# UVの自動ラップ解除

![](../assets/auto-unwrap-update-810.jpg)\
自動UVアンラップを使用すると、3Dモデルの読み込み時にUV アイランドを自動的に生成できます。 既存のUVがない3Dモデル上でペイントするために使用できます。

## 自動ラップ解除の有効化

![](../assets/uv-new-project.png)

新しいプロジェクトを作成したり、既存のプロジェクトにメッシュを再読み込みする場合は、「自動ラップ解除」設定がオンになっていることを確認してください。 無効にすると、プロセスがスキップされ、メッシュUVはそのままの状態が維持されます。

## UVアンラップ設定

![](../assets/unwrap-settings.png)

メッシュを読み込み、ラップ解除プロセスを使用する場合、次の設定を使用できます。 一部の設定は、インターフェイスのオプションボタンから利用できます。

| セクション | ***設定*** | ***説明*** |
| --- | --- | --- |
| **シーケンスのラップ解除** | **シーム** | シーム（UV アイランドの枠線）を持たないメッシュに対してのみ生成するか、常に再生成するかを制御します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>不足しているデータを生成します</strong> （既定）：不足しているメッシュに対してシームが生成されます。</li><li data-preserve-html="true"><strong>すべての</strong>を再計算：すべてのメッシュに対して縫い目が生成されます。</li></ul> |
| **UV アイランド** | UVのないメッシュから、または任意のメッシュに対して、UVラップ解除を生成するかどうかを制御します。 有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>不足しているデータを生成します</strong> （既定）: UVのないメッシュに対してUVアンラップが生成されます。</li><li data-preserve-html="true"><strong>すべての</strong>を再計算：すべてのメッシュのUVラップ解除が生成されます。</li></ul> |  |
| **パッキング** | メッシュのUV アイランドのパッキング/レイアウトを制御します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>不足しているデータを生成します</strong> （既定）: UVが不足しているメッシュのUV アイランドをパックします。</li><li data-preserve-html="true"><strong>すべての</strong>を再計算：すべてのUV アイランドをパックします。</li></ul> |  |
|  |  |  |
| **レイアウトのカスタマイズ** | **余白サイズ** | UV アイランド間の間隔を指定します。 この設定は、解像度とは無関係に一般的なパーセンテージを適用します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>余白なし</strong> : 0%</li><li data-preserve-html="true"><strong>小</strong> （既定）: 0.2%</li><li data-preserve-html="true"><strong>中</strong> : 0.5%</li><li data-preserve-html="true"><strong>大</strong> : 1%</li></ul> |
|  | **UV アイランドの向き** | パッキングプロセス中のUV アイランドの方向を制御します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>制約なし</strong> （既定）：方向の計算に制約は適用されません。</li><li data-preserve-html="true"><strong>3D メッシュに合わせる</strong>:UV アイランドの方向がメッシュの方向を向くように制限します</li></ul> |
|  |  |  |
| **UV タイル** | **最大UV タイル数** | 「UVタイル」ワークフローが有効な場合、この設定によって、UV アイランド上に分布するために生成するタイルの最大数が決まります。 |
|  |  |  |
| **最適化** | **細長いUV アイランドを避ける** | 有効にすると、このプロセスにより、長すぎると見なされるUV アイランドが分割され、テクスチャ容量の使用量が増えます。before（上）とafter（下）の例： <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r10-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../assets/uv-before-after.jpg" width="400px"/></div> |

## 既知の制限

ラップ解除プロセスに関する制限事項を以下に示します。

* 高ポリゴンメッシュの処理には時間がかかる場合があります。
* まったく同じ座標にある頂点が結合されます
* まれに、一部のメッシュパーツでUV生成が失敗することがあります
* 1回のUV アイランドで、不均一または大幅に歪んだテキセル比が発生する場合がある
* テクスチャセット間の均一なテキセル比
* 生成されるUV アイランドは非常に長くなることがあり、場合によってはUV空間に収まらないことがあります
* 縮退した面または小さなエッジや重なり合うエッジを持つ三角形でないメッシュ面は、UVをラップ解除できない場合があります
