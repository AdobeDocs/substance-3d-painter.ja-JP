---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-rendering-states-params-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterの「すべてのレンダリング状態パラメーター」シェーダー APIリファレンスにアクセスし、レンダリング状態パラメーターを制御します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Rendering States Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: すべてのレンダリング状態パラメータ – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%

---


# すべてのレンダリング状態パラメータ – シェーダー API

## レンダリング状態の例

## バックフェースカリング

背面を非表示：

```
//: state cull_face on
```


前面と背面を描画します。

```
//: state cull_face off
```


## 合成

完全に不透明なブレンドなしオブジェクト：

```
//: state blend none
```


背面から前面への描画順序の標準の描画モード：

```
//: state blend over
```


背面から前面への描画順序の標準の描画モード。 カラーにアルファが事前に掛けられているものとします。

```
//: state blend over_premult
```


追加描画モード：

```
//: state blend add
```


乗法描画モード：

```
//: state blend multiply
```


## シェーダサンプリングローカリティ

初期設定では、ドキュメントのチャンネルは変形されていないテクスチャ座標を使用してサンプリングされ、ペイント中のレンダリングが最適化されます。

ページ装飾が表示される場合は、*非ローカル*&#x200B;状態を&#x200B;*on*&#x200B;に設定します。

```
//: state nonlocal on 

 
```
