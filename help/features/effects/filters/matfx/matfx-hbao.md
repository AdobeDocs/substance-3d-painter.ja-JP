---
title: MatFX HBAO
description: Substance 3D PainterのMatFX HBAOフィルターの使用方法について説明します。
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%
---

# MatFX HBAO

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![MatFX HBAOアイコン](./Resources/icon_matfx_hbao.png "MatFX HBAO")

<b>イン：</b>効果/ambient occlusion、Height、シェーディング

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 説明

MatFX HBAOフィルタは、Height情報から地平線ベースのambient occlusionを生成します。

テクスチャレイヤーまたはマスクで、ソースチャンネルまたはHeightに基づいて深度シャドウや接触シャドウを加えるために使用されます。

</td>
</tr>
</table>

<a name="parameters"></a>

## パラメーター

| パラメーター名 | 説明 |
| --- | --- |
| <b>ぼかしの強さ：</b> | 結果のぼかしの強さを調整します。 |
| <b>ぼかしの回り込み：</b> | ぼかしのラップを切り替えます。 有効にすると、テクスチャの反対側からピクセルがサンプリングされます。 |
| <b>チャネルソース：</b> | オクルージョンの作成に使用するチャンネルソースを選択します。 |
| <b>ワールド単位を使用：</b> | ワールドスペース単位の使用を切り替えます。 |
| <b>深度:</b> | Height入力の知覚深度を調整します。 |
| <b>半径：</b> | オクルージョン効果のサンプリング半径を調整します。 |
| <b>強度：</b> | オクルージョンの強さを調整します。 |
| <b>リリーフ残高：</b> | リリーフ貢献度のバランスを調整します。 |
