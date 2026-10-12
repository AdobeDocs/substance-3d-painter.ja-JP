---
breadcrumb-title: ""
description: Substance 3D Painterのインストールを自動化して、エンタープライズデプロイメントとパイプライン統合のワークフローを実現する方法について説明します。
title: 自動インストール
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%
---

# 自動インストール

Substance 3Dスタンドアロンインストーラーを使用する場合は、アプリケーションをサイレントモードでインストールして簡単にデプロイできます。

**InnoSetup**&#x200B;を使用してインストーラーを生成しています。 インストーラーで使用できるパラメーターのセット全体は、[ここ](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline)から取得できます。

## コマンドラインによるサイレントモードでのインストール

サイレントインストールの実行に使用するフラグは&#x200B;**/SILENT**&#x200B;です。 フラグ&#x200B;**/NCRC**&#x200B;を使用してパッケージのCRC （検証）をスキップして、プロセスを高速化することもできます。

例：

```
SubstancePainter_Installer.exe /NCRC /SILENT /DIR="C:InstallationFolder"
```


>[!NOTE]
>
> フォルダーを区切るには、インストールパスに円記号を1つ付ける必要があります。円記号を1つ付けない場合、インストーラーはパスを認識しません。
