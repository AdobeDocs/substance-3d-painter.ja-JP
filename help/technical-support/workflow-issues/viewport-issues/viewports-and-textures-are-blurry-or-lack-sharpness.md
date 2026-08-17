---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Substance 3D Painterでぼやけたビューポートとテクスチャを修正して、鮮明でクリアな画質を実現する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ビューポートとテクスチャがぼやけていたり、シャープさに欠ける
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# ビューポートとテクスチャがぼやけていたり、シャープさに欠ける

ビューポートが不鮮明になる理由は異なります。

## 高DPI画面(Retina)設定

デフォルトでは、Substance 3D Painterは高DPI/Retina画面のビューポート解像度を縮小してパフォーマンスを向上させます。

この動作は、**ビューポートの拡大/縮小**&#x200B;パラメーターを変更することで、[メイン設定](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/general-71008262.html)で変更できます。

## テクスチャのフィルタリング

ビューポートでは、ミップマップとテクスチャフィルタリングを使用して、[スパース仮想テクスチャ](../../../features/sparse-virtual-textures.md)をストリーミングしてパフォーマンスを向上させることができます。 これにより、テクスチャがぼやける場合があります。

テクスチャフィルターは、[ビューポート設定](../../../interface/display-settings/viewport-settings.md)パラメーターの下にあるディスプレイ設定ウィンドウで調整できます。
