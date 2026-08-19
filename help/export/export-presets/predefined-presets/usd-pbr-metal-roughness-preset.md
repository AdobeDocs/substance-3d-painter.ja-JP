---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/getting-started/export/export-presets/predefined-presets/usd-pbr-metal-roughness-preset.html"
breadcrumb-title: ''
description: Substance 3D PainterでUSDz(Apple AR)書き出しプリセットを使用して、Apple ARワークフロー用のテクスチャを書き出す方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export presets > Predefined Presets > USDz (Apple AR) Preset
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: USDz (Apple AR)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# USDz(Apple AR)の定義済みテンプレート

>[!NOTE]
>
> カスタム出力テンプレートを使用してUSDに書き出すには、USDz(Apple AR)テンプレートを使用しないでください。 代わりに選択した出力テンプレートを使用し、<b>設定タブ</b>の下部にある<b>USDアセットの書き出し</b>を有効にします。

USDz(Apple AR)の事前定義出力テンプレートは、Apple ARアプリケーションで使用するように設定されたアセットを書き出します。

USDz(Apple AR)テンプレートを使用するには：

1. <b>ファイル/テクスチャを書き出し</b>またはキーボードショートカット<b>Ctrl + Shift + E</b>を使用して、書き出しウィンドウを開きます。
1. <b>「設定」タブ</b>で、<b>「出力テンプレート」ドロップダウン</b>を開き、<b>USDz (Apple AR)</b>を選択します。

![出力テンプレートドロップダウンが開いており、USDz (Apple AR)が選択されている書き出しウィンドウの画像。](../../../assets/export-usd.png){zoomable="yes"}

5つのテクスチャファイル（ベースカラー、メタリック、法線、オクルージョン、粗さ）が作成、保存されます。 非可逆圧縮による斑点を避けるために、通常のマップを除くすべてのファイルがJPGとして保存されます。PNGとして保存されます。

さらに、次の2つのファイルが拡張子usdcとusdzで作成されます。

FinderからMacOSで直接開いたJadeToadの例を次に示します。

![](../../../assets/usdz.png){width="400px"}

以下に、iPhoneに送信されたUSDZファイルの例を示します。このファイルでは、ARモードを使用してJadeToadモデルを実際の環境に配置しています。

![](../../../assets/3d-usdz.jpg){width="500px"}
