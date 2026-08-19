---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/impossible-to-use-the-alt-keyboard-shortcut-on-linux.html"
breadcrumb-title: ''
description: Substance 3D PainterのLinuxでALTキーボードショートカットの問題を解決して、キーボードを適切に操作する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Impossible to use the ALT keyboard shortcut on Linux
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: LinuxでALTキーボードショートカットを使用できない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# LinuxでALTキーボードショートカットを使用できない

**Gnome**&#x200B;をユーザーインターフェイスとして使用するLinuxディストリビューション（**Ubuntu**&#x200B;または&#x200B;**CentOS**）を実行している場合は、**ALT**&#x200B;キーの既定の動作を無効にして、ビューポート内を移動できるようにすることをお勧めします。

## CentOS

1 - **システム/Windows**&#x200B;に移動します

![](../../../assets/centos-window.png){width="250px"}

2 - 「移動キー」設定を「 **Alt** 」以外に変更します。 例えば、「 **Super** 」を使用します（キーボードの「Windows」キーを選択する場合）。

![](../../../assets/centos-setting.png){width="350px"}

## Ubuntu

1 – ターミナルを開き、次のコマンドを実行します。

```
sudo apt-get install dconf-tools
```


これにより、高度な構成ツールがインストールされます。実行するには、追加の依存関係のインストールを許可する必要がある場合があります。

2 – スタートメニューを開き、「 **Dconf-tools** 」を探します。 起動します。

3 – 左側のツリーメニューを展開するには、次のルートに移動します： **組織/ gnome /デスクトップ/ wm /環境設定**

4 - 「mouse-button-modifier」を編集し、値を変更します。 それを設定するか、または代わりに設定しますが、*空のままにしないでください* 。 Superは、「Windows」キーと同じです。

![](../../../assets/ubuntu-setting.png){width="500px"}
