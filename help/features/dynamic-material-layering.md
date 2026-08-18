---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/dynamic-material-layering.html"
breadcrumb-title: ''
description: Substance 3D Painterで動的マテリアルレイヤリングを使用して、マテリアルと手続き型マスクをブレンドして組み合わせる方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Dynamic Material Layering
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 動的マテリアルレイヤリング
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---


# 動的マテリアルレイヤリング

![](../assets/dynamic-material-blending-materials.jpg){width="450px"}

**動的マテリアルレイヤリング**&#x200B;は、一般的なマテリアルを1つのテクスチャではなくシェーダ内で混合する特殊なワークフローです。 このワークフローの主な利点は、ブレンドがダイナミックで、シェーダ内の一般的なマテリアルを傾斜させることで、あるレベルの品質を制御および保持できることです。 マテリアルは一般的ですが、マテリアルをブレンドするために使用されるマスクはメッシュに固有のものなので、繰り返しません。

![](../assets/tilling-mat-layer.gif){width="400px"}

マテリアルレイヤリングワークフローを有効にするには、特定のシェーダが必要です。\
Substance 3D Painterにデフォルトで付属しているシェーダ「 **pbr-material-layering** 」では、3つのマスクで4つのマテリアルをブレンドできます。

## サブレイヤースタック

このシェーダでは、サブスタックを定義し、シェーダで直接サンプリングできます。 Substance 3D Painterに付属のシェーダ「pbr-material-layering」の例：

```
//: stacks [ 

//:   { 

//:     "id": "Mask", 

//:     "channels": [ 

//:   {"id": "opacity"} 

//:  ] 

//:   }, 

[...] 

//: ]
```


![](../assets/sub-stacks.png)この例では、シェーダは指定されたテクスチャセットに3つのサブスタックを作成し、それぞれに「不透明度」チャンネルを作成します。 サブスタックには、 TextureSetリストウィンドウからアクセスできます。

サブレイヤースタックの&#x200B;**チャンネル**&#x200B;はシェーダ&#x200B;**で**&#x200B;定義されているため、テクスチャセット設定に新しいチャンネルを追加することはできません。 チャンネルを追加または削除するには、シェーダファイルを更新する必要があります。

サポートされる最大チャンネル数は、ハードウェアでサポートされる合計サンプラー数によって定義されます。\
Substance 3D Painterでは、パラメーターとして読み込まれるマテリアルに対してバイドレステクスチャ（したがって無制限の量のテクスチャ）をサポートしますが、レイヤースタックに対してエンジンによって提供されるチャンネルは32（Windowsの場合）に制限されます。 この制限には、プロジェクトのメッシュにベイク処理された法線やアンビエントオクルージョンなどの他のテクスチャも含まれます。

## マテリアルの入力

サブスタックを設定してマスクに加えてマテリアルを定義することもできますが、多くの場合、シェーダでマテリアル入力を定義するだけで、シェルフから直接マテリアルを使用するほうが効率的です。 ほとんどの場合、これらのマテリアルはUnityやUnreal Engine 4などの最終用途にも存在します。 マテリアルを宣言する命名規則は、シェーダ「pbr-material-layering」では次のようになります。

```
//: materials [ 

//:   { 

//:      "id": "Material1", 

//:      "label": "Material 1", 

//:      "default": "", 

//:      "size": 1024, 

//:      "default_color": [0.5, 0.5, 0.5] 

//:   }, 

[...] 

//: ]
```


![](../assets/materials.png)一部のマテリアル（Substanceマテリアルまたはマテリアルプリセット）が読み込まれた結果は次のとおりです。

マテリアルの解像度は、「サイズ」パラメータで定義できます。 シェーダが「default」パラメータを使用して作成されている場合、デフォルトでマテリアルをロードすることもできます（ロードする必要があるリソースの名前/ラベルを使用して）。

シェーダ自体のマテリアルとマスクにアクセスするには、「param auto」キーワードを使用してマテリアルとマスクを接続します。

```
//: param auto Material1.channel_basecolor 

uniform sampler2D color1; 

 

//: param auto Mask.channel_opacity 

uniform sampler2D mask;
```


この特定のワークフローで最も重要な部分は、マスクとシェーダパラメータです。 そのため、Substance 3D Painterの書き出しウィンドウでは、「 **シェーダーパラメーターを書き出し**」設定を有効にすることをお勧めします。 これにより、ディスクのテクスチャの横に&#x200B;**JSON**&#x200B;ファイルが作成されます。テクスチャの横には、サブスタックの設定、使用されているマテリアル、シェーダおよびそのパラメータに関する情報が含まれています。 パラメータの書き出しと読み込み

現時点では、1つのテクスチャへのマスクのパッキングは、書き出し中にはサポートされていません。 ただし、スクリプト作成機能を使用してSubstanceバッチツールを呼び出し、代わりにSubstanceを使用してパッキングを実行するという簡単な回避策もあります。

![](../assets/export-window-shader.png)

このJSONファイルは、プロジェクトのレイヤースタックとシェーダの設定に使用できます。\
これにより、共通のパラメータを共有することで、複数のアプリケーション間を簡単に行き来できます。

![](../assets/import-jsons.png)
