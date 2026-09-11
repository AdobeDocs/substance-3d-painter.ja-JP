---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Substance 3D Painter ビューポートで後ろから表示したときにメッシュ面が消える問題を修正し、メッシュを正しく表示する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 背後から見ると面が消える
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# 背後から見ると面が消える

デフォルトでは、ビューポートのメッシュにメッシュポリゴンの背面（背面）が表示されない場合があります。 これは、現在のシェーダーによって選別されるためです。

面の裏面を表示するには、[シェーダー設定](../../../interface/shader-settings/shader-settings.md)で現在のシェーダーを&#x200B;**pbr-metal-rough-alpha-test**&#x200B;に変更します。
