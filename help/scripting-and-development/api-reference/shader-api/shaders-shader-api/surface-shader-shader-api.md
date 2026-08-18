---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/surface-shader-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterのサーフェスシェーダー APIリファレンスにアクセスして、カスタムサーフェスのシェーダーエフェクトとマテリアルを作成します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Surface Shader - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: サーフェスシェーダ – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---


# サーフェスシェーダ – シェーダー API

## surface-shader.glsl

Substance Painterで使用できるシェーダリソースを作成するには、次のプロファイルを持つ&#x200B;*shade*&#x200B;という関数を1つ含むglslファイルを作成します。

```
void shade(V2F inputs);
```


## V2F入力タイプの定義：

```
struct V2F { 

  vec3 normal;               // interpolated normal 

  vec3 tangent;              // interpolated tangent 

  vec3 bitangent;            // interpolated bitangent 

  vec3 position;             // interpolated position 

  vec4 color[1];             // interpolated vertex colors (color0) 

  vec2 tex_coord;            // interpolated texture coordinates (uv0) 

  SparseCoord sparse_coord;  // interpolated sparse texture coordinates used by textureSparse() sampling function 

  vec2 multi_tex_coord[8];   // interpolated texture coordinates (uv0-uv7) 

};
```


注意： uv1-uv7のSparseCoordを取得するには、[lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)で定義された&#x200B;*getSparseCoord(vec2)*&#x200B;を明示的に呼び出す必要があります

## サーフェスシェーダ出力：

フラグメントのプロパティを記述するために、*shade*&#x200B;関数内から次の関数を呼び出すことができます：

```
// fragment opacity. default value: 1.0 

void alphaOutput(float); 

// diffuse lighting contribution. default value: vec3(0.0) 

void diffuseShadingOutput(vec3); 

// specular lighting contribution. default value: vec3(0.0) 

void specularShadingOutput(vec3); 

// color emitted by the fragment. default value: vec3(0.0) 

void emissiveColorOutput(vec3); 

// fragment color. default value: vec3(1.0) 

void albedoOutput(vec3); 

// subsurface scattering properties, see lib-sss.glsl for details. default value: vec4(0.0) 

void sssCoefficientsOutput(vec4);
```


例えば、フラグメントの色を計算するための最も基本的なレンダリング式は、*emissiveColor + アルベド\* diffuseShading + specularShading*です
