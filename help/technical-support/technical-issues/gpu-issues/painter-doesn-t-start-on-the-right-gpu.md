---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/technical-issues/gpu-issues/painter-doesn-t-start-on-the-right-gpu.html"
breadcrumb-title: ''
description: Substance 3D Painterが適切なGPUで起動するように設定し、パフォーマンスと互換性を最適化する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Painter doesnt start on the right GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 正しいGPUでPainterが開始しない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---


# Painterが適切なGPUで開始しない

Windowsでは、アプリケーションの起動時に適切なGPUが使用されず、パフォーマンスと安定性の問題が発生する場合があります。 以下に、ソフトウェアが適切なGPUで動作することを確認するための一般的な問題とその解決策のリストを示します。

使用されているGPUを確認するには、[ログファイル](../../exporting-the-log-file.md)を確認してください。

## Windows

### ケーブル構成の監視

Windowsでは、アプリケーションに割り当てられるGPUは、アプリケーションが実行されているモニターによって異なります。 これは、モニターケーブルがGPU自体の出力に直接リンクされているためです。 したがって、アプリケーションが起動するモニターがグラフィックカード自体の出力ではなく、マザーボードのグラフィック出力にリンクされている場合、アプリケーションが間違ったGPUで起動することがあります。 その場合、Windowsは専用GPUではなく、統合GPUを使用する可能性が高くなります。

<b>この問題を解決するには</b> ：マザーボードにリンクされているモニターのプラグインを解除し、代わりにGPU出力にリンクすることで、ケーブル構成を修正します。

### GPUドライバーの誤ったインストール

GPUドライバーが正しくインストールされていない場合、アプリケーションは専用GPUに到達できず、代わりに統合GPUでフォールバックする必要があります。

<b>この問題を解決するには</b> ：現在のGPUドライバーをアンインストールし、クリーンアップを実行してから、コンピューターの再起動後にGPUドライバーを再インストールします。

### Nvidia GPUドライバープロファイル設定

ラップトップなどの一部のコンピューターでは、デフォルトで専用のNvidia GPUではなく、統合GPUでアプリケーションが実行される場合があります。 NVIDIA GPUでは、適切なGPUへの切り替えはアプリケーションプロファイルに依存します。 アプリケーションにこのようなプロファイルがない場合は、手動で割り当てることができます。

<b>この問題を解決するには</b> :

1. デスクトップを右クリックして、NVIDIAコントロールパネル<b>または</b>を選択します。コントロールパネルに移動して、NVIDIAコントロールパネルを検索します。
1. <b>3D設定</b>で、<b>3D設定の管理</b>に移動します
1. 「<b>プログラムの設定</b>」タブで、<b>Substance 3D Painter</b>の新しいプロファイルを追加します
1. 優先するグラフィックプロセッサー設定を「高性能NVIDIAプロセッサー」に変更します。

### Windowsパフォーマンス設定

デフォルトのパフォーマンスと消費電力の設定が原因で、WindowsがアプリケーションのGPU設定を間違った設定にした可能性があります。

<b>この問題を解決するには： </b>以下の手順に従って、既定のGPU構成を上書きしてください。

1. デスクトップを右クリックして表示設定を開きます。

   ![](../../../assets/settings-33.png)
1. ホーム上のウィンドウの下部に移動し、「 Graphics Settings 」をクリックします。

   ![](../../../assets/graphics-settings.png)
1. 「参照」ボタンをクリックして、 Substance 3D Painterの実行可能ファイルを見つけます。

   ![](../../../assets/browse-16.png)
1. アプリケーションが追加されたら、「オプション」ボタンをクリックします。

   ![](../../../assets/options-19.png)
1. 設定「高パフォーマンス」を選択し、「保存」ボタンをクリックします。

   ![](../../../assets/specs.png)

## Linux

### 「デフォルト以外のGPUを優先」を無効にする

デスクトップのショートカットからPainterを使用する場合、またはSteamからを使用する場合は、<b>\*.desktop</b>ファイル内の設定<b>PrefersNonDefaultGPU</b>が<b>false</b>に設定されていることを確認してください。

この設定は誤解を招く可能性があり、より強力で控えめなGPUの代わりに、統合されたGPUが使用/強制される原因になります。 詳細については、[こちらのディスカッション](https://github.com/ValveSoftware/steam-for-linux/issues/9940)を参照してください。

### DRI\_PRIME環境変数を使用して特定のGPUを強制する

デフォルトでは、PainterはVulkan Graphics APIでリストされた最初のGPUを使用しますが、このGPUが間違っている可能性があり（最初にリストされた統合GPUである可能性があります）、パフォーマンスが低下します。 DRI\_PRIME環境変数を使用して、任意のGPUを強制できます。 詳細については、[Arch wikiのドキュメント](https://wiki.archlinux.org/title/PRIME#For_open_source_drivers%E2%80%94PRIME)を参照してください。 [Mesaドキュメント](https://docs.mesa3d.org/envvars.html#envvar-DRI_PRIME)を参照することもできます。
