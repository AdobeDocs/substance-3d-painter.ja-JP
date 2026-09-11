---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-appears-pink-in-the-viewport.html"
breadcrumb-title: ''
description: Substance 3D Painter ビューポートでピンクのメッシュのアピアランスを修正して、マテリアルが適切にレンダリングされるようにする方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh appears pink in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ビューポートではメッシュがピンク色で見える
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---


# ビューポートではメッシュがピンク色で見える

![](../../../assets/pink-mesh.jpg){width="400px"}

**メッシュの作成に使用された**&#x200B;シェーダー&#x200B;**がコンパイルされなくなったため** （**ログウィンドウ**&#x200B;で説明）、ビューポートの内部に&#x200B;**ピンク**&#x200B;と表示される場合があります。 これは、最新バージョンのシェーダー APIをサポートしていない古いシェーダーが原因である可能性があります。

修正方法は次のとおりです。

* **既定のシェーダー**&#x200B;の場合： [シェーダーの更新](../../../interface/shader-settings/updating-a-shader.md)ページから順を追って手順を実行します。
* **カスタムシェーダー**&#x200B;の場合：ログウィンドウと[シェーダー API](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html)ページのエラーメッセージを確認してください。
