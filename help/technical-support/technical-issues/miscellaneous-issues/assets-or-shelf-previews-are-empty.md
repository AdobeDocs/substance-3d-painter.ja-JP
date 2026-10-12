---
breadcrumb-title: ""
description: Substance 3D Painterで空のアセットとシェルフのプレビューを修正し、サムネールの表示機能を復元する方法について説明します。
title: アセット（またはシェルフ）のプレビューが空です
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%
---

# アセット（またはシェルフ）のプレビューが空です

この問題は、他のソフトウェアが原因である可能性があります。[ソフトウェアの競合](../startup-issues/software-conflicts.md)を参照してください。

どのソフトウェアをアップデート/アンインストールするかを判断できない場合は、「QT\_PLUGIN\_PATH」という名前の環境変数を探して削除します。

**Windowsの場合：**

1. コントロールパネルの&#x200B;**システム**&#x200B;を開きます。
1. [詳細設定]タブで、[**環境変数**]をクリックします
1. **&quot;QT\_PLUGIN\_PATH&quot;**&#x200B;という名前の変数を探します
1. **削除**
1. コンピューターを&#x200B;**再起動**
