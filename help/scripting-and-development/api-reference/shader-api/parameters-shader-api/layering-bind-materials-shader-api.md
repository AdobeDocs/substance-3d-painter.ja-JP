---
breadcrumb-title: ""
description: Substance 3D Painterのレイヤーのバインドマテリアルシェーダー APIリファレンスにアクセスし、レイヤー化されたワークフローでマテリアルをバインドします。
title: 重ね合わせバインドマテリアル - シェーダー API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%
---

# 重ね合わせバインドマテリアル - シェーダー API

## マテリアルレイヤー：シェーダーパラメーターとしてマテリアルをバインド

マテリアルは、一意の識別子「id」によって定義されます。 追加のパラメーター：

* &#39;default&#39;：使用する既定のマテリアルリソース名です。
* &#39;size&#39;:マテリアルマップのテクスチャサイズ。
* &#39;group&#39;: マテリアルセレクションウィジェットのUIグループです。

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


マテリアルからサンプラーにチャンネルをバインドするには、マテリアルのIDの後にチャンネルタグが続く自動パラメーターを定義します（[すべてのエンジンパラメーター.glsl](all-engine-params-shader-api.md)で使用可能なチャンネルを参照）。

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
