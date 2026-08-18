---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/physical-size.html"
breadcrumb-title: ''
description: Substance 3D Painterで物理サイズを設定し、実際の寸法を定義して正確なテクスチャスケーリングを行う方法について説明します。
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

物理サイズは、実際のサイズを定義するSubstanceマテリアル内のプロパティです。 3Dサーフェス上のマテリアルのサイズと外観を正確に一致させるために使用できます。 Painterでは、デフォルトの内部単位としてセンチメートルが使用されます。

物理サイズを使用するには、このプロパティを0,0,0以外の値に設定したマテリアルを適用し、UVトランスフォーム/スケールの下にある塗りつぶしレイヤー（またはエフェクト）の物理サイズモードを有効にします。

詳しくは、以下を参照してください。

* <b>物理サイズ</b>パラメーター（[充填予測](../painting/fill-projections/fill-projections.md)）
* [ビューポート設定](../interface/display-settings/viewport-settings.md)の<b>グリッド</b>のパラメーター
* <b>[シェーダー設定](../interface/shader-settings/shader-settings.md)の物理サイズ</b>に基づくディスプレイスメント

>[!NOTE]
>
> * Painterバージョン8.3以降では、物理サイズはすべての種類のプロジェクションで使用できます。
> * ほとんどのメッシュファイル形式では、メッシュの作成時に使用される単位が指定されています。この単位は、読み込み時に自動的にセンチメートルに変換されます。
> * .objなどの一部の形式には単位情報がないため、 .objメッシュを使用してプロジェクトを作成すると、変換なしでデフォルトでセンチメートル単位で測定されます。
