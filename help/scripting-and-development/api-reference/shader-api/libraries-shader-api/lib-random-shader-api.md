---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-random-shader-api.html"
breadcrumb-title: ''
description: Substance 3D PainterのLib Random シェーダー APIリファレンスにアクセスして、カスタムシェーダの作成でランダム値を生成します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Random - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ライブラリランダム – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---


# ライブラリランダム – シェーダー API

## lib-random.glsl

**パブリック関数：** *getBlueNoiseThreshold* *getBlueNoiseThresholdTemporal* *fibonacci1D* *fibonacci2D* *fibonacci2DDitheredTemporal*

ライブラリからインポート

```
import lib-defines.glsl
```


スカラー値を含む2Dブルーノイズテクスチャ

```
//: param auto texture_blue_noise 

uniform sampler2D texture_blue_noise;
```


ブルーのノイズテクスチャ解像度

```
const ivec2 texture_blue_noise_size = ivec2(256);
```


現在のフレームのランダムシード

```
//: param auto random_seed 

uniform int alg_random_seed;
```


ピクセル座標に基づいて均一なランダム値を取得します。

```
float getBlueNoiseThreshold() 

{ 

  return texture(texture_blue_noise, gl_FragCoord.xy / vec2(texture_blue_noise_size)).x + 0.5 / 65536.0; 

}
```


ピクセル座標とフレームIDに基づいて、均一なランダム値を取得します。

```
float getBlueNoiseThresholdTemporal() 

{ 

  return fract(getBlueNoiseThreshold() + M_GOLDEN_RATIO * alg_random_seed); 

}
```


フィボナッチシーケンスからi *番目*&#x200B;の番号を返します。

```
float fibonacci1D(int i) 

{ 

  return fract((float(i) + 1.0) * M_GOLDEN_RATIO); 

}
```


フィボナッチシーケンスからi *番目*&#x200B;カップルを返します。 nbSampleは、均一な分布を取得するために必要です。

```
vec2 fibonacci2D(int i, int nbSamples) 

{ 

  return vec2( 

    (float(i)+0.5) / float(nbSamples), 

    fibonacci1D(i) 

  ); 

}
```


フィボナッチシーケンスからi *番目*&#x200B;カップルを返します。 nbSampleは、均一な分布を取得するために必要です。 このバージョンでは、フレーム単位およびピクセル単位の擬似ランダム回転が適用されます。

```
vec2 fibonacci2DDitheredTemporal(int i, int nbSamples) 

{ 

  vec2 s = fibonacci2D(i, nbSamples); 

  s.x += getBlueNoiseThresholdTemporal(); 

  return s; 

} 

 
```
