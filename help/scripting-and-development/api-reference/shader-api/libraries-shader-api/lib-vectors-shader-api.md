---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-vectors-shader-api.html"
breadcrumb-title: ''
description: Substance 3D PainterのLib Vector シェーダー APIリファレンスにアクセスして、カスタムシェーダのベクトル操作を操作します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Vectors - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ライブラリのベクター – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---


# ライブラリのベクター – シェーダー API

## lib-vectors.glsl

**パブリック関数：** *computeLocalFrame* *getEyeVec* *tangentSpaceToWorldSpace* *worldSpaceToTangentSpace*

ライブラリからインポート

```
import lib-normal.glsl
```


どのビューがシェーディングされるか。

```
//: param auto is_2d_view 

uniform bool is2DView;
```


どのような投影が使われているのか。

```
//: param auto is_perspective_projection 

uniform bool is_perspective;
```


ワールド空間での目の位置。

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


ワールド空間のカメラ方向。

```
//: param auto world_camera_direction 

uniform vec3 camera_dir; 

 

//: param auto facing 

uniform int facing; 

 

bool isBackFace() { 

  return facing == -1 || (facing == 0 && !gl_FrontFacing); 

}
```


ワールド空間の目のベクトルを計算

```
vec3 getEyeVec(vec3 position) { 

  return is_perspective ? 

    normalize(camera_pos - position) : 

    -camera_dir; 

}
```


正接空間からワールド空間へのベクターの変換

```
vec3 tangentSpaceToWorldSpace(vec3 vecTS, V2F inputs) { 

  return normalize( 

    vecTS.x * inputs.tangent + 

    vecTS.y * inputs.bitangent + 

    vecTS.z * inputs.normal); 

}
```


ワールド空間から正接空間へのベクターの変換

```
vec3 worldSpaceToTangentSpace(vec3 vecWS, V2F inputs) { 

  // Assume the transformation is orthogonal 

  return normalize(vecWS * mat3(inputs.tangent, inputs.bitangent, inputs.normal)); 

}
```


ワールド空間における頂点の局所フレーム

```
struct LocalVectors { 

  vec3 vertexNormal; 

  vec3 tangent, bitangent, normal, eye; 

};
```


カスタムのワールド空間法線とanisotropy angleからローカルフレームを計算

```
LocalVectors computeLocalFrame(V2F inputs, vec3 normal, float anisoAngle) { 

  LocalVectors vectors; 

  vectors.vertexNormal = inputs.normal; 

  vectors.normal = normal; 

 

  // Flip the normals for back facing polygons 

  if (isBackFace()) { 

    vectors.vertexNormal = -vectors.vertexNormal; 

    vectors.normal = -vectors.normal; 

  } 

 

  vectors.eye = is2DView ? 

    vectors.normal : // In 2D view, put view vector along the normal 

    getEyeVec(inputs.position); 

 

  // Trick to remove black artifacts 

  // Backface ? place the eye at the opposite - removes black zones 

  if (dot(vectors.eye, vectors.normal) < 0.0) { 

    vectors.eye = reflect(vectors.eye, vectors.normal); 

  } 

 

  // Create a local frame for BRDF work 

  vec3 tangent = normalize( 

    inputs.tangent 

    * vectors.normal * dot(inputs.tangent, vectors.normal) 

  ); 

  vec3 bitangent = normalize( 

    inputs.bitangent 

    * vectors.normal * dot(inputs.bitangent, vectors.normal) 

    * tangent * dot(inputs.bitangent, tangent) 

  ); 

 

  float cosAngle = cos(anisoAngle); 

  float sinAngle = sin(anisoAngle); 

  vectors.tangent = cosAngle * tangent - sinAngle * bitangent; 

  vectors.bitangent = cosAngle * bitangent + sinAngle * tangent; 

 

  return vectors; 

}
```


メッシュと文書のHeightおよび法線からローカルフレームを計算

```
LocalVectors computeLocalFrame(V2F inputs) { 

  // Get world space normal 

  vec3 normal = computeWSNormal(inputs.sparse_coord, inputs.tangent, inputs.bitangent, inputs.normal); 

  return computeLocalFrame(inputs, normal, 0.0); 

} 

 
```
