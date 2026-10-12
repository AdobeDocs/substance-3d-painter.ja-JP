---
breadcrumb-title: ""
description: GPUが適切にアクセラレーションされるように、Substance 3D PainterでGPU認識に関する問題がGDI一般として表示される問題の修正方法について説明します。
title: GPUが認識されず、GDI一般としてメンションされる
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%
---

# GPUが認識されず、GDI一般としてメンションされる

この問題は追跡が少し複雑で、複数のソースが原因である可能性があります。

* Nvidia Optimusを搭載したコンピューターを使用している場合は、次のリンクを参照してください。[GPUが認識されません](gpu-is-not-recognized.md)
* モニターがプライマリGPUに接続されていること（およびWindowsでこのモニターがメインディスプレイとして設定されていること）を確認します
* Windowsでメインディスプレイのカラービット深度が32ビットに設定されていることを確認します
* それでも問題が解決しない場合は、GPUドライバーをクリーンに再インストールします（完全アンインストール後、Windowsレジストリにある残りの部分をクリーンアップします）。
