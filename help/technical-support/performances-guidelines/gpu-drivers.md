---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/performances-guidelines/gpu-drivers.html"
breadcrumb-title: ''
description: レンダリングのパフォーマンスと安定性を最適化するための、Substance 3D PainterのGPU VRAMおよびドライバー要件について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > GPU Drivers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU VRAMおよびドライバー
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# GPUドライバー

推奨ドライバーを使用しない限り、パフォーマンスは保証されません。 WHQL以外のドライバは避ける必要があります。\
GPUドライバーは他のソフトウェアと同様に、リリースが変わるたびにパフォーマンスの問題が発生する可能性があります。 新しいバージョンに更新した後に問題が発生した場合は、ドライバーを以前のバージョンにダウングレードすることをお勧めします。

## NVIDIAドライバー設定

一部のデフォルトNVIDIA設定はパフォーマンスに影響を与える可能性があります。プロファイルを作成して、次のパラメーターを無効にすることを推奨します（オフに設定します）。

* スレッド最適化
* 垂直同期

## 他のアプリケーションでGPUを利用する方法

GPUの操作にSubstance 3D Painterだけではなく、他のアプリケーションも同じ処理を行います。 Blender、Maya、Unreal Engine、Unity、C4Dなど、Painterと一緒に使用される一般的なアプリケーションも含め、ほとんどの3DアプリケーションはGPUとVRAMを使用して実行されます。 これらのアプリケーションを開いたまま良好なパフォーマンスを維持するためのソリューションは、独自のVRAM割り当てをリクエストするために、Substance 3D Painterが最初に起動されることを確認することです。 ただし、一部のソフトウェアはVRAMの一部を動的に読み込むことができ、Painterの後に起動した場合でもSubstance 3D Painterと競合する可能性があります。

一般に、PainterがアクセスできるVRAMの量が多いほど、実行速度が速くなるので、Painterと同時に実行する他のアプリケーションが使用するVRAMの量を最小限に抑えるようにしてください。

## GPU VRAMの量と帯域幅

Substance 3D Painterでは、ほとんどの計算をGPUに依存して実行します。 このため、[必要システム構成](../../getting-started/system-requirements.md)に準拠したGPUを用意することが重要です。

Painterでは、計算処理（最終的なテクスチャを作成するブレンド処理など）を行うために、テクスチャをGPUメモリ(VRAM)に転送します。 ただし、VRAMの空き容量が不足し始めた場合、未使用のテクスチャがコンピューターのRAMに転送され、VRAMの空き容量が増えます。 Substance 3D Painterは、作業中にGB分のデータの書き込みと読み取りを行います。 つまり、VRAMの容量（容量）と転送時の帯域幅速度の両方が重要になります。 [MSI AfterBurner](https://www.msi.com/page/afterburner)などのツールを使用して、この動作を監視できます。

>[!NOTE]
>
> <b>Nvidia GTX 970</b>には、Substance 3D Painterに影響を与えるGPUメモリに関する問題のあるデザインがあることが知られています。 4 GB全体の最後の500 MBは、残りの3.5 GBよりも低速で動作します。 Substance 3D Painterが最後の500 MBで動作する場合、パフォーマンスは（測定した値から）10倍も低下する可能性があります。 技術的な詳細については、<https://www.pcper.com/news/Graphics-Cards/NVIDIA-Responds-GTX-970-35GB-Memory-Issue>を参照してください。
