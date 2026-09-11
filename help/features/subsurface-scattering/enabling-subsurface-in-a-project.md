---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/subsurface-scattering/enabling-subsurface-in-a-project.html"
breadcrumb-title: ''
description: Substance 3D Painterプロジェクトで表面化散乱を有効にして、リアルな半透明のマテリアル効果を作成する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Enabling Subsurface in a Project
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: プロジェクトでサブサーフェスを有効にする
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# プロジェクトでサブサーフェスを有効にする

Substance 3D Painterで表面化散乱を正しくアクティブにするには、いくつかのパラメーターを最初に設定する必要があります。\
このページでは、有効にするパラメーターに関するガイドを提供します。

## 1 - テクスチャセットの設定

[テクスチャセット](../../interface/texture-set/texture-set.md)に、**散布**&#x200B;チャンネルがまだ存在しない場合は追加します。

![](../../assets/add-channel.png)

>[!NOTE]
>
> 散布チャンネルは&#x200B;**サーフェス**&#x200B;の&#x200B;**マスク**&#x200B;のように機能します。チャンネルが黒の場合はサブサーフェスがなく、白の場合はサブサーフェスの強度が最大になります。 このチャンネルはグレースケール値で、 **デフォルトでは黒**&#x200B;です。 レイヤースタックに塗りつぶしレイヤーを追加してデフォルトカラーを制御するか、ペイントレイヤーを使用して手動で強さを制御します。

## 2 – グローバルサブサーフェス設定

[ディスプレイ設定](../../interface/display-settings/display-settings.md) （ポストエフェクト設定の下）で、メインのサブサーフェス分散設定を有効にします。

![](../../assets/enable-subsurface.png)

>[!NOTE]
>
> サブサーフェスエフェクトを有効/無効にすると、プロジェクト全体に影響します。 パフォーマンスの面で重すぎる場合は、このグローバルパラメータを使用すると便利です。

## 3 - シェーダーの設定

![](../../assets/shader-parameters.png)

既定のシェーダーを含む[シェーダー設定](../../interface/shader-settings/shader-settings.md)ウィンドウには、2つの設定を含む「**SSSパラメーター**」グループがあります。\
ターゲットのマテリアルに合わせてスケールとカラーを変更します。 これらの設定の詳細については、[サブサーフェスパラメーター](subsurface-parameters.md)を参照してください。

## ボーナス：シャドウの有効化

表面化散乱効果は問題なく機能しますが、単独で使用すると奇妙に見える場合があります。\
シャドウを有効にすると、ビューポートの最終的な外観を改善し、最終的なマテリアルのリアリズムを高めることができます。

[環境設定](../../interface/display-settings/environment-settings.md)ウィンドウで、「**シャドウ**」設定を有効にします。

![](../../assets/shadow-2.png)
