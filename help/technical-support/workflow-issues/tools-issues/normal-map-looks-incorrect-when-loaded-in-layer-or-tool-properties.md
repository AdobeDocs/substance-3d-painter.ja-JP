---
breadcrumb-title: ""
description: Substance 3D Painterのレイヤーおよび法線マッププロパティのツール表示に関する問題を修正して、正確なサーフェスのディテールを得る方法について説明します。
title: レイヤーまたはツールプロパティに読み込むと、法線マップが正しく表示されない
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%
---

# レイヤーまたはツールプロパティに読み込むと、法線マップが正しく表示されない

現在の塗りつぶしレイヤーツールに法線を読み込むと、それがOpenGL 法線マップである場合は、正しく表示されない場合があります。\
理由は非常に単純です。Substance 3D Painterのエンジンは、読み込まれた法線マップがデフォルトでDirectXであると想定しています。

このビヘイビアーは、substance マテリアルまたは専用チャンネルの横にある小さな矢印をクリックすると簡単に編集できます。

![](../../../assets/channel-format-override.png)
