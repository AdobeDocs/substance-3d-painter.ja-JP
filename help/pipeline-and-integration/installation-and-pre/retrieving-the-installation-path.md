---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: Substance 3D Painterのインストールパスを取得して、スクリプトを作成したり、パイプラインを統合したりする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: インストールパスの取得
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 6%

---


# インストールパスの取得

このページでは、バージョンおよびプラットフォームに応じてアプリケーションのインストールパスを取得する方法に関する情報を再編成します。

## Windows

### Creative Cloud デスクトップ

1. Windowsレジストリエディター(**regedit**)を開きます。
1. レジストリキーに移動します： ** HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Paths\**
1. **Adobe Substance 3D Painter.exe**&#x200B;というサブキーを開きます
1. キーの値には、インストールされているアプリケーションの実行可能ファイルへのパスが含まれています

>[!NOTE]
>
> このレジストリキーは、バージョン7.2以降でのみ使用できます。\
>  古いバージョンの場合、インストールパスは&#x200B;**HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts**&#x200B;のファイル関連付けから取得できます。

### Substance 3D Standalone

1. Windowsレジストリエディター(**regedit**)を開きます。
1. レジストリキー&#x200B;**HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**&#x200B;に移動します
1. アプリケーションバージョンのAppIDに一致するサブキーを見つけます（以下の表を参照）
1. キーの値には、アプリケーションのインストール場所へのパスが含まれています

| バージョン | AppId |
| --- | --- |
| **バージョン1.x** | `{410F5B6E-A29C-4F43-9DE3-44A1357D6AF5}` |
| **バージョン2.x** | `{f42b7a996fa1d13a1d0a2e33eea2c0800bb5d1b8}` |
| **3.x (2017.x) ～ 7.1** | `{33C3E9E2-0675-4196-9019-28AB9C5E9BB0}` |
| **7.2以降** | `{2a8bbb68-725b-477c-9194-60efc5ece348}` |

### スチーム

アプリケーションは、Steamインストールフォルダーの&#x200B;**steamapps/common/**&#x200B;サブフォルダーにインストールされます。

## Mac

Macでは、アプリケーションは次の場所にインストールされます。

| バージョン | パス |
| --- | --- |
| **7.2以降** | **/Applications/Adobe Substance 3D Painter.app** |
| **レガシ** | **/Applications/Substance Painter.app** |

## Linux

Linuxでは、rpmパッケージは次のパスにインストールされています。

| バージョン | パス |
| --- | --- |
| **7.2以降** | **/opt/Adobe/Adobe\_Substance\_3D\_Painter** |
| **レガシ** | **/opt/Allegorithmic/Substance\_Painter** |
