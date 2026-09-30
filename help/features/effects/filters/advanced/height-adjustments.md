---
title: Height調整
description: Substance 3D PainterのHeight調整フィルターの使用方法について説明します。
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 1%
---

# Height調整

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Height調整アイコン](./Resources/icon_height_adjust.png "Height調整")

<b>イン:</b>効果/調整、拡大・縮小、オフセット、反転

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 説明

Height調整フィルターは、Heightチャンネルを反転、オフセットまたは選択した値で乗算します。

テクスチャレイヤー上またはマスク内（白黒出力）で、Height情報を非破壊的な方法で調整するために使用します。

</td>
</tr>
</table>

<a name="parameters"></a>

## パラメーター

| パラメーター名 | 説明 |
| --- | --- |
| <b>反転：</b> | 結果の反転を切り替えます。 |
| <b>オフセット：</b> | 指定した量を加算または減算してHeight値を調整します。 |
| <b>乗算：</b> | Height値をこの値で乗算します。 乗算器として、高い領域はより高く、低い領域はより低くなります。 |

>[!NOTE]
>
> **Multiply**&#x200B;および&#x200B;**Offset**&#x200B;パラメータースタックーのうち、オフセットが最初に適用されるパラメーターです。 オフセットの結果、指定されたポイントでHeightの値が0になった場合、乗算は0で乗算されます。つまり、そのポイントでは変化しません。 乗算した値をオフセットするには、2つ目のHeight調整フィルターを追加します。
