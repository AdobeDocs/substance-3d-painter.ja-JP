---
breadcrumb-title: ""
description: Substance 3D PainterでUVタイルを使用して、タイル形式のUVレイアウトと複数のテクスチャセットを操作する方法について説明します。
title: UV タイル
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 2%
---

# UV タイル

![](../../assets/banner-uvtiles.jpg)

UV タイルを使用すると、テクスチャセット内の複数のUV範囲にわたる複数のテクスチャセットにテクスチャを付けることができます。

デフォルトでは、従来のワークフローでは、テクスチャは各UV範囲に対して繰り返されます。 UV タイルを使用すると、各範囲は代わりに専用テクスチャになります。 このワークフローでは、UVを複数のテクスチャセットに分割することによって、テクスチャの全般的な解像度を実質的に向上させることができます。 UV タイルでは現在、UDIMの命名規則のみがサポートされています。

UV タイルワークフローについて詳しくは、次のページを参照してください。

* UV タイルワークフローでの[プロジェクトの作成](../../getting-started/project-creation.md)
* [2D ビュー](../../interface/viewport/2d-view.md)のUV タイルを表示しています。
* パフォーマンスを向上させるための[UV タイルマスク](../../interface/layer-stack/geometry-mask.md)。
* [画像シーケンス](image-sequence.md)を読み込んで使用しています。
* [テクスチャセット設定](../../interface/texture-set/texture-set-settings.md)でUV タイルごとの解像度を調整しています。

>[!NOTE]
>
> UV タイルプロジェクトでの作業は負荷が高くなる可能性があるため、SSDを使用して読み込み時間を短縮し、一般的なパフォーマンスを向上することをお勧めします。 また、SSD上でキャッシュの場所を設定することをお勧めします。
