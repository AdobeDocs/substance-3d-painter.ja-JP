---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/technical-issues/stability-issues/windows-blue-screens.html"
breadcrumb-title: ''
description: Substance 3D Painterを使用してシステムを安定して動作させる場合に、Windowsのブルースクリーンエラーが発生しないようにする方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Windows Blue Screens
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Windowsブルースクリーン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


# Windowsブルースクリーン

Windows [Blue Screens Of Death (BSOD)](https://en.wikipedia.org/wiki/Blue_screen_of_death)では、通常、ドライバーまたはハードウェアの誤動作に関連しています。 Substance 3D Painter自体は、これらのBSODの責任はありませんが、アプリケーションがどれほど強力であるために、コンピュータ自体の問題に光を当てることができます。 Substance 3D Painterの場合、次の問題が原因でBSODが発生する可能性があります。

## GPUドライバーが不安定

Substance 3D Painterでは、様々な計算を実行するためにGPUに多く依存しています。 GPUドライバーは、不安定になったり、退行したりする場合があります。 最新の修正とパフォーマンスの向上を得るために、GPUを最新に保つことをお勧めします。 参照： [GPUに古いドライバーがあります](../gpu-issues/gpu-has-outdated-drivers.md)。

### Windowsのインストールが不安定

更新を行うと、Windows自体が不安定になる場合があります。 Windowsに付属の診断ツールを使用して、システムで発生する可能性のあるエラーを検出します。

**展開イメージのサービスと管理** (DISM)と&#x200B;**システムファイルチェッカー** (SFC)ツールを実行することをお勧めします。 DISMは、破損したシステムファイルや欠落しているシステムファイルを修正するために、SFCで必要な置換ファイルを回復するのに役立ちます。

実行中&#x200B;**DISM** :

1. **[スタート]メニュー**&#x200B;を開く
1. **コマンドプロンプト**&#x200B;を検索
1. **結果を右クリック**&#x200B;し、「**管理者として実行**」を選択します
1. 次のコマンドを入力してください： **DISM /Online /Cleanup-Image /RestoreHealth**
1. **Enter**&#x200B;を押します

実行中&#x200B;**SFC** :

1. **[スタート]メニュー**&#x200B;を開く
1. **コマンドプロンプト**&#x200B;を検索
1. **結果を右クリック**&#x200B;し、「**管理者として実行**」を選択します
1. 次のコマンドを入力します： **sfc /scannow**
1. **Enter**&#x200B;を押します

両方のコマンドを実行した後、コンピューターを再起動してアップデートを適用します。

この件名の詳細については、「[システムファイルチェッカーツールを使用して、見つからないか破損したシステムファイルを修復する](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system)」を参照してください

### ディスク容量の不足

Substance 3D Painterに[スパース仮想テクスチャ](../../../features/sparse-virtual-textures.md)が導入されて以来、作業中にディスクを使用してテクスチャをキャッシュできるようになりました。 システムの空き容量が不足すると、不安定になる可能性があります。

この問題には、次の2つの簡単な解決策があります。

* ディスクの空き容量を増やして、キャッシュシステムの空き容量を増やします。
* キャッシュディレクトリを、空き容量の多い別のドライブに移動します。 この場所は、アプリケーションのメイン設定に移動することで変更できます。[[一時ファイル]設定](https://docs.substance3d.com/display/SPDOC/General)を参照してください。

### 障害のあるディスク（HDDまたはSSD）

前の点で述べたように、キャッシュシステムはディスクに大きく依存します。 ディスクドライブに障害がある場合、データの書き込みや読み取りを行うときにシステムが不安定になることがあります。

ディスクに障害があるかどうかを検出するには、WindowsでCHKDSKを実行します。

1. **スターメニュー**&#x200B;を開く
1. **コンピューター/このPC**&#x200B;を選択
1. **ハードドライブ上で**&#x200B;を右クリックし、**プロパティ**&#x200B;を選択します。
1. 「**ツール**」タブに切り替えます。
1. 「**エラーチェック**」の「**今すぐ確認/チェック**」をクリックします。

### 障害のあるメモリ

プログラムがメモリの安全な読み取りや書き込みを行うことができない場合、メモリ(RAM)の障害によってシステムの不安定が発生することがあります。 メモリの整合性を確認するために、**MemTest**&#x200B;を実行することをお勧めします。

MemTestのインストールおよび使用方法については、[このガイド](https://www.memtest86.com/technical.htm)を参照してください。
