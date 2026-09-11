---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/dynamic-material-layering.html"
breadcrumb-title: ''
description: Substance 3D Painterで動的マテリアルレイヤリングツールを使用して、プロシージャルのマスクでマテリアルを合成する方法を説明します。
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

**動的マテリアルレイヤリング**&#x200B;は、1つのテクスチャではなく、シェーダー内で汎用マテリアルが混在している場合に使用される、特殊なワークフローです。 この方法の主な利点は、描画が動的で、シェーダー内の汎用マテリアルを調整することで、ある程度の画質を制御および保持できることです。 マテリアルは一般的ですが、マテリアルをブレンドするために使用されるマスクはメッシュに固有のものなので、繰り返しません。

![](../assets/tilling-mat-layer.gif){width="400px"}

マテリアルレイヤリングワークフローを有効にするには、具体的なシェーダーが必要です。\
Substance 3D Painterにデフォルトで付属しているシェーダー「 **pbr-マテリアルレイヤー** 」では、3つのマスクで4つのマテリアルを合成できます。

## サブレイヤースタック

このシェーダーサブスタックは、シェーダーによって定義および直接サンプリングすることができる。 Substance 3D Painterに付属の「pbr マテリアルレイヤー」シェーダーの例：

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


![](../assets/sub-stacks.png)この例では、シェーダーは指定されたテクスチャセットに3つのサブスタックを作成し、それぞれに「不透明度」チャンネルを含めます。 サブスタックには、 TextureSetリストウィンドウからアクセスできます。

サブテクスチャセットの&#x200B;**チャンネル**&#x200B;はシェーダー&#x200B;**で**&#x200B;定義されているため、レイヤースタック設定で新しいチャンネルを追加することはできません。 チャンネルを追加または削除するには、シェーダーファイルを更新する必要があります。

サポートされる最大チャンネル数は、ハードウェアでサポートされる合計サンプラー数によって定義されます。\
Substance 3D Painterは、パラメーターとして読み込まれるマテリアルに対してバインドレステクスチャ（したがって無制限の量のテクスチャ）をサポートしますが、エンジンによってレイヤースタックに提供されるチャンネルは32（Windowsの場合）に制限されています。 この制限には、プロジェクトのメッシュにベイクされた「通常」や「Ambient occlusion」などの他のテクスチャも含まれます。

## マテリアル入力

マスクに加えてマテリアルを定義するサブスタックも設定できますが、多くの場合、シェーダーにマテリアル入力を定義し、シェルフから直接マテリアルを使用するほうが効率的です。 ほとんどの場合、これらのマテリアルはUnityやUnrealエンジン4などの最終用途にも存在します。 マテリアルをマテリアルする命名規則は、シェーダー「pbr-declaring」に次のように記述されています。

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


![](../assets/materials.png)一部のマテリアル（Substance マテリアルまたはマテリアルプリセット）が読み込まれた場合の結果は次のとおりです。

マテリアルの解像度は「size」パラメーターで定義できます。 デフォルトでは、「default」パラメータを使用してシェーダーを作成する際に、マテリアルをロードすることもできます（ロードする必要があるリソースの名前/ラベルを使用して）。

シェーダー自体のマテリアルとマスクにアクセスするには、「param auto」キーワードを使用してパスとマスクを接続します。

```
//: param auto Material1.channel_basecolor 

uniform sampler2D color1; 

 

//: param auto Mask.channel_opacity 

uniform sampler2D mask;
```


このワークフローでは、マスクとシェーダーパラメーターが最も重要です。 そのため、Substance 3D Painterの書き出しウィンドウでは、「 **シェーダーパラメーターを書き出し**」設定を有効にすることをお勧めします。 これにより、ディスクの横に&#x200B;**JSON**&#x200B;ファイルが作成されます。このファイルには、サブスタックの設定、使用されているマテリアル、シェーダおよびそのパラメーターに関する情報が含まれています。 パラメータの書き出しと読み込み

現時点では、書き出し時の1つのテクスチャへのマスクのパッキングはサポートされていません。 ただし、スクリプト作成機能を使用してSubstanceバッチツールを呼び出し、代わりにSubstanceを使用してパッキングを実行するという簡単な回避策もあります。

![](../assets/export-window-shader.png)

このJSON ファイルを使用して、プロジェクトのレイヤースタックとシェーダを設定できます。\
これにより、共通のパラメータを共有することで、複数のアプリケーション間を簡単に行き来できます。

![](../assets/import-jsons.png)
