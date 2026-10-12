---
breadcrumb-title: ""
description: Substance 3D PainterでGPU認識の問題を修正し、ハードウェアのアクセラレーションとパフォーマンスを適切に動作させる方法について説明します。
title: GPUが認識されない
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%
---

# GPUが認識されない

![](../../../assets/not-recognized-gpu.png){width="500px"}

一部の&#x200B;**NVIDIA Optimus**&#x200B;ユーザーは、適切なGPUでSubstance 3D Painterを実行する際に問題が発生することがあります。 回避策は、Windowsのレジストリで次のキーを0に設定することです。

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
