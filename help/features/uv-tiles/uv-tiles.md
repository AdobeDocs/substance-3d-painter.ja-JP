---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/uv-tiles.html"
breadcrumb-title: ''
description: Substance 3D PainterでUVタイルを使用して、タイル状UVレイアウトと複数のテクスチャセットを操作する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > UV Tiles
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV タイル
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 2%

---


# UV タイル

![](../../assets/banner-uvtiles.jpg)

UVタイルは、複数のUV範囲にわたる複数のテクスチャセットをテクスチャセット内にテクスチャする方法です。

デフォルトでは、従来のワークフローでは、テクスチャが各UV範囲に対して繰り返されます。 UVタイルを使用すると、各範囲が代わりに専用のテクスチャになります。 このワークフローを使用すると、UVを複数のテクスチャセットに分割して、一般的なテクスチャ解像度を仮想的に上げることができます。 UVタイルは現在、UDIM命名規則のみをサポートしています。

UVタイルのワークフローの詳細については、次のページを参照してください。

* UVタイルワークフローを使用した[プロジェクトの作成](../../getting-started/project-creation.md)
* [2Dビュー](../../interface/viewport/2d-view.md)でUVタイルを表示しています。
* [UVタイルマスク](../../interface/layer-stack/geometry-mask.md)を使用してパフォーマンスを向上させます。
* [画像シーケンス](image-sequence.md)を読み込んで使用しています。
* [テクスチャセット設定](../../interface/texture-set/texture-set-settings.md)でUVタイルごとの解像度を調整しています。

>[!NOTE]
>
> UVタイルプロジェクトの操作は負荷が高くなる可能性があるため、読み込み時間と一般的なパフォーマンスを向上させるためにSSDを使用することをお勧めします。 また、SSD上でキャッシュの場所を設定することをお勧めします。
