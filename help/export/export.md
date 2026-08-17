---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export.html"
breadcrumb-title: ''
description: Substance 3D Painterのテクスチャを様々な形式で書き出し、他のアプリケーションやゲームエンジンで使用する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 書き出し
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---


# 書き出し

## テクスチャの書き出し

テクスチャは、ビットマップのコレクションとして書き出されます。 Painterでは、出力テンプレートを使用してテクスチャを柔軟に書き出すことができます。 出力テンプレートを使用すると、書き出すファイルの名前、テクスチャをチャンネルにパックする方法、書き出すファイルのフォーマットとビット深度などを制御できます。 これは難しそうですが、Painterには、一般的に使用される3Dアプリケーションやユースケース用に設定された、数十ものデフォルト出力テンプレートが含まれています。

<b>書き出しウィンドウ</b>を開き、<b>ファイル/テクスチャの書き出し</b>でテクスチャの書き出しを開始するか、キーボードショートカット<b>CTRL + SHIFT + E</b>を使用します。テクスチャの書き出しについて詳しくは、次のリンクを参照してください。

* [書き出しウィンドウ](../export/export-window/export-window.md)
* [出力テンプレート](../export/export-presets/export-presets.md)
* [出力テンプレートの変更または作成](creating-export-presets.md)

### メッシュを書き出す

Painterでは、UVを自動生成するなどの方法で、読み込んだメッシュを修正できます。 Painterでメッシュに変更を加えた場合は、<b>ファイル/メッシュを書き出し</b>でメッシュを書き出すことができます。

メッシュを書き出すときには、いくつかのオプションがあります。

* <b>ディスプレイスメント/テッセレーションなし</b>:マテリアルに基づくジオメトリを修正せずに、ベースメッシュをエクスポートします。
  * <b>三角形化を適用</b>：読み込んだメッシュが四角形またはポリゴンで構成されている場合は、このオプションを有効にして、Painterの三角形化されたメッシュを書き出すことができます。 これは、他のアプリケーションの三角形分割が異なる場合に、視覚的な三角形分割に基づくバグを回避するのに役立ちます。
* <b>ディスプレイスメント/テッセレーションを使用</b>: Painterは、メッシュをテッセレーションしてポリゴンを追加し、ディスプレイスメントまたはHeightを使用してメッシュのサーフェスジオメトリを変化させます。
  * <b>頂点法線の再計算</b>:メッシュのサーフェスを変更すると、既存の頂点の法線が正しくない可能性があります。 このオプションを有効にすると、Painterは頂点法線を新しいサーフェスの正しい値に自動的に更新します。

![](../assets/export-render.jpg){width="500px"}
