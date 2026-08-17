---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/workflow-issues/export-issues/texture-dilation-or-padding.html"
breadcrumb-title: ''
description: Substance 3D Painterでテクスチャの膨張とパディングを使用して、書き出されたテクスチャのエッジのアーティファクトを防ぐ方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > Texture dilation or Padding
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: テクスチャの拡大またはパディング
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# テクスチャの拡大またはパディング

**パディング** （**膨張**&#x200B;とも呼ばれる）は、テクスチャの生成後に行われる処理です。 このエフェクトは、UV アイランドの境界線を広げて、空の領域を同じようなピクセルで塗りつぶすことを目的としています。

ゲームエンジンまたはオフラインレンダラーによる[mipmaps](../../../getting-started/glossary.md)の生成後に品質を確保するには、適切なパディングを生成することが重要です。\
Substance 3D Painterは無限のパディングを発生させます。つまり、ピクセルは他のUV アイランドまたはテクスチャの境界線に達するまで引き伸ばされます。

## 無限のパディング生成

無限パディングの仕組みの例を次に示します。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/padding.gif){width="512px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/padding-zoom.gif)

</td>
</tr>
</table>

## MipMaps

3Dコンピューターグラフィックスでは、**ミップマップ**&#x200B;は事前に計算され、最適化されたテクスチャシーケンスです。各テクスチャは、同じ画像の段階的に低い解像度の表現です。 これは、レンダリングの速度を上げ、エイリアシングの斑点を減らすことを目的としています。 カメラに近いオブジェクトには高解像度のミップマップイメージが使用されます。 低解像度の画像は、オブジェクトが遠くに見えるときに使用されます。 これは、元のテクスチャからすべてのピクセルを読み取るか、レンダリングする効率的な方法です。 ミップマップ（各レベル）は、テクスチャ自体の内部に埋め込まれます（ファイル形式でサポートされている場合）。

テクスチャ解像度を下げる際に、メッシュのUVの内側でブリードする不正確なカラーを回避できるため、ミップマップではパディングが非常に重要です。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-padding.gif){width="400px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-nopadding.gif){width="400px"}

</td>
</tr>
</table>

上の例では、グレーの背景はUV（右画像）に裁ち落とされますが、パディングを使用するとカラーがクリーンに保たれます（左画像）。

3Dアプリケーションでは、次のような結果になります。

![](../../../assets/padding-toggle.gif)

## パディングコントロール

Substance 3D Painterでは、パディングの生成を場所に関係なく変更することができます（無効にするなど）。

* **ベイク処理時** ：詳細については、[ベイク処理に関するドキュメント](../../../baking/baking.md)を参照してください。
* **テクスチャセットのテクスチャを生成する** ：詳細については、[テクスチャセットの設定](../../../interface/texture-set/texture-set-settings.md)のドキュメントを参照してください。
* **テクスチャを書き出す場合** ：詳しくは、[書き出し設定](../../../export/export-window/export-window.md)のドキュメントで「パディングの設定」のセクションを参照してください。
