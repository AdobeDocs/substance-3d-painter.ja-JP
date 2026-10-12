---
breadcrumb-title: ""
description: Substance 3D Painter ビューポートで後ろから表示したときにメッシュ面が消える問題を修正し、メッシュを正しく表示する方法を説明します。
title: 背後から見ると面が消える
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%
---

# 背後から見ると面が消える

デフォルトでは、ビューポートのメッシュにメッシュポリゴンの背面（背面）が表示されない場合があります。 これは、現在のシェーダーによって選別されるためです。

面の裏面を表示するには、[シェーダー設定](../../../interface/shader-settings/shader-settings.md)で現在のシェーダーを&#x200B;**pbr-metal-rough-alpha-test**&#x200B;に変更します。
