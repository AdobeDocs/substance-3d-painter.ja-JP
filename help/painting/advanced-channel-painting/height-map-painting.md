---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Substance 3D PainterでHeightマップを直接ペイントして、ディスプレイスメントとサーフェスの標高エフェクトを作成する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Height Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Heightマップのペイント
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


# Heightマップのペイント

## 一般的な概念

通常の作業台で作業するのではなく、高い作業台で作業する方が、品質、管理性、柔軟性、アセット間の一貫性の向上など、多くのメリットがあります。

このプロセスは次のようになります。

* 高ポリゴンメッシュからベイクされた法線マップは、低ポリゴンメッシュにロードされます。
* ハイトマップチャンネルに追加のディテールをペイントします。
* ペイントしたHeightはすべてのレイヤを通って合成され、リアルタイムで法線マップに変換され、最終的に高ポリゴンメッシュの法線とブレンドされます。

あなたが心配しなければならないすべては、そのHeightを塗ることであり、残りはすべて自動で行われます。

### Height HDRフォーマット

Heightチャンネルは&#x200B;**HDR**&#x200B;色の形式を使用します。従来のHeightマップでは0 ～ 255の彩度が高くなりますが、この形式を使用すると、輝度の制限に到達することなく正の値と負の値をペイントできます。

* Height上のビットマップまたはサブスタンスでペイントすると、そのソースは元の[0,255]範囲から[-1,1]範囲に再マップされます。

グレーの中間は0に再マップされます。 したがって、127より小さい値はheightmapから&#x200B;**減算**&#x200B;し、127より大きい値はHeightマップ&#x200B;**線形覆い焼き（加算）**&#x200B;のデフォルトの描画モードを使用する場合にheightmapに&#x200B;**加算**&#x200B;します。

* 単色でペイントする場合は、-1 ～ 1の値を直接選択できます。

### Height可視化

単独モードでHeightマップを表示すると、デフォルトのプレビューには正の値のみが表示され、負の値には強い黒の彩度が表示されます。

**+/ – カラー**&#x200B;設定では、正の値と負の値に異なる色を使用して範囲全体を表示できます。

**拡大・縮小**&#x200B;設定では、デフォルトの[-1,1]範囲を超えて追加または削除した場合に、そのHDRマップの表示範囲を変更できます。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/height1.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/height2.png)

</td>
</tr>
</table>
