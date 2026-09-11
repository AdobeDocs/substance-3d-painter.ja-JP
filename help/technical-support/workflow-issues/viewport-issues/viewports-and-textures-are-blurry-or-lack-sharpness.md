---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Substance 3D Painterでぼやけたビューポートやテクスチャを補正して、鮮明でクリアな画質を実現する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ビューポートやテクスチャがぼやけている、または鮮明さに欠けている
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# ビューポートやテクスチャがぼやけている、または鮮明さに欠けている

様々な理由でビューポートがぼやけて見えることがあります。

## 高DPI画面(Retina)設定

デフォルトでは、Substance 3D Painterは高DPI/Retina画面のビューポート解像度を縮小してパフォーマンスを向上させます。

この動作は、**ビューポートの拡大/縮小**&#x200B;パラメーターを変更することで、[メイン設定](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/general-71008262.html)で変更できます。

## テクスチャのフィルタリング

ビューポートはミップマップとテクスチャフィルタリングを使用して、[スパース仮想テクスチャ](../../../features/sparse-virtual-textures.md)のストリーム入出力を行い、処理速度を改善します。 これにより、テクスチャがぼやける場合があります。

フィルタリングは、[ビューポートの設定](../../../interface/display-settings/viewport-settings.md)のパラメーターの下にあるディスプレイの設定ウィンドウで調整できます。
