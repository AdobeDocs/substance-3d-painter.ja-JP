---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/technical-issues/rendering-issues/some-hdpi-scaling-values-are-not-working.html"
breadcrumb-title: ''
description: 高解像度ディスプレイを適切にサポートするために、Substance 3D PainterでHDPIスケール値に関する問題を修正する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Some HDPI scaling values are not working
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 一部のHDPIスケール値が機能しない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---


# 一部のHDPIスケール値が機能しない

Windowsでは、一部のHDPIスケール値（高解像度モニターのインターフェイスの拡大/縮小に使用される値）が正しく機能しない場合があります。\
これは、ウィンドウフレームワーク(Qt)がサポートしていないためです。 フレームワークのプロバイダーによって実際に管理されるまで、修正することはできません。

そのため、設定によっては次のような動作が発生する場合があります。

* 120 DPI （**125%**&#x200B;スケーリング） - 96 DPIとしてレンダリング（**100%**&#x200B;スケーリング）
* 144 DPI （**150%**&#x200B;スケーリング） - 192 DPIとしてレンダリング（**200%**&#x200B;スケーリング）
* 168 DPI （**175%**&#x200B;スケーリング） - 192 DPIとしてレンダリング（**200%**&#x200B;スケーリング）

詳細については、<https://bugreports.qt.io/browse/QTBUG-55654>を参照してください。
