---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/shader-settings/updating-a-shader.html"
breadcrumb-title: ''
description: Substance 3D Painterのカスタムシェーダを更新して、シェーダの変更を適用し、シェーダファイルを再ロードする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings > Updating a shader
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: シェーダを更新する
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---


# シェーダを更新する

問題を修正したり、最新の機能を利用したりするために、プロジェクトで使用するシェーダを更新する必要がある場合があります。 このページでは、これを行う方法について説明します。

以下では、プロジェクトのシェーダを更新する方法を2段階に分けて説明します。

* **シェーダーウィンドウを使用してシェーダーを更新する**
* **Resource Updaterプラグインを使用してシェーダーを更新する**

プロジェクトで&#x200B;**カスタムシェーダ** （デフォルトではSubstance 3D Painterに付属していません）を使用する場合は、[カスタムシェーダ](https://substance3d.adobe.com/display/DRAFTPAINTER/Shader+API)ページを参照して、更新方法に関するガイドを取得してください。

## Shaderウィンドウを使用してシェーダを更新する

### 1 – シェーダ設定ウィンドウを開きます。

**シェーダ設定**&#x200B;ウィンドウは、Dockツールバーのデフォルトでは右側にあります。

![](../../assets/shader-settings-window.png)

### 2 – シェーダボタンをクリックして、更新されたシェーダを選択します。

シェーダボタン（元に戻す/やり直しボタンの下）をクリックして、すでに使用されているものと一致するシェーダを見つけます。

![](../../assets/shader-mini-shelf.png)

### 3 – シェーダが更新されます

新しいシェーダがロードされると、メンション&#x200B;**古い**&#x200B;が削除され、3Dモデルがビューポートに正常に表示されます。

![](../../assets/updated-shader.png)

## Resource Updaterプラグインを使用してシェーダを更新する

### 1 – リソースアップデーターを開く

インターフェイスの左側に移動して、**プラグインツールバー**&#x200B;を見つけ、**リソースアップデーター**&#x200B;アイコンをクリックします。

![](../../assets/resource-icon.png)

### 2 - [シェーダ]タブに切り替える

表示された新しいウィンドウで、「Shader」タブをクリックして、現在のプロジェクトに存在するシェーダを表示します。

![](../../assets/shader-tab.png)

### 3 – シェーダを検索して更新する

Shaderタブに、現在のプロジェクトのすべてのShaderリソースユーザのリストが表示されます。 **古い**&#x200B;シェーダーは、**赤い背景**&#x200B;で表示されています。 リソースの横にある「更新」ボタンをクリックして更新します。

![](../../assets/update-shader-click.gif)
