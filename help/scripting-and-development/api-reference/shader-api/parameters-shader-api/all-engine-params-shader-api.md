---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-engine-params-shader-api.html"
breadcrumb-title: ''
description: エンジンレベルのシェーダーパラメーターを制御するには、Substance 3D PainterのAll Engine Params シェーダー APIリファレンスにアクセスします。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Engine Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: すべてのエンジンパラメーター – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# すべてのエンジンパラメーター – シェーダー API

## エンジン・パラメータの例

## テクスチャパラメーター

Substance Painterでは、Sparse Virtual Texture(SVT)システムを使用して、ビューポートにテクスチャを表示します。

このシステムの詳細については、[オンラインドキュメント](../../../../features/sparse-virtual-textures.md)を参照してください。

このシステムは、シェーダコードの書き方に影響を与えます。 *SamplerSparse*&#x200B;構造とテクスチャ参照関数（[lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)を参照）を使用して、この関数の使用を簡略化するためのヘルパーを提供しています。

基本的な使用方法：

```
// Defines the SamplerSparse structure 

import lib-sparse.glsl 

 

//: param auto TEXTURE_TAG 

uniform SamplerSparse uniform_tex;   // Texture sampler and its information
```


テクスチャパラメータでは、&#39;or&#39;演算子を使用してフォールバックを定義できます。

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform SamplerSparse uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2
```


ここで、*TEXTURE\_TAG*&#x200B;は、以下で説明するタグの1つです。

### 文書のチャンネルタグ

縫い目の問題を回避するために、これらのテクスチャはすべて&#x200B;**合成**&#x200B;および&#x200B;**拡張**&#x200B;されます。

**テクスチャセットチャンネル**

*channel\_ambientocclusion* *channel\_anisotropyangle* *channel\_anisotropylevel* *channel\_basecolor* *channel\_blendingmask* *channel\_diffuse* *channel\_diffuse* *channel\_emissive* *channel\_glossiness* *channel\_Height* *channel\_ior* *channel\_metallic* *channel\_normal* *channel\_opacity* *channel\_reflection* *channel\_roughness* *channel\_scattering* *channel\_roughness* *channel\_specularlevel* *channel\_transmissive*

**ユーザーチャネル**

*channel\_user0* *channel\_user1* *channel\_user2* *channel\_user3* *channel\_user4* *channel\_user5* *channel\_user6* *channel\_user7*

### メッシュマップ

*texture\_ambientocclusion* ：環境オクルージョンマップ\
*texture\_curvature* ：曲率マップ\
*texture\_id* : IDマップ\
*texture\_normal* ：接線空間の法線マップ\
*texture\_normal\_ws* :ワールド空間の法線マップ\
*texture\_position* :ワールド空間の位置マップ\
*テクスチャ\_Thickness* : Thicknessマップ

## 追加のテクスチャパラメーター

基本的な使用方法：

```
//: param auto TEXTURE_TAG 

uniform sampler2D uniform_tex;   // The texture itself 

 

//: param auto TEXTURE_TAG_size 

uniform vec4 uniform_tex_size;   // The size of the texture (width, height, 1/width, 1/height)
```


テクスチャパラメータでは、&#39;or&#39;演算子を使用してフォールバックを定義できます。

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform sampler2D uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2 

 

//: param auto TEX_TAG_1_size or TEX_TAG_2_size 

uniform vec4 uniform_tex_size; // if TEX_TAG_1 exists then TEX_TAG_1_size else TEX_TAG_2_size
```


ここで、*TEXTURE\_TAG*&#x200B;は、以下で説明するタグの1つです。

*texture\_blue\_noise* :ブルーのノイズテクスチャ\
*texture\_environment* ：環境マップ(**mip-mip-mapped**)は、[lib-env.glsl](../libraries-shader-api/lib-env-shader-api.md)を使用してこのマップを使用します

## その他のパラメーター

*aspect\_ratio* :ビューポート&#x200B;*幅/Height*&#x200B;比を含む&#x200B;*float*

```
//: param auto aspect_ratio 

uniform float uniform_aspect_ratio;
```


*camera\_view\_matrix* :ワールド空間からカメラ空間への変換を表す&#x200B;*mat4*

```
//: param auto camera_view_matrix 

uniform mat4 uniform_camera_view_matrix;
```


*camera\_view\_matrix\_it* : *camera\_view\_matrix*&#x200B;の逆転置バージョン

```
//: param auto camera_view_matrix_it 

uniform mat4 uniform_camera_view_matrix_it;
```


*camera\_vp\_matrix\_inverse* : *プロジェクション\*&#x200B;カメラ\_view\_matrix*マトリックスの逆

```
//: param auto camera_vp_matrix_inverse 

uniform mat4 uniform_camera_vp_matrix_inverse;
```


*environment\_exposure* : envmapの露光量を表す&#x200B;*float*

```
//: param auto environment_exposure 

uniform float uniform_environment_exposure;
```


*environment\_max\_lod* : mip-mapピラミッドのenvmapの深度を表す&#x200B;*float*&#x200B;です

```
//: param auto environment_max_lod 

uniform float uniform_max_lod;
```


*environment\_rotation* : envmapの上軸を中心とした回転を表す&#x200B;*float*\
値は[0,1]の範囲にあり、[0, 2\*pi]の範囲にマップする必要があります。

```
//: param auto environment_rotation 

uniform float uniform_environment_rotation;
```


*向き* :レンダリングされた面を示す&#x200B;*整数*&#x200B;です（–1：背面、0：未定義、1：前面）\
値0は、glsl組み込み変数&#x200B;*gl\_FrontFacing*&#x200B;を安全に使用できることを意味します

```
//: param auto facing 

uniform int uniform_facing;
```


*fovy* : Y軸に沿ったカメラの視野を表す&#x200B;*float*

```
//: param auto fovy 

uniform float uniform_fovy;
```


*is\_2d\_view* : 2Dビューに対してレンダリングが実行されているかどうかを示す&#x200B;*bool*

```
//: param auto is_2d_view 

uniform bool uniform_2d_view;
```


*is\_perspective\_projection* : *bool*&#x200B;は、投影がパースか直交投影かを示します

```
//: param auto is_perspective_projection 

uniform bool uniform_perspective_projection;
```


*main\_light* : *vec4*&#x200B;は、環境の主光源の位置を示します

```
//: param auto main_light 

uniform vec4 uniform_main_light;
```


*mvp\_matrix* :モデルビューの投影行列を表す&#x200B;*mat4*

```
//: param auto mvp_matrix 

uniform mat4 uniform_mvp_matrix;
```


*シーン\_オリジナル\_半径* :シーンの正規化前の境界球の半径を表す&#x200B;*浮動小数点*

```
//: param auto scene_original_radius 

uniform float uniform_scene_original_radius;
```


*screen\_size* ：画面サイズデータ&#x200B;*（幅、Height、1/幅、1/Height）*&#x200B;を含む&#x200B;*vec4*

```
//: param auto screen_size 

uniform vec4 uniform_screen_size;
```


*world\_camera\_direction* :ワールドカメラの向きを表す&#x200B;*vec3*

```
//: param auto world_camera_direction 

uniform vec3 uniform_world_camera_direction;
```


*world\_eye\_position* :ワールドアイの位置を表す&#x200B;*vec3*

```
//: param auto world_eye_position 

uniform vec3 uniform_world_eye_position; 

 
```
