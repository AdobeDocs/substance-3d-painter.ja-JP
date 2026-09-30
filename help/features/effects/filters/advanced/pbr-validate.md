---
title: PBR 検証
description: Substance 3D PainterのPBR 検証フィルターの使用方法について説明します。
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 2%
---

# PBR 検証

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![PBR 検証アイコン](./Resources/icon_pbr_validate.png "PBR 検証")

<b>イン：</b>エフェクト/pbr、メタリック、ラフネス

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 説明

PBR 検証フィルタはアルベド暗値と金属反射率範囲を調べてPBRデータを検証する。

塗りつぶしレイヤー上で使用され、マテリアル値が予想されるPBR範囲内に収まることを確認します。 マテリアルを書き出すときにPBR 検証を有効にしないでください。

</td>
</tr>
</table>

<a name="parameters"></a>

## パラメーター

| パラメーター名 | 説明 |
| --- | --- |
| <b>検証モード：</b> | アルベド、金属反射率、またはその両方を検証するかどうかを選択します。 |
| <b>アルベドの暗い範囲のしきい値：</b> | アルベドの検証に使用できるダーク値の最小しきい値を選択します。 |
| <b>金属の反射率範囲：</b> | メタリックの値の検証に使用する反射率範囲を選択します。 |
| <b>オーバーレイマップ：</b> | マップデータの上の検証オーバーレイを切り替えます。 |

