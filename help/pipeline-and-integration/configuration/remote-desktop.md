---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/pipeline-and-integration/configuration/remote-desktop.html"
breadcrumb-title: ''
description: リモートワークフローと共同作業を有効にするためにリモートデスクトップアクセス用にSubstance 3D Painterを設定する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Remote Desktop
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: リモートデスクトップ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# リモートデスクトップ

ここでは、Windowsのリモートデスクトップ(RDP)経由でSubstance 3D Painterを実行できるようにするソリューションと代替方法について説明します。

デフォルトでは、Windows上のRDPは、存在しないか低すぎるOpenGLコンテキストで実行されるため、アプリケーションが正しく動作しないか、クラッシュします。 Substance 3D PainterにはOpenGL 3.3コンテキストが必要です。 以下は問題を軽減する解決策ですが、最初の問題はWindowsと一部のGPUドライバーに依存しているため、機能する見栄えはありません。

>[!NOTE]
>
> Nvidia Quadro GPUはデフォルトでRDPモードでアプリケーションを実行できますが、Nvidia GeForce GPUはOpenGL 1.4コンテキストのみを提供します（これはSubstance 3D Painterには低すぎます）。 この問題を解決するために、実行可能ファイルをインストールすることができます。参照： <https://developer.nvidia.com/designworks>

## Windowsポリシーの構成

Windows 10では、RDPモードでGPUを実行できるように&#x200B;**グループポリシー**&#x200B;を変更する必要がある場合があります。

次の操作を行います。

1. **Win + R**&#x200B;を押して、実行ウィンドウを開きます
1. 「 **gpedit.msc** 」と入力してから、
1. **ローカルコンピューターポリシー\コンピューターの構成\管理用テンプレート\Windowsコンポーネント\リモートデスクトップサービス\リモートデスクトップセッションホスト\リモートセッション環境**&#x200B;に移動します
1. オプション&#x200B;**すべてのリモートデスクトップサービスセッションでハードウェアの既定のグラフィックスアダプターを使用する**&#x200B;を有効にします。

## Windows TSCONコマンド

以前のポリシー変更が機能しない場合は、**tscon**&#x200B;コマンドラインを使用できます。 このコマンドは、リモートコンピューターを切断し、新しいリモートコンピューターを物理ハードウェア（マウス、キーボードなど）に接続します。 アプリケーションを実行してリモートで再接続するだけで、GPU上のアプリケーションを操作できます。

1. キー&#x200B;**Windows+R**&#x200B;を押して、**実行**&#x200B;ウィンドウを開きます。
1. **cmd**&#x200B;と入力して、 **Enter**&#x200B;を押します。
1. コマンドラインに次のコマンドを入力します： **tscon 1 /dest:console**
1. Enterキーを押します
1. コマンドラインで次のコマンドを入力します： **start &quot;Path/To/Folder/Painter/Folder/Substance 3D Painter.exe&quot;**（Substanceに合わせてパスを変更してください）
1. Enterキーを押します

これらの手順の後、数秒間待ってアプリケーションが起動してから、セッションに再接続します。

この手順が機能しない場合は、管理者モードでWindowsコマンドラインを実行する必要があります。

## 代替手段

それでも前の提案が機能しない場合は、リモート接続を介したGPUをサポートするVNCやTeamviewerなどの代替ソリューションを使用することをお勧めします。
