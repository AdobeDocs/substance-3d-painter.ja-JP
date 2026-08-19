---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: Substance 3D Painterを有効にし、ライセンスを管理して、テクスチャペイント用のアプリケーションの使用を開始する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ライセンス認証とライセンス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# ライセンス認証とライセンス

このページでは、Painterの使用を開始できるように、ライセンスをアクティベートして管理する方法について説明します。

## アプリケーションタイプごとのアクティベーションプロセス

アクティベーションプロセスは、Painterをどこから購入したか、またはどこからアクセスできるかによって異なります。

| アプリケーションタイプ | アクティベーションプロセス |
| --- | --- |
| Creative Cloud デスクトップ | [HelpXドキュメント](https://helpx.adobe.com/jp/download-install/using/download-creative-cloud-apps.html)の専用ページを参照してください。 問題が発生した場合、[Creative Cloudのドキュメント](https://helpx.adobe.com/jp/creative-cloud/user-guide.html)に詳細な回答が記載されている場合があります。 |
| スチーム | Steamライブラリから直接製品を起動します。 |
| Substance 3Dスタンドアロン | 以下のアクティベーションプロセスを参照してください。 |

## スタンドアロンアクティベーションの手順

### ライセンス認証ウィザード

ライセンス認証ウィザードは、特定の旧バージョンのSubstance 3D Painterで表示されます。

2022年9月30日より前にSubstance 3D webサイトからダウンロードした永続ライセンス版のファイルがある場合でも、アクティベーションウィザードを使用して対象バージョンのSubstance 3D Painterをライセンス認証できます。 [従来のSubstanceライセンスとアカウントについて詳しくは、こちらを参照してください。](https://substance3d.adobe.com/faq-end-of-life-accounts/)

![](../assets/activation-wizard.png){width="350px"}

ライセンス認証ウィザードには、次の3つのオプションがあります。

* <b>この製品の評価</b> ：従来の体験版は利用できなくなりました。 代わりに、[Substance 3Dアプリケーションごとに30日間の無料体験をここから](https://www.adobe.com/jp/products/substance3d/free-trial-download.html?msockid=35568f9be2b964ec22d09c04e3eb65af)またはCreative Cloudデスクトップから開始できます。
* <b>ライセンスファイルを使ってライセンス認証する</b>: 2022年9月30日より前にSubstance 3D Webサイトのアカウントページからダウンロードしたライセンスファイル(<b>\*.key</b>)を使って製品をライセンス認証します。
* <b>アカウントを使用したライセンス認証</b> ：従来のSubstanceアカウントはライセンス認証に使用できなくなりました。

>[!WARNING]
>
> ライセンス認証ウィザードを使用してライセンスファイルをインストールするには、Painterを管理者として実行し、アンチウイルスを一時的に無効にしてください。

### 手動アクティベーション

次のフォルダーにlicense.keyファイルを置くことで、Substance Painterを手動でアクティベートできます。

>[!NOTE]
>
> ファイルの名前が&#x200B;**license.key**&#x200B;であることを確認してください。名前が指定されていない場合、アプリケーションはファイルを見つけることができません。

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Platform</th><th>バージョン</th><th colspan="2">パス</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong>以降</td><td colspan="1">アプリデータ（ローカル）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">アプリデータ（ローミング）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">レガシー</td><td colspan="1">アプリデータ（ローカル）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">アプリデータ（ローミング）</td><td colspan="1">C:\Users\[ユーザー名]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="2">/Users/[ユーザー名]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">レガシー</td><td colspan="2">/Users/[ユーザー名]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="2">/home/[ユーザー名]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>レガシー</td><td colspan="2">/home/[ユーザー名]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> 上記のパスの一部のディレクトリは、デフォルトで非表示になっている場合があります。 ファイルエクスプローラーでパスを手動で入力するか、隠しファイルを表示して表示します。

### 環境変数

Painterが&#x200B;**license.key**&#x200B;ファイルをチェックする場所は、[環境変数](../pipeline-and-integration/configuration/environment-variables.md)で上書きできます。
