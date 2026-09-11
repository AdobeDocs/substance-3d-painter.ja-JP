---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/tools-issues/normal-map-looks-incorrect-when-loaded-in-layer-or-tool-properties.html"
breadcrumb-title: ''
description: Substance 3D Painterのレイヤーおよび法線マッププロパティのツール表示に関する問題を修正して、正確なサーフェスのディテールを得る方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Normal map looks incorrect when loaded in layer or tool properties
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: レイヤーまたはツールプロパティに読み込むと、法線マップが正しく表示されない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%

---


# レイヤーまたはツールプロパティに読み込むと、法線マップが正しく表示されない

現在の塗りつぶしレイヤーツールに法線を読み込むと、それがOpenGL 法線マップである場合は、正しく表示されない場合があります。\
理由は非常に単純です。Substance 3D Painterのエンジンは、読み込まれた法線マップがデフォルトでDirectXであると想定しています。

このビヘイビアーは、substance マテリアルまたは専用チャンネルの横にある小さな矢印をクリックすると簡単に編集できます。

![](../../../assets/channel-format-override.png)
