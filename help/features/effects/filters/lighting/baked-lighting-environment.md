---
title: ベイク済み照明環境
description: Substance 3D Painterのベイク済み照明環境フィルターの使用方法について説明します。
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 2%
---

# ベイク済み照明環境

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![ベイク済み照明環境アイコン](./Resources/icon_baked_lighting_environment.png "ベイク済み照明環境")

<b>イン：</b>効果/照明、烘焙、環境、PBR

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 説明

ベイク済み照明環境フィルターは、マテリアルおよび環境光の情報をカラーチャンネルにベイクします。

パススルーモードに設定されたペイントレイヤーで使用され、すべてのチャンネルに適用されます。 正確なシミュレートされた照明が不要な場合や、リソースが限られている場合（モバイルプロジェクトやカラーマップのみに依存するアセットなど）、定型化されたワークフローで役立ちます。

</td>
</tr>
</table>

## 入力

| 名前を入力 | 説明 |
| --- | --- |
| <b>Ambient occlusion:</b>グレースケール | Ambient occlusionマップを使用します。 |
| <b>環境マップ:</b>グレースケール | 環境マップを使用します。 |
| <b>標準：</b>色 | 法線マップを使用します。 |

<a name="parameters"></a>

## パラメーター

| パラメーター名 | 説明 |
| --- | --- |
| <b>水平方向の回転：</b> | 環境光の水平方向の回転を調整します。 |
| <b>垂直方向の回転：</b> | 環境光の垂直方向の回転を調整します。 |
| <b>露光量：</b> | ベイク結果の露光量を調整します。 |
| <b>Heightの強さ：</b> | Height情報が結果に与える影響の強さを調整します。 |
| <b>Ambient occlusionの強さ：</b> | 烘焙のambient occlusionの強さを調整します。 |
| <b>オクルージョンの適用度：</b> | 烘焙内のSpecularオクルージョンの強さを調整します。 |
