---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-bind-materials-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterのレイヤリングバインド材料シェーダー APIリファレンスにアクセスして、レイヤードワークフローで材料をバインドします。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Bind Materials - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: レイヤバインドマテリアル – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# レイヤバインドマテリアル – シェーダー API

## マテリアルレイヤリング：マテリアルをシェーダパラメータとしてバインドします。

マテリアルは、一意の識別子「id」によって定義されます。 追加のパラメーター：

* &#39;default&#39;：使用される既定の数量単価型リソース名です。
* &#39;size&#39;:マテリアルマップのテクスチャサイズです。
* &#39;group&#39;:マテリアル選択ウィジェットのUIグループです。

例：

```
//:  materials [ 

//:    { 

//:       "id": "Material1", 

//:       "default": "Concrete 044", 

//:       "size": 512, 

//:       "group": "Material 1" 

//:    }, { 

//:       "id": "Material2", 

//:       "default": "Leaves elm", 

//:       "size": 1024, 

//:       "group": "Material 2" 

//:    } 

//:  ]
```


マテリアルからサンプラーにチャンネルをバインドするには、マテリアルのIDの後にチャンネルタグが続く自動パラメーターを定義します（[all-engine-params.glsl](all-engine-params-shader-api.md)で使用可能なチャンネルを参照）。

```
//: param auto Material1.channel_basecolor 

uniform sampler2D basecolor_tex1; 

//: param auto Material1.channel_metallic 

uniform sampler2D metallic_tex1; 

//: param auto Material1.channel_roughness 

uniform sampler2D roughness_tex1; 

 

//: param auto Material2.channel_basecolor 

uniform sampler2D basecolor_tex2; 

//: param auto Material2.channel_metallic 

uniform sampler2D metallic_tex2; 

//: param auto Material2.channel_roughness 

uniform sampler2D roughness_tex2; 

 
```
