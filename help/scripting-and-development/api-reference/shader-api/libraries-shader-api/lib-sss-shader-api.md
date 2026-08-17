---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-sss-shader-api.html"
breadcrumb-title: ''
description: Substance 3D PainterのLib SSS シェーダー APIリファレンスにアクセスして、カスタムシェーダでサブサーフェススキャッタリングエフェクトを作成します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib SSS - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ライブラリSSS - シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---


# ライブラリSSS - シェーダー API

## lib-sss.glsl

**パブリック関数：** *getSSSCoefficients*

ライブラリからインポート

```
import lib-sampler.glsl
```


スカラーSSS係数テクスチャ

```
//: param auto channel_scattering 

uniform SamplerSparse sss_tex; 

 

//: param auto scene_original_radius 

uniform float sssSceneScale; 

 

//: param custom { 

//:   "label": "Enable", 

//:   "default": true, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Enable the Subsurface Scattering. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform bool sssEnabled;
```


光がマテリアルを通してまっすぐ透過するか（半透明）、散乱を開始する前に拡散するか（肌）を選択します。

```
//: param custom { 

//:   "default": 1, 

//:   "label": "Scattering Type", 

//:   "widget": "combobox", 

//:   "values": { 

//:     "Translucent": 0, 

//:     "Skin": 1 

//:   }, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Skin or Translucent/Generic. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform int sssType;
```


サブサーフェス拡散エフェクトへのグローバルスケール

```
//: param custom { 

//:   "default": 0.5, 

//:   "label": "Scale", 

//:   "min": 0.01, 

//:   "max": 1.0, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Controls the radius/depth of the light absorption in the material. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform float sssScale;
```


材料のSSSの波長依存性

```
//: param custom { 

//:   "default": [0.701, 0.301, 0.305], 

//:   "label": "Color", 

//:   "widget": "color", 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>The color of light when absorbed by the material. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform vec3 sssColor;
```


材料のSSS係数を返す

```
vec4 getSSSCoefficients(float scattering) { 

  if (sssEnabled) { 

    vec3 sss = sssScale / sssSceneScale * scattering * sssColor; 

    return vec4(sss, sss == vec3(0.0) ? 0.0 : 1.0); 

  } 

  return vec4(0.0); 

} 

vec4 getSSSCoefficients(SparseCoord coord) { 

  if (sssEnabled) { 

    return getSSSCoefficients(getScattering(sss_tex, coord)); 

  } 

  return vec4(0.0); 

} 

 
```
