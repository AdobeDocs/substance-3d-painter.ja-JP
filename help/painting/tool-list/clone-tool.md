---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/painting/tool-list/clone-tool.html"
breadcrumb-title: ''
description: Substance 3D Painterのコピーツールを使用して、テクスチャのディテールをある領域から別の領域にコピーし、シームレスにテクスチャペイントすることができます。
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Clone Tool
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: クローンツール
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%

---


# クローンツール

Substance 3D Painter 2で導入されたクローンツールは、[ペイントツール](https://support.allegorithmic.com/documentation/display/SPDOC/Paint+brush)と同じ種類のパラメーターを共有します。 名前が示すように、コピーツールを使用すると、特定のレイヤーまたは完全なレイヤースタックの内容を、あるポイントから別のポイントに複製できます。

![](../../assets/clone-01.gif)

## 使用状況

コピーツールを使用する最も簡単な方法は、ペイントレイヤーのコンテンツに使用することです。

これは2つの手順で実行できます。

* モデルにマウスを置いて「 **V** 」キーを押し、ソースの場所を選択します。
* 次に、複製した領域が表示される場所にマウスを配置して、ペイントを開始します。

「**V** 」をもう一度押すと、いつでもソースを更新できます。

![](../../assets/2018-06-12-18-11-59.png)

デフォルトでは、クローンツールでペイントする場合、ブラシを放すとソースの場所に従って場所が更新されます。 「**コピーソース動作**」に使用されるボタンを無効にすると、「**V**」を押したときにソースが定義された場所に戻ります。 これは、同じソース領域を使用して複数回ペイントする場合に便利です。

コピーツールをより効率的に使用するには、ペイントレイヤーを作成し、すべてのチャンネルの描画モードを「通過」に設定します。 これにより、「コピーレイヤー」の下にあるすべてのレイヤーから情報を非破壊的な方法で複製できます。 以下のレイヤーはそのままで、後で適用された変更はコピーレイヤーで考慮されます。

![](../../assets/clone-02.gif)
