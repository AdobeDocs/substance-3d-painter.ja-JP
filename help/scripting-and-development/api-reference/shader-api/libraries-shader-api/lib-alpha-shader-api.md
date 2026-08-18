---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-alpha-shader-api.html"
breadcrumb-title: ''
description: カスタムシェーダのアルファチャンネルと透明度を操作するには、Substance 3D PainterのLibAlphaシェーダー APIリファレンスにアクセスします。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Alpha - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ライブラリAlpha- シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '72'
ht-degree: 0%

---


# ライブラリAlpha- シェーダー API

## lib-alpha.glsl

**パブリック関数：** *alphaKill*

```
import lib-sampler.glsl 

import lib-random.glsl
```


エンジンによって提供される不透明度マップ。

```
//: param auto channel_opacity 

uniform SamplerSparse opacity_tex;
```


Alphaテスト閾値。

```
//: param custom { 

//:   "default": 0.33, 

//:   "label": "Alpha threshold", 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float alpha_threshold;
```


Alphaテストディザリング。

```
//: param custom { 

//:   "default": false, 

//:   "label": "Alpha dithering", 

//:   "group": "Common Parameters" 

//: } 

uniform bool alpha_dither;
```


アルファテストをエミュレート：不透明度がユーザー定義のしきい値未満の場合、現在のフラグメントを破棄します。 テクスチャサンプリング呼び出しの後に呼び出す必要があります：派生物を壊すことができます

```
void alphaKill(float alpha) 

{ 

  float threshold = alpha_dither ? getBlueNoiseThresholdTemporal() : alpha_threshold; 

  if (alpha < threshold) discard; 

} 

 

void alphaKill(SparseCoord coord) 

{ 

  alphaKill(getOpacity(opacity_tex, coord)); 

} 

 
```
