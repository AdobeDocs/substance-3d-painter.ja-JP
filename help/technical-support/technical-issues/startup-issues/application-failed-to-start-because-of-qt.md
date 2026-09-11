---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/application-failed-to-start-because-of-qt.html"
breadcrumb-title: ''
description: Qtフレームワークの問題が原因で発生したSubstance 3D Painterの起動エラーを修正し、アプリケーションを適切に起動する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Application failed to start because of Qt
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Qtが原因でアプリケーションを開始できませんでした
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# Qtが原因でアプリケーションを開始できませんでした

アプリケーションの起動時に、次のエラーメッセージが表示される場合があります。

>> 

Qtプラットフォームプラグインを初期化できなかったため、このアプリケーションは開始できませんでした。 アプリケーションを再インストールすると、この問題が解決する場合があります。

利用可能なプラットフォームプラグインは、最小、オフスクリーン、webgl、windowsです。

このエラーは、アプリケーションと競合する別のソフトウェア定義の環境変数が原因で発生する可能性があります。

アプリケーションを起動する前に、現在の環境から以下の変数を削除してください。

```
QT_PLUGIN_PATH 

QML2_IMPORT_PATH
```


>[!NOTE]
>
> これらの変数は、**pyinstaller**&#x200B;などを使用して、Pythonコンテキストから継承することもできます。 これらは、アプリケーションが起動されたコンテキストから必ず削除してください。
