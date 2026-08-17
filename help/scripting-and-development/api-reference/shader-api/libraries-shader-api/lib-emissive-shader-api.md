---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-emissive-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterのライブラリ放射シェーダー APIリファレンスにアクセスして、放射マテリアルと光彩効果を作成します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Emissive - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ライブラリ・エミッシブ：シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# ライブラリ・エミッシブ：シェーダー API

## lib-emissive.glsl

**パブリック関数：** *pbrComputeEmissive*

ライブラリからインポート

```
import lib-sparse.glsl
```


放射チャンネルテクスチャ。

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


放射強度の微調整に使用する値。

```
//: param custom { 

//:   "default": 1.0, 

//:   "label": "Emissive Intensity", 

//:   "min": 0.0, 

//:   "max": 100.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float emissive_intensity;
```


見る人の目に映る放射光を計算

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
