---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/physical-size.html"
breadcrumb-title: ''
description: Substance 3D Painterで物理サイズを設定し、実際の寸法を定義してテクスチャを正確に拡大・縮小する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Physical size
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 物理サイズ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%

---


# 物理サイズ

![](../assets/banner-physicalsize-2.png)

物理サイズは、Substanceマテリアル内のプロパティで、実際のサイズを定義します。 3Dサーフェス上のマテリアルのサイズと外観を正確に一致させることができます。 Painterでは、デフォルトの内部単位としてセンチメートルが使用されます。

物理サイズを使用するには、このプロパティを0,0,0以外の値に設定したマテリアルを適用し、UV物理サイズ/スケールで塗りつぶしレイヤー（またはエフェクト）の変換モードを有効にします。

詳しくは、以下を参照してください。

* [入力投影](../painting/fill-projections/fill-projections.md)の<b>物理サイズ</b>パラメーター
* [ビューポート設定](../interface/display-settings/viewport-settings.md)の<b>グリッド</b>パラメーター
* <b>[シェーダー設定](../interface/shader-settings/shader-settings.md)の物理サイズ</b>に基づくディスプレイスメント

>[!NOTE]
>
> * Painterバージョン8.3以降では、物理サイズはすべての種類の投影で使用できます。
> * ほとんどのメッシュファイル書式では、メッシュの作成時に使用される単位が指定されています。この単位は、読み込み時に自動的にセンチメートルに変換されます。
> * .objなどの一部の形式には単位情報がないため、.objメッシュを使用してプロジェクトを作成すると、変換されずに既定でセンチメートル単位で測定されます。
