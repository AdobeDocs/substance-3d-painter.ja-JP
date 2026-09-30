---
title: しきい値
description: Substance 3D Painterのしきい値フィルターの使用方法について説明します。
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 3%
---

# しきい値

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![しきい値アイコン](./Resources/icon_threshold.png "しきい値")

<b>イン:</b>効果/調整

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 説明

「しきい値」フィルターは、「モード」パラメーターで設定された比較基準が、しきい値と相対的な入力ピクセル値について満たされた場合、白を返します。 これはヒストグラムスキャンと似ていますが、コントラストは常に最大レベルになり、より速く、より正確に同様の結果を得ることができます。

特定のチャンネルからハイコントラストマスクをすばやく作成するには、塗りつぶしレイヤー上またはマスク（白黒出力）上で直接使用します。

</td>
</tr>
</table>

<a name="parameters"></a>

## パラメーター

| パラメーター名 | 説明 |
| --- | --- |
| <b>しきい値：</b> | 入力ピクセル値を比較する輝度値を調整します。 |
| <b>モード：</b> | しきい値に対して使用する比較基準として、「より大きい」、「より大きいか等しい」、「より小さい」、「以下」のいずれかを選択します。 |
| <b>_mode:</b> | 内部モードの値を選択します。 |
| <b>_threshold:</b> | 内部しきい値を調整します。 |
| <b>_threshold_min:</b> | 内部の最小しきい値を調整します。 |
| <b>_threshold_max:</b> | 内部の最大しきい値を調整します。 |
