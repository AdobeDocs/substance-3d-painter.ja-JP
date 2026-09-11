---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/workflow-issues/license-issues/maintenance-is-expired-dialog-on-startup.html"
breadcrumb-title: ''
description: ライセンス管理用に、Substance 3D Painterの起動時に表示されるメンテナンスの期限切れダイアログを解決する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > License Issues > Maintenance is expired dialog on startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 起動時の「メンテナンスの期限が切れました」ダイアログ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---


# 起動時の「メンテナンスの期限が切れました」ダイアログ

![](../../../assets/expired-mainteance-message.png)

アプリケーションを起動すると、「現在のメンテナンスの期限が切れました」というメッセージを含むダイアログが表示される場合があります。 このページでは、このダイアログを回避する方法の解決策について説明します。

## 解決策1：ライセンスファイルを更新する

ライセンスファイルが古すぎるため、更新する必要があるため、警告メッセージが表示されます。 これを行うには、アプリケーションウィザードを使用して&#x200B;**製品を再アクティベート**&#x200B;するだけです。 ライセンスファイルは、Substance 3D webサイト<https://www.substance3d.com/>から手動でダウンロードすることもできます。

## 解決策2：環境設定を編集してダイアログを非表示にする

>[!NOTE]
>
> この代替ソリューションを使用する前に、まずライセンスファイルを更新することをお勧めします。

別の解決策として、特定の設定を配置して警告メッセージを非表示にすることもできます。

アプリケーションの環境設定の場所に移動します。

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>システム</th><th>バージョン</th><th>パス</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>（登記簿）</p></td><td><strong>7.2</strong>以降</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>レガシー</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>（図書館）</p></td><td><strong>7.2</strong>以降</td><td>/Users/[ユーザー名]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>レガシー</td><td>/Users/[ユーザー名]/Library/Preferences/com.substance3d.user.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong>以降</td><td>/home/[ユーザー名]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>レガシー</td><td>/home/[ユーザー名]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

### Windows

Windowsで変数を設定するには、次の手順に従います。

1. [スタート]メニューを開きます。
1. **Regedit**&#x200B;を検索して、レジストリエディターを開きます。
1. 上記の表に示したレジストリキーに移動します。
1. 左側のツリー表示で、ソフトウェアとして名前が付けられたレジストリキーをクリックします。
1. 右側のパネルの空の領域を右クリックして、**新規/文字列値**&#x200B;を選択します。
1. 新しい値に&#x200B;**DisableLicenseWarningPopup**&#x200B;という名前を付け、Enterキーを押して検証します。
1. 作成した値をダブルクリックします。
1. 値データフィールドを&#x200B;**true**&#x200B;に設定します
1. 変更内容を保存します。
1. アプリケーションを起動します。

### MacOS

1. 新しい&#x200B;**Finder**&#x200B;ウィンドウを開く
1. 上の表に示されたパスに移動します。
1. **plist**&#x200B;ファイルを右クリックして、**プログラムから開く/Xcode**&#x200B;を選択します。
1. 一覧の先頭に、**DisableLicenseWarningPopup**&#x200B;という名前の新しいキーを追加します
1. キーの種類を&#x200B;**文字列**&#x200B;に設定します
1. キーの値を&#x200B;**true**&#x200B;に設定します
1. ファイルを保存して閉じます。
1. アプリケーションを起動します。

### Linux

Linuxで変数を設定するには、次の手順に従います。

1. 上の表のパスリストに移動します。
1. フォルダーにある&#x200B;**.conf**&#x200B;ファイルを開きます。
1. **[全般]**&#x200B;行の下に新しい行を追加します
1. 新しい行に次のテキストを貼り付けます： **DisableLicenseWarningPopup=true**
1. ファイルを保存します。
1. アプリケーションを起動します。
