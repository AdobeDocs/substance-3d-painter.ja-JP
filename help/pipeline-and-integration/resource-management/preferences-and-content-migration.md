---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/preferences-and-content-migration.html"
breadcrumb-title: ''
description: 新しいシステムにアップグレードまたは移行する際に、Substance 3D Painterで環境設定とコンテンツを移行する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Preferences and content migration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 環境設定とコンテンツの移行
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---


# 環境設定とコンテンツの移行

このページでは、環境設定およびシェルフ/アセットからデータを移行して、新しいバージョンで使用する方法について説明します。

バージョン7.2のリリース後、複数のバージョンのアプリケーション（Substance 3Dスタンドアロン、Steam、およびCreative Cloudデスクトップ）で共通にできるように、環境設定とシェルフの場所が変更されました。 この変更により、以前の環境設定とカスタムリソース&#x200B;**が既定で無視されるようになりました** （**ただし、失われていません**）。 **シェルフ**&#x200B;の名前が&#x200B;**アセット**&#x200B;に変更されたため、移行には以下に示すいくつかの手順が必要です。

## シェルフとアセットのリソースの移行

デフォルトのユーザーのリソースの場所が変更されました。つまり、文書フォルダーに入れられたコンテンツは、アプリケーションの新しいバージョンでは無視されるようになりました。 このコンテンツを復元するには、ファイルをある場所から別の場所に移動するだけです。

### コンテンツの場所

シェルフパスまたはアセットパスは次の場所にあります。

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Platform</th><th>バージョン</th><th>パス</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong>以降</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">レガシー</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">レガシー</td><td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>レガシー</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

### シェルフのコンテンツを移行する方法

古いシェルフの内容はディスク上のファイルに過ぎないため、それらのファイルの移行は、単にファイルを適切な場所に配置することだけです。

1. アプリケーションを閉じる
1. 古いシェルフフォルダーに移動します
1. サブフォルダー（アルファ、手続き、マテリアルなど）をコピーまたはカットする
1. 新しいアセットフォルダーに移動します
1. 以前にコピーしたサブフォルダーをAssetsフォルダー内にペーストし、確認メッセージが表示されたら上書きします。

アプリケーションを再起動すると、コンテンツがアセットウィンドウに表示されます。

>[!NOTE]
>
> リソースの親フォルダーだけでなく、サブフォルダーも必ずコピーしてください。 親フォルダーの名前が&#x200B;**shelf**&#x200B;から&#x200B;**assets**&#x200B;に変更されました。親フォルダーのみをコピーすると、アプリケーションにリソースが表示されなくなります。

### シェルフプリセットを移行する方法

シェルフプリセットは設定ファイル内に保存されます。 これらのプリセットを移行するには：

1. アプリケーションを閉じる
1. 古いシェルフフォルダーに移動します
1. Shelf.iniファイルのコピーまたはカット
1. 新しいアセットフォルダーに移動します
1. ファイルをペーストして既存のファイルを上書き

アプリケーションを再起動すると、保存された検索が専用セクションまたはアセットウィンドウに表示されます。

## 環境設定の移行

アプリケーション設定は、インターフェイスから手動で再調整することをお勧めします。 これは、互換性の問題を発生させることなく情報を移行するための最も安全な方法です。

それ以外の場合は、次のページを参照して、環境設定の場所を確認してください： [環境設定とアプリケーションデータの場所](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html)。
