---
breadcrumb-title: ""
description: より良いパフォーマンスを得るために、統合グラフィックの代わりに専用GPUを使用するようにSubstance 3D Painterを設定する方法について説明します。
title: 統合GPUで実行
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%
---

# 統合GPUで実行

![](../../../assets/integrated-gpu.png){width="500px"}

一部のコンピューターは、デフォルトで専用のGPUではなく、統合チップセットで実行するように設定されています。\
内蔵チップセットのパフォーマンスは非常に低いため、代わりに専用GPUを使用することをお勧めします。 ポップアップが表示され、警告が表示されます。

NVIDIA GPUでは、NVIDIA GPUへの切り替えはアプリケーションプロファイルに依存します。 アプリケーションにこのようなプロファイルがない場合は、グラフィックカードを手動で割り当てることができます。

1. デスクトップを右クリックして、NVIDIAコントロールパネル&#x200B;**または**&#x200B;を選択します。コントロールパネルに移動して、NVIDIAコントロールパネルを検索します。
1. **3D設定**&#x200B;で、**3D設定の管理**&#x200B;に移動します
1. 「**プログラムの設定**」タブで、**Substance 3D Painter**&#x200B;の新しいプロファイルを追加します
1. 優先するグラフィックプロセッサー設定を「高性能NVIDIAプロセッサー」に変更します。
