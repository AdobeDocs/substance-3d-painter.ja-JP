---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/multi-bi-gpu.html"
breadcrumb-title: ''
description: Substance 3D PainterをマルチGPUおよびBi-GPUシステム用に設定して、レンダリングパフォーマンスを最適化する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > MultiBi-GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MultiBi-GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---


# マルチ/Bi-GPU

一部のGPU構成やGPUモデルは、Substance 3D Painterと互換性がなく、不安定になったり、クラッシュしたりする場合があります。 互換性のない設定を以下に示します。

| ***構成*** | ***解決策*** |
| --- | --- |
| **Nvidia SLI/AMD Crossfire** （グラフィックカードブリッジ） | GPUドライバー設定で、 SLIまたはCrossfireを無効にします。 |
| **Bi-GPU** （1枚のグラフィックカードに2つのGPUチップセット） | ドライバーの設定で、2つのGPUチップセットの使用を1つのみに無効にします。 |
