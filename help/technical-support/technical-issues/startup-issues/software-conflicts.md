---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/software-conflicts.html"
breadcrumb-title: ''
description: Substance 3D Painterがシステムで正常に起動するのを妨げるソフトウェアの競合を解決する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Software conflicts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ソフトウェアの競合
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# ソフトウェアの競合

Substance 3D Painterがクラッシュしたり、正常に動作しなくなる可能性のある、他のソフトウェアに関する既知の問題の一覧を示します。

| *潜在的な競合の原因* | *問題* |
| --- | --- |
| **ウイルス対策/スパイウェア対策** | ウイルス対策ソフトウェアまたはスパイウェア対策ソフトウェアは、次の問題の原因の1つです。<ul data-preserve-html="true"> <li data-preserve-html="true"><b>誤検出</b>: Painterが誤ってウイルスまたはマルウェアとしてフラグされています。</li> <li data-preserve-html="true"><b>ブロックされているファイル</b>: Painterでファイルの読み取りまたは書き込みができません（書き出し、プリセットの作成など）。</li> <li data-preserve-html="true"><b>ファイルの削除</b>：必要なファイルが削除されたため、Painterを開始できないか、正常に動作しません。</li> </ul>このような場合は、アンチウイルスを一時的に無効にして、ウイルス対策が有効かどうかを確認するか、手動でPainterのウイルス対策ソフトウェアを追加することをお勧めします。 |
| **AMD CrossFireおよびNVIDIA SLI** | Painterでは複数のGPU設定がサポートされていないため、クラッシュする場合があります。 この機能は無効にすることをお勧めします。 |
| <b>オートデスクアシスタント</b> | Autodesk Assistantアプリケーションは、起動時やプロジェクトファイルを開いたときに競合を発生させ、アプリケーションをクラッシュさせる可能性があります。 問題を解決するには、Autodeskアプリケーションを更新します。 |
| <b>台のAlienware/デル製コンピュータ</b> | 詳細については、次のページを参照してください： [ファイルを開くまたは保存するとクラッシュする](../stability-issues/crash-when-opening-or-saving-a-file.md)。 |
| **Paragon SoftwareによるAPFS** | このソフトウェアは、起動時にアプリケーションをクラッシュさせる可能性のあるWindowsパス環境変数の場所を登録する場合があります。 ソフトウェアのアンインストールでは不十分な場合があり、環境変数を手動で削除する必要がある場合があります。 問題のある場所の例： `C:Program Files (x86)Paragon SoftwareAPFS for Windowsï–›éŒ à €è¸€ì‡ì‡ç¿¹` |
| **Avecto** | 古いバージョンのAvectoを実行していると、速度低下やクラッシュが発生する可能性があります。 必ず最新バージョンに更新してください。 |
| **Asus GPUの調整** | このソフトウェアは、Substance 3D Painter内でのシェーダのコンパイル中に問題を引き起こす場合や、シェーダのコンパイルが開始できない場合があります。 この問題が発生した場合は、ソフトウェアをアンインストールして、問題が解決するかどうかを確認することをお勧めします。 |
| **Asus RAMCache** | このソフトウェアは、Substance 3D Painterが正常に起動しないか、実行中に不安定になる場合があります。 安定性に問題がある場合は、Asus RAMCacheを無効にするかインストールすることをお勧めします。 |
| **Asus Sonic Suite** | ASUSマザーボードを搭載したコンピューターでは、<b>Asus Sonic Suite</b>がデフォルトでインストールされる場合があります。 このソフトウェアをアンインストールすると、Substance 3D Painterのディスプレイやインターフェイスの問題が解決される場合があります。 |
| **Cloud Backup Software** **（** OneDrive、**GDrive、** **Dropbox、** **Filestreamなど）** | クラウドバックアップソフトウェアは、プロジェクトの保存中に多数のクラッシュの原因となる可能性があります。 このような場合は、プロジェクトファイルを作業して同期されていないフォルダーに保存し、変更が行われなくなったら、代わりにプロジェクトファイルをクラウドドライブにコピーすることをお勧めします。 |
| **Chitubox** | このソフトウェアは、競合が発生し、プロジェクトを開いたり保存したりといったファイルダイアログを開くと、アプリケーションがクラッシュする可能性があります。 この問題を回避するには、Chitubox環境設定で設定<b>[デスクトップモデルのサムネイルプレビューを有効にする]</b>を無効にします。 |
| **Duetディスプレイ** | <b>Duet Display</b>は、Substance 3D Painterの動作に影響を与える可能性のあるGPUドライバーの問題を引き起こすことが知られています。 アンインストールすることをお勧めします。 |
| **Google Chrome** | Google ChromeとSubstance 3D Painterを同時に実行すると、クラッシュする場合がある。 Substance 3D Painterの安定性を高めるために、Google ChromeおよびGPUドライバーを更新することをお勧めします。 それでもクラッシュが発生する場合は、 Google Chromeでハードウェアアクセラレーションを無効にします（これにより、ChromeはGPUを使用できなくなります）。 |
| **ナヒミックオーディオソフトウェア** | <b>ナヒミック</b>は、Painterをフリーズまたはクラッシュさせる可能性があります。 これを停止すると役に立ちます。また、更新すると問題を回避できます。 Nahimicは、アプリケーションを妨げる可能性があり、停止または無効にする必要があるバックグラウンドサービスも実行します。 |
| **Openshotビデオソフトウェア** | <b>Openshot Video Software</b>は、シェルフのプレビューとの競合を引き起こす可能性があります。 Openshotをアップデートすると、この問題が解決します。 |
| **Pyinstaller** | このアプリケーションは、間違った環境設定を生成し、起動時にエラーを引き起こす可能性があります。 詳細については、「[Qtが原因でアプリケーションを起動できませんでした](application-failed-to-start-because-of-qt.md)」を参照してください。 |
| **Rtr / Plays.tv** | <b>Rptr</b> (または<b>[Plays.tv](http://plays.tv/) </b>)は、一部のGPUドライバーで既定でインストールされています。 このソフトウェアは、不安定な状態になり、アプリケーションがクラッシュする可能性があります。 アプリケーションをアンインストールすることをお勧めします。 |
| **RGBFusion** | このソフトウェアは、グラフィックタブレットドライバーとの競合を引き起こしたり、プロセスを停止すると一時的に問題を修正したり、RGBFusionをアンインストールして永続的な修正を行ったりする可能性があります。 |
