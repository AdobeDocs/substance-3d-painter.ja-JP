---
breadcrumb-title: ""
description: Substance 3D PainterのLibランダムシェーダー APIリファレンスにアクセスして、カスタムシェーダー作成でランダムな値を生成します。
title: ライブラリランダム – シェーダー API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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


スカラー値を含む2D青テクスチャ

```
//: param auto texture_blue_noise 

uniform sampler2D texture_blue_noise;
```


ブルーノイズのテクスチャ解像度

```
const ivec2 texture_blue_noise_size = ivec2(256);
```


現在のフレームランダムシード

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


ピクセル座標とフレーム IDに基づいて、均一なランダム値を取得します。

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


フィボナッチシーケンスからi *番目*&#x200B;カップルを返します。 nbSampleは、均一な分布を取得するために必要です。 このバージョンでは、フレーム単位およびピクセル単位の擬似ランダムな回転が適用されます。

```
vec2 fibonacci2DDitheredTemporal(int i, int nbSamples) 

{ 

  vec2 s = fibonacci2D(i, nbSamples); 

  s.x += getBlueNoiseThresholdTemporal(); 

  return s; 

} 

 
```
