---
breadcrumb-title: ""
description: Substance 3D Painterの「すべてのレンダリング状態パラメーター」シェーダー APIリファレンスにアクセスし、レンダリング状態パラメーターを制御します。
title: すべてのレンダリング状態パラメータ – シェーダー API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%
---

# すべてのレンダリング状態パラメータ – シェーダー API

## レンダリング状態の例

## バックフェースカリング

折り返し面:

```
//: state cull_face on
```


前後の面を描画します。

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


## シェーダーサンプリング局所性

初期設定では、ペイント中のレンダリングの最適化のために、変形されていないテクスチャ座標を使用してドキュメントチャンネルがサンプリングされます。

ページ装飾が表示される場合は、*非ローカル*&#x200B;状態を&#x200B;*on*&#x200B;に設定します。

```
//: state nonlocal on 

 
```
