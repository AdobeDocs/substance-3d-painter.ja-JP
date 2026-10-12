---
breadcrumb-title: ""
description: Substance 3D PainterをマルチGPUおよびBi-GPUシステム用に設定して、レンダリングパフォーマンスを最適化する方法について説明します。
title: MultiBi-GPU
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%
---

# マルチ/Bi-GPU

一部のGPU構成やGPUモデルは、Substance 3D Painterと互換性がなく、不安定になったり、クラッシュが発生したりします。 互換性のない設定を以下に示します。

| ***構成*** | ***解決策*** |
| --- | --- |
| **Nvidia SLI/AMD Crossfire** （グラフィックカードブリッジ） | GPUドライバー設定で、 SLIまたはCrossfireを無効にします。 |
| **Bi-GPU** （1枚のグラフィックカードに2つのGPUチップセット） | ドライバーの設定で、2つのGPUチップセットの使用を1つのみに無効にします。 |
