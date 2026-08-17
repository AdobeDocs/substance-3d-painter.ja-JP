---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/uv-tiles/image-sequence.html"
breadcrumb-title: ''
description: Substance 3D PainterでUVタイルを使用した画像シーケンスを使用して、テクスチャアニメーションワークフローを実行する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > UV Tiles > Image Sequence
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 画像シーケンス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 8b892d2d6c9d0f1a3b5d9d3ab9b180a7c2770a83
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# 画像シーケンス

イメージシーケンスは、シェルフ内で1つのリソースとしてグループ化されたイメージのコレクションです。 画像は、ファイル名の特定のパターンに基づいてグループ化されます。

## シーケンスとして画像を読み込む方法

画像ファイルを読み込むときに、ファイル名が特定のパターンに一致する場合は、シーケンスとして自動的に読み込まれます。 読み込んだファイルの横に追加の画像がある場合は、その画像も考慮されます。 したがって、シーケンスからすべてのファイルを手動で読み込む必要はなく、最初のファイルを選択するだけで十分です。

ファイル名の一致例：

次のファイル名では、ファイル名の最後の部分がUDIM番号1032を参照していることを認識できるため、画像シーケンスが正常に読み込まれます。

* file\_22.1032.jpg
* file\_22-223.1032.jpg
* file\_22-223-1032.jpg
* file\_22-223\_1032.jpg

次のファイル名は正しく構造化されていないため、画像シーケンスとして読み込まれません。

* file\_22-2232032.jpg
* file\_22-223PM2032.jpg
* file\_22-223-0032.jpg
* file\_22-223\_Rec2020.jpg

ファイル名の照合は、次の正規表現に基づいて行われます。

```
 ^(.+?)[\.\-\_](?
```


## 画像シーケンスの使用方法

イメージシーケンスは、他のリソースと同様に、インターフェイスの任意のリソーススロットにロードできます。 ただし、場合によっては、正しく使用するために追加の設定が必要になることがあります。

[塗りつぶしレイヤー](../../painting/fill-projections/fill-projections.md) （および塗りつぶし効果）で、投影モードが&#x200B;**塗りつぶし（UVタイルごとに一致）**&#x200B;に設定されていることを確認し、シーケンスの各イメージがテクスチャセットの右[UVタイル](uv-tiles.md)に割り当てられていることを確認します。
