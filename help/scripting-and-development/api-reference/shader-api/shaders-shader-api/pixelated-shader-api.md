---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/pixelated-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterのピクセル化されたシェーダー APIのリファレンスにアクセスして、カスタムのピクセル化されたレンダリングエフェクトを作成します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Pixelated - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ピクセル化 – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---


# ピクセル化 – シェーダー API

## 基本ピクセル化シェーダ

ライブラリから読み込みます。

```
import lib-sampler.glsl
```


ここでは、包括光源の位置を定義します

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


自動パラメーターのワールドアイ位置をユニフォーム&#x200B;**camera\_pos**&#x200B;に&#x200B;**バインド**&#x200B;します。

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


ドキュメントのチャンネル&#x200B;**ベースカラー**&#x200B;を均一な&#x200B;**ベースカラー\_tex**&#x200B;に&#x200B;**バインド**&#x200B;します。

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


このシェーダの新しいカスタムツイークとその既定値を定義します。 このオプションは、影を付けたときにアウトラインのThicknessを微調整するために使用します。

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


このシェーダの新しいカスタムツイークとその既定値を定義します。 これは、点灯したときにアウトラインのThicknessを微調整するために使用します。

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
```


シェーダのエントリポイント。

```
void shade(V2F inputs) 

{
```


いくつかの有用な値を計算する。

```
  vec3 V = normalize(camera_pos - inputs.position); 

  vec3 N = normalize(inputs.normal); 

  vec3 L = normalize(light_pos - inputs.position); 

  float NdV = dot(N, V); 

  float NdL = max(0.0, dot(N, L));
```


**優先度**&#x200B;は、**アウトライン検出**&#x200B;を実行します。 アウトラインの状態に達した場合は、黒で終了します。

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  } 

 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord);
```


ベースカラーの輝度に基づいて、マスクサイズに多少のジッターを加えます

```
  float maskRadiusJitter = pow(dot(baseColor, vec3(0.3333)), 0.1);
```


フラグメントの画面領域の位置に基づいて、マスク値を計算します。 これにより、グリッドのようなパターンが作成されます。

```
  float mask = pow(1.0 - length(fract(gl_FragCoord.xy / 7.0) - vec2(0.5)), maskRadiusJitter * 5.0) * 5.0;
```


ここでは、ベースカラーをサンプリングし、簡単な拡散減衰を適用します

```
  vec3 color = baseColor * NdL; 

 

  diffuseShadingOutput(mask * color); 

} 

 
```
