---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Substance 3D Painterのビューポートで背面からメッシュ面を表示したときにメッシュ面が消える問題を解決し、メッシュを適切に表示する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 後ろから見るとメッシュの面が消える
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# 後ろから見るとメッシュの面が消える

デフォルトでは、ビューポート内のメッシュは、メッシュポリゴンの背面（背面）を表示しない場合があります。 これは、現在のシェーダによって非表示にされているためです。

面の背面を表示するには、[シェーダ設定](../../../interface/shader-settings/shader-settings.md)で現在のシェーダを&#x200B;**pbr-metal-rough-alpha-test**&#x200B;に変更するだけです。
