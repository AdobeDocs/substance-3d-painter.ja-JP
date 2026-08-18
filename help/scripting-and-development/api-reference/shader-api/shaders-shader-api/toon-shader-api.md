---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/toon-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterのトーンシェーダー APIリファレンスにアクセスして、カスタムトゥーン形式のレンダリングエフェクトを作成します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Toon - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: トーン – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# トーン – シェーダー API

## 基本トーンシェーダ

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


**メッシュの曲率**&#x200B;を均一な&#x200B;**曲率\_tex**&#x200B;に&#x200B;**バインド**&#x200B;します。 曲率が使用できない場合は、透明なテクスチャが提供されます。

```
//: param auto texture_curvature 

uniform SamplerSparse curvature_tex;
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


曲率を使用するかどうかに関係なく、

```
//: param custom { 

//:   "default": false, 

//:   "label": "Use curvature" 

//: } 

uniform bool use_curvature;
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


**優先度**&#x200B;は、**アウトライン検出**&#x200B;を実行します。 アウトラインの検出に曲線マップを使用するかどうかをユーザーが選択できるようにします。

```
  if (use_curvature) { 

    float curv = textureSparse(curvature_tex, inputs.sparse_coord).r; 

    NdV = 1.0 - curv; 

  }
```


アウトラインの状態に達した場合は、黒で終了します。

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  }
```


ここでは、4ステップの色の分離を行った。

```
  vec3 color = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  if (NdL > 0.75) { 

    color = color; 

  } else if (NdL > 0.5) { 

    color = color * 0.5; 

  } else if (NdL > 0.1) { 

    color = color * 0.1; 

  } 

  else
```


フォールバックは黒です。

```
    color = vec3(0.0); 

 

  diffuseShadingOutput(color); 

} 

 
```
