---
title: Heightを標準に
description: Substance 3D PainterのHeight対通常フィルターの使用方法について説明します。
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%
---

# Heightを標準に

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![通常のアイコンへのHeight](./Resources/icon_height_to_normal.png "通常のHeightへの移動")

<b>内：</b>効果/

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 説明

Heightから法線フィルターは、Heightチャンネルに基づいて正確な法線データを生成します。

Height情報を通常のデータに変換するためにテクスチャレイヤー上で使用されます。

</td>
</tr>
</table>

<a name="parameters"></a>

## パラメーター

| パラメーター名 | 説明 |
| --- | --- |
| <b>既存の法線を上書きする：</b> | 既存の標準データの上書きを切り替えます。 |
| <b>ワールド単位を使用：</b> | 変換に対するワールド単位の使用を切り替えます。 |
| <b>法線の強度：</b> | **ワールド単位の使用**&#x200B;が&#x200B;**偽**&#x200B;の場合、これを使用して生成された標準データの強度を調整します。 |
| <b>表面のサイズ(cm):</b> | **ワールド単位を使用**&#x200B;が&#x200B;**真**&#x200B;の場合、これを使用して、表示されるサーフェスの幅またはHeightのいずれか大きい方を調整します。 |
| <b>深度 (cm):</b> | **ワールド単位を使用**&#x200B;が&#x200B;**真**&#x200B;の場合、これを使用してサーフェスの最大Height範囲を調整します。 |
