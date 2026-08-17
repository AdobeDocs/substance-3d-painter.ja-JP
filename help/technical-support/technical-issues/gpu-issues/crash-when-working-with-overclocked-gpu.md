---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/crash-when-working-with-overclocked-gpu.html"
breadcrumb-title: ''
description: アプリケーションのパフォーマンスを安定させるため、オーバークロックされたGPUで作業している際にSubstance 3D Painterがクラッシュする問題の解決方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Crash when working with overclocked GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: オーバークロックされたGPUの操作中にクラッシュする
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# オーバークロックされたGPUの操作中にクラッシュする

オーバークロックされたGPUは、多くの場合、GPUコンストラクターによって最初に設計されなかった周波数で実行されるため、不安定になります。 GPUがオーバークロックされていて、安定性の問題がある場合は、しばらく工場出荷時のデフォルトの周波数に戻すことをお勧めします。

## Nvidia GPU

ドライバー355.82以降のNVIDIA GPUでは、ドライバー設定でデバッグモードを有効にすることで、GPUオーバークロックを一時的に無効にすることができます。 これにより、グラフィックカードに関連する問題を確認および判定できます。

デバッグモードを有効にするには：

1. **Nvidiaコントロールパネル**&#x200B;を開きます（デスクトップを右クリックします）。
1. **ヘルプ**&#x200B;メニューをクリックします。
1. **デバッグモード**&#x200B;をクリックします。

>[!NOTE]
>
> GPUがリファレンスカードの場合、デバッグモードが使用できない場合があります。 GPUが非標準クロックで動作している場合、またはBIOSが変更されている場合にのみ使用できます。 この場合、オーバークロックを手動で無効にすることをお勧めします。
