---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/content/importing-assets/adding-content-on-the-hard-drive.html"
breadcrumb-title: ''
description: ハードディスクからSubstance 3D Painterにコンテンツを追加し、ローカルファイルでリソースライブラリを拡張する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Content > Importing assets > Adding content on the hard drive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ハードドライブへのコンテンツの追加
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 2%

---


# ハードドライブへのコンテンツの追加

新しいコンテンツを直接ハードドライブの適切な場所に配置することで、ライブラリにリソースを追加できます。

ユーザーアセットのデフォルトフォルダーがデフォルトで用意されており、アプリケーションインターフェイスを使用するか、次の場所に手動でドロップして、新しいコンテンツを追加できます。 このデフォルトのライブラリは、ブラシ、ツール、スマートマテリアルなどの新しいプリセットを作成するときにも使用されます。詳細については、[プリセット](../../painting/presets/presets.md)のドキュメントを参照してください。

## アセットの配置場所

以下は、デフォルトの&#x200B;**アセット**&#x200B;ライブラリの場所です。このライブラリには、デフォルトで独自のカスタムコンテンツが作成されます。

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Platform</th><th>バージョン</th><th>パス</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong>以降</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">レガシー</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">レガシー</td><td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong>以降</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>レガシー</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!WARNING]
>
> アプリケーションに同梱されている&#x200B;**スターターアセット**&#x200B;はインストールフォルダー内にあり、新しいバージョンごとに置き換えられます。 この場所に個人コンテンツを置くことはお勧めしません。更新するたびに&#x200B;**削除**&#x200B;され、読み取り/書き込み権限の問題が発生する可能性があるためです。\
> **アセット**&#x200B;の場所または別のカスタムの場所を使用することをお勧めします。 カスタムライブラリの場所を追加する方法の詳細については、[新しいライブラリを追加する](../../interface/assets/adding-a-new-library.md)を参照してください。

## ファイル形式と使用方法

Substance 3D Painterライブラリには、様々な種類のファイルを読み込むことができます。 指定したフォルダー（*alphas*、*colorluts*、*effects*&#x200B;など）に配置 は使用状況のタイプをアセットに割り当てるため、新しいコンテンツを追加する際には適切なフォルダーを選択することが重要です。 カスタムライブラリの場所を追加すると、その場所に適切なフォルダーが自動的に作成されることに注意してください。

| *ファイル形式* | *使用方法* | *フォルダー* |
| --- | --- | --- |
| **SBSAR** | Substance マテリアル | アセット/マテリアル |
| **SBSAR** | フィルター | アセット/エフェクト |
| **SBSAR** | ジェネレーター | アセット/ジェネレーター |
| **PNG、TGA、JPEGなど** | テクスチャまたはAlpha | アセット/テクスチャ&#x200B;**または**&#x200B;シェルフ/ Alpha |
| **HDR、EXR** | 環境またはカラーLut | アセット/環境&#x200B;**または**&#x200B;シェルフ/ Colorlut |
| **GLSL** | シェーダー | アセット/シェーダ |
| **SPPR** | ブラシプリセット | アセット/プリセット/ブラシ |
| **SPPR** | パーティクルプリセット | アセット/プリセット/パーティクル |
| **SPPR** | マテリアルプリセット | アセット/プリセット/マテリアル&#x200B;**または**&#x200B;アセット/マテリアル |
| **SPPR** | ツールプリセット | アセット/プリセット/ツール |
| **SPSM** | スマートマテリアル | アセット/スマートマテリアル |
| **SPMSK** | スマートマスク | アセット/スマートマスク |
| **SPEXP** | プリセットを書き出し | Shelf / Export-presets |

>[!NOTE]
>
> バージョン7.2.0では、カスタムフォルダーおよびカテゴリをライブラリで使用できます。 これらのアイテムには、[パスでフィルター](../../interface/assets/filter-by-path.md)するか、[パンくず](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/navigating-in-the-shelf-147095659.html)を使用して「アセット」ウィンドウからアクセスできます。

>[!WARNING]
>
> **SBS** （SBSARではない）ファイルは直接使用できません。Substance 3D DesignerからSBSARとしてエクスポートする必要があります。
