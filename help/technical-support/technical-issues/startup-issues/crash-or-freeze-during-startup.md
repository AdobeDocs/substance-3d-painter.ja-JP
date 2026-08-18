---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/crash-or-freeze-during-startup.html"
breadcrumb-title: ''
description: Substance 3D Painterの起動時にクラッシュおよびフリーズし、アプリケーションを安定して起動する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Crash or freeze during startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 起動時にクラッシュまたはフリーズする
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---


# 起動時にクラッシュまたはフリーズする

このページには、アプリケーションが正しく起動しない場合に発生する既知の問題とその解決策が一覧表示されます。

## ソフトウェアの競合

競合を引き起こす可能性のある既知のすべてのソフトウェアの一覧については、次のページを参照してください： [ソフトウェアの競合](software-conflicts.md)。

## 間違ったGPUでの実行

アプリケーションが適切なGPUで起動しない場合、安定性の問題が発生する可能性があります。 詳しくは、このページを参照してください。[Painterが適切なGPUで開始されない](../gpu-issues/painter-doesn-t-start-on-the-right-gpu.md)。

## 古いバージョンのGPUドライバー

古いGPUドライバーを使用すると、フリーズやクラッシュが発生する可能性があります。 可能であれば、最新のGPUドライバーを使用することをお勧めします。 参照： [GPUに古いドライバーがあります](../gpu-issues/gpu-has-outdated-drivers.md)。

## 画面が白くなり、応答しない

Windowsの起動時にアプリケーションがフリーズする（白い画面になる）場合は、いくつかの理由が考えられます。

* 外部アプリケーションが競合を作成しています。どの競合を知るには、[ソフトウェアの競合](software-conflicts.md)を参照してください。
* アプリケーションの一部のウィンドウが別のモニターで開かれています。 インタフェースをデフォルトのレイアウトに戻すと、アプリケーションが正常に起動します。
  1. レジストリエディター（**regedit**、スタートメニューから）を開きます
  1. アプリケーションの環境設定に移動します（[環境設定とアプリケーションデータの場所](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html)を参照）
  1. **Adobe Substance 3D Painter**&#x200B;キーを展開します
  1. **メインウィンドウ2018**&#x200B;キーを選択して削除します
  1. アプリケーションを再起動します

## システムパス/Pythonパスが正しくないためクラッシュする

アプリケーションは、システムパスをチェックしてPythonモジュールと環境設定をロードします。 システムの設定が正しくない場合は、起動時にクラッシュする可能性があります。

Windows:

1. **スタート**&#x200B;メニューを開く
1. **システム（コントロールパネル）**&#x200B;を検索して選択します
1. **[システムの詳細設定]**&#x200B;をクリックします
1. **環境変数**&#x200B;をクリックします
1. **システム変数**&#x200B;で、**PATH**&#x200B;変数を見つけます

次に、変数を編集してその内容を確認できます。 例えば、変数に次のような文字が含まれている場合、クラッシュが発生します

```
ï–›éŒ à €è¸€ì‡ì‡ç¿¹
```


## Windows 10のアップデート

Windows 10の一部のアップデートで不安定になる場合があります。 Windowsに付属の診断ツールを使用して、システムで発生する可能性のあるエラーを検出します。

**展開イメージのサービスと管理** (DISM)と&#x200B;**システムファイルチェッカー** (SFC)ツールを実行することをお勧めします。 DISMは、破損したシステムファイルや欠落しているシステムファイルを修正するために、SFCで必要な置換ファイルを回復するのに役立ちます。

実行中&#x200B;**DISM** :

1. [スタート]メニューを開く
1. コマンドプロンプトを検索
1. 結果を右クリックし、「管理者として実行」を選択します。
1. 次のコマンドを入力してください： **DISM /Online /Cleanup-Image /RestoreHealth**
1. Enterキーを押します

実行中&#x200B;**SFC** :

1. [スタート]メニューを開く
1. コマンドプロンプトを検索
1. 結果を右クリックし、「管理者として実行」を選択します。
1. 次のコマンドを入力します： **sfc /scannow**
1. Enterキーを押します

両方のコマンドを実行した後、コンピューターを再起動してアップデートを適用します。

このテーマの詳細については、[システムファイルチェッカーツールを使用して、見つからないか破損したシステムファイルを修復する](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system)を参照してください。

## 古いバージョンで起動するとクラッシュする

Windowsでは、インストールフォルダーに用意されているdllファイルのいずれかが古すぎるため、バージョン2018(4.x)以前のバージョンが起動しない場合があります。 このクラッシュは、ファイルを手動で新しいバージョンに置き換えることで修正できます。

次の操作を行います。

1. Substance Painterインストールフォルダーに移動します。
1. <b>backup\_libeay32.dll</b>のファイル名<b>libeay32.dll</b>を変更します。
1. 次のファイルをダウンロードします： [updated\_libeay32.zip](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/182266673/225968681/1/1644000679697/updated-libeay32.zip)。
1. zipファイルからdllファイルを展開し、インストールフォルダー（Substance Painter.exeファイルの横）に入れます。
1. アプリケーションを起動します。
