---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.html"
breadcrumb-title: ''
description: Substance 3D Painterで安定したレンダリングとパフォーマンスを実現するためのGPUドライバーの互換性要件について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPUドライバーの互換性
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 2%

---


# GPUドライバーの互換性

このページでは、Substance 3D Painterの問題の原因になりかねないGPUドライバーに関する情報を再編成します。

## Nvidia

次の表に、Nvidia GPU（GeForceまたはQuadroモデル）の問題を発生させるために知られているすべてのドライバーバージョンを示します。

| *ドライバーバージョン* | *問題の説明* |
| --- | --- |
| <b> 425.xx </b> | GPU レイトレーシングの斑点 |
| <b> 429.xx以前の</b> | 黒いテクスチャブロックの斑点。 |
| <b> 435.xx以前の</b> | テクスチャの計算時にsRGBカラーの問題が発生する。 |
| <b> 439.xx </b> | テクスチャが破損しています。 |
| <b> 441.08 </b> | クラッシュまたは安定性の問題。 |
| <b> 442.19 </b> | クラッシュまたは安定性の問題。 |
| <b>528.09</b> | オペレーティングシステムがフリーズする。 |
| <b>572.16 ～ 572.42</b> | テクスチャのベイク処理時に斑点またはクラッシュが発生する。 |

### AMD

| *ドライバーバージョン* | *問題の説明* |
| --- | --- |
| **20.7.x** ～ **20.11.2** | テクスチャのグリッチまたは破損。 |
| **20.11.3** ～ **21.2.1** | テクスチャの不具合や破損、およびクラッシュや安定性の問題。 |
| **21.2.3** ～ **21.6.1** | クラッシュまたは安定性の問題。 |
