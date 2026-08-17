---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/blocky-artifacts-appear-on-textures-in-the-viewport.html"
breadcrumb-title: ''
description: Substance 3D Painterのビューポートでテクスチャに表示される濃淡のむらが出て、すっきりとした画質を実現する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Blocky artifacts appear on textures in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ビューポートのテクスチャに濃淡のむらが出る
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# ビューポートのテクスチャに濃淡のむらが出る

バージョン2018.3.0以降では、ビューポートに次のようなアーティファクトが表示される場合があります。

![](../../../assets/viewport-artifacts.jpg){width="400px"}

これらのアーティファクトは、Nvidia GPUドライバーの問題に関連しています。\
アーティファクトを回避するには、Sparse Virtual Texturesハードウェアサポートを非アクティブにする必要があります。

GeForce **ドライバー440.97**&#x200B;は現在、**この問題を修正**&#x200B;しました。 アドビでは、これらのドライバーを更新し、良好なパフォーマンスを得るためにSVTを有効にしておくことをお勧めします。

新しいドライバーはNVIDIA Webサイトで入手できます： <https://www.nvidia.com/Download/index.aspx>

## スパース仮想テクスチャハードウェアアクセラレーションを無効にする

### 1 - Substance 3D Painterを起動し、設定を開きます。

![](../../../assets/settings-34.png)

編集/設定を選択して、メインの「設定」を開きます。

### 2 - 「スパース仮想テクスチャ」という名前のセクションを見つけます。

![](../../../assets/svt-subsection.png)

「一般」セクション内を下にスクロールして、「スパース仮想テクスチャ」という名前のサブセクションを見つけます

### 3 – 設定をオフにする

![](../../../assets/uncheck-hardware.png)

チェックを外して、「ハードウェアサポートアクセラレーション」設定を無効にします。

### 4 - Substance 3D Painterを検証して再起動します

![](../../../assets/validate-1.png)

「OK」ボタンをクリックして、変更を検証します。

![](../../../assets/restart-3.png)

「はい」をクリックしてSubstance 3D Painterを再起動し、変更内容を適用します。
