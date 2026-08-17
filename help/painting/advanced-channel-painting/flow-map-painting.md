---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/flow-map-painting.html"
breadcrumb-title: ''
description: Substance 3D Painterでフローマップをペイントし、マテリアルのフロー方向と異方性効果を制御する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Flow Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: フローマップペイント
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# フローマップペイント

専用チャンネルを用意する予定ですが、通常チャンネルとブラシパラメーターを使用すれば、Substance 3D Painterでフローマップをペイントできます。

## ステップ1 ：法線マップを作成する

16 x 16ピクセルの法線マップテクスチャを作成します。 色は128、255、128である必要があり、次の色が設定されます： ![](../../assets/up-dx.png)\
（このカラーは、DirectXでベクトルが見上げるのと同じです）。

## ステップ2 ：通常チャンネルを追加する

Substance 3D Painterプロジェクトで、**テクスチャセット設定**&#x200B;を使用して&#x200B;**通常**&#x200B;チャンネルを追加します（このチャンネルが存在しない場合）。

## ステップ3 :ブラシを設定する

ブラシパラメーターでパス追跡機能を有効にします。 法線マップテクスチャ（手順1）を法線チャンネルスロットにロードします。 他のチャンネルを無効にします。

![](../../assets/brush-settings-1.png){width="300px"}

## ステップ4 :ペイントします！

パスに従う設定を有効にしてメッシュをペイントすると、ブラシストロークは法線マップに方向を描画します。

![](../../assets/painting-1.png){width="700px"}
