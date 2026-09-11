---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/shader-settings/updating-a-shader.html"
breadcrumb-title: ''
description: Substance 3D Painterのカスタムシェーダを更新してシェーダーの変更を適用し、シェーダーファイルを再ロードする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings > Updating a shader
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: シェーダーの更新
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---


# シェーダーの更新

問題を解決したり、最新の機能を利用するには、プロジェクトで使用するシェーダーを更新する必要がある場合があります。 このページでは、これを行う方法について説明します。

以下では、プロジェクトのシェーダーを更新する2つの方法を順を追って説明します。

* **シェーダーウィンドウを使用してシェーダーを更新する**
* **Resource Updaterプラグインを使用してシェーダーを更新する**

プロジェクトで&#x200B;**カスタムシェーダー** （既定ではSubstance 3D Painterに付属していません）を使用する場合は、[カスタムシェーダー](https://substance3d.adobe.com/display/DRAFTPAINTER/Shader+API)ページを参照して、更新方法に関するガイドを取得してください。

## シェーダーウィンドウを使用したシェーダーの更新

### 1 - [シェーダー設定]ウィンドウを開く

**シェーダー設定**&#x200B;ウィンドウは、右側のDockツールバーで既定で利用できます。

![](../../assets/shader-settings-window.png)

### 2 - 「 シェーダー 」ボタンをクリックして、更新されたシェーダーを選択します。

「シェーダー」ボタン（「取り消し」/「やり直し」ボタンの下）をクリックして、既に使用されているシェーダーと一致するデータを見つけます。

![](../../assets/shader-mini-shelf.png)

### 3 – シェーダが更新されます

新しいシェーダーが読み込まれたら、メンション&#x200B;**古い**&#x200B;が削除され、3Dモデルがビューポートで正常に表示されます。

![](../../assets/updated-shader.png)

## Resource Updaterプラグインを使用してシェーダーを更新する

### 1 – リソースアップデーターを開く

インターフェイスの左側に移動して、**プラグインツールバー**&#x200B;を見つけ、**リソースアップデーター**&#x200B;アイコンをクリックします。

![](../../assets/resource-icon.png)

### 2 - 「シェーダー」タブに切り替えます。

表示された新しいウィンドウで、「シェーダー」タブをクリックして、現在のプロジェクトに存在するシェーダーを表示します。

![](../../assets/shader-tab.png)

### 3 - シェーダーを検索して更新する

Shaderタブに、現在のプロジェクトのすべてのShaderリソースユーザのリストが表示されます。 **古い**&#x200B;シェーダーが&#x200B;**赤い背景**&#x200B;で表示されています。 リソースの横にある「更新」ボタンをクリックして更新します。

![](../../assets/update-shader-click.gif)
