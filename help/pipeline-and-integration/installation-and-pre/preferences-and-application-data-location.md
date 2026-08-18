---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/pipeline-and-integration/installation-and-preferences/preferences-and-application-data-location.html"
breadcrumb-title: ''
description: Substance 3D Painterで設定やユーザーデータを管理するための環境設定とアプリケーションデータの場所について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Preferences and application data location
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 環境設定とアプリケーションデータの場所
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 4%

---


# 環境設定とアプリケーションデータの場所

このページでは、バージョンおよびプラットフォームごとにアプリケーションの環境設定が保存される場所に関する情報を再編成します。\
**カスタムシェルフ** （スタジオインストールの場合）を追加する場合や、アプリケーションの&#x200B;**クリーンインストール**&#x200B;を実行するために、これらの環境設定を削除する場合に備えて、環境設定の保存場所を知っていると便利です。

## 環境設定

このパスは、アプリケーション環境設定（保存されたショートカット、シェルフ/アセットパス、インターフェイスレイアウトなど）の場所です。

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>システム</th><th>バージョン</th><th>パス</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>（登記簿）</p></td><td><strong>7.2</strong>以降</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>レガシー</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>（図書館）</p></td><td><strong>7.2</strong>以降</td><td>/Users/[ユーザー名]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>レガシー</td><td>/Users/[ユーザー名]/Library/Preferences/com.substance3d.user.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong>以降</td><td>/home/[ユーザー名]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>レガシー</td><td>/home/[ユーザー名]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

## アプリケーションデータ

このパスは、追加のアプリケーションデータ（アセットのサムネール、ログファイルなど）の場所です。

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Platform</th><th>バージョン</th><th colspan="2">パス</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong>以降</td><td colspan="1">アプリデータ（ローカル）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">アプリデータ（ローミング）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">レガシー</td><td colspan="1">アプリデータ（ローカル）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">アプリデータ（ローミング）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="2">/Users/[ユーザー名]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">レガシー</td><td colspan="2">/Users/[ユーザー名]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="2">/home/[ユーザー名]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>レガシー</td><td colspan="2">/home/[ユーザー名]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> 上記のパスの一部のディレクトリは、デフォルトで非表示になっている場合があります。 ファイルエクスプローラーでパスを手動で入力するか、隠しファイルを表示して表示します。
