---
breadcrumb-title: ""
description: Substance 3D PainterのライブラリEmissiveシェーダー APIリファレンスにアクセスして、emissiveマテリアルと光彩エフェクトを作成します。
title: ライブラリEmissive - シェーダー API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%
---

# ライブラリEmissive - シェーダー API

## lib-emissive.glsl

**パブリック関数：** *pbrComputeEmissive*

ライブラリからインポート

```
import lib-sparse.glsl
```


emissiveチャンネルのテクスチャ。

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


emissiveの適用度を微調整するために使用する値。

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


見る人の目に映るemissiveの輝きを計算

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
