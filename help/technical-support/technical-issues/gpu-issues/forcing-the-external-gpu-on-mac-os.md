---
breadcrumb-title: ""
description: macOSでSubstance 3D Painterに外部GPUを強制的に使用して、レンダリングパフォーマンスを向上させる方法について説明します。
title: Mac OSでの外部GPUの強制
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%
---

# Mac OSでの外部GPUの強制

Mac OS Mojaveでは、アプリケーションごとに外部GPUを使用するように指定できます。 この設定を有効にすると、Substance 3D Painterのパフォーマンスと安定性が向上する場合があります。

詳細については、[Appleのドキュメント](https://support.apple.com/en-us/HT208544)を参照してください。

有効にするには：

1. Substance 3D Painterを実行中の場合は閉じます。
1. Finderで「Substance 3D Painter」を選択すると、**Applications**&#x200B;フォルダーに格納されてい**す。**
1. **Command-I**&#x200B;を押すか、**Substance 3D Painter**&#x200B;アプリケーションを右クリックして、**情報を取得**&#x200B;を選択します。
1. 新しいウィンドウで、設定「**外部GPUを優先**」を有効にします。
1. Substance 3D Painterを再起動します。

>[!NOTE]
>
> この設定は、eGPUが接続されていない場合、または現在のバージョンのMacOSが古すぎる場合は表示されません。
