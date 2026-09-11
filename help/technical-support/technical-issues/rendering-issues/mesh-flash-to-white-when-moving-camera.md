---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.html"
breadcrumb-title: ''
description: Substance 3D Painter ビューポートでカメラを動かして安定したレンダリングを行うときにメッシュの点滅が白くなる問題を修正する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh flash to white when moving camera
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: カメラを移動するとメッシュフラッシュが白くなる
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# カメラを移動するとメッシュフラッシュが白くなる

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

古いプロジェクトがビューポートのカメラ中を動き回ると、白い/空のテクスチャによって生じる白いフラッシュが一時的に表示される場合があります。 これは、[スパース仮想テクスチャ](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures) (SVT)システムが、古いシェーダーでは使用されないシェーダー構成に依存しているためです。

白いフラッシュを取り除くには、**プロジェクトシェーダー**&#x200B;を&#x200B;**更新**&#x200B;するだけです。

* **既定のシェーダー**&#x200B;の場合： [シェーダーの更新](../../../interface/shader-settings/updating-a-shader.md)ページから順を追って手順を実行します。
* **カスタムシェーダー**&#x200B;の場合：ログおよび[シェーダー API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html)ページのエラーメッセージを確認してください。
