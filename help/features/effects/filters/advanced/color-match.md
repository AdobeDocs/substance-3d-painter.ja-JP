---
title: カラーマッチ
description: Substance 3D Painterでカラーマッチフィルターを使用する方法について説明します。
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%
---

# カラーマッチ

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_color_match.png" alt="カラーマッチアイコン" title="カラーマッチ"/><br><strong>イン:</strong>効果/調整</td>
    <td style="border: 0;" valign="top">説明<br>カラーマッチフィルターは、ソースとターゲットの両方の値を定義する入力スロットをサポートし、定義されたソースの色範囲とターゲットの色範囲を一致させます。 カラーマッチを使用すると、色相、クロマ、ルミナンスの処理方法を制御しながら、サーフェスのカラーを変更しながらディテールを維持できます。<br>カラーマッチは色を微調整するために塗りつぶしレイヤーで使用されます。</td>
  </tr>
</table>

## 入力

| 名前を入力 | 説明 |
| --- | --- |
| **ソースカラー：** | ソースカラーの入力スロット。 カスタムカラーマップまたはアンカーポイントを使用します。 |
| **ターゲットの色：** | ターゲットカラーの入力スロット。 カスタムカラーマップまたはアンカーポイントを使用します。 |

## パラメーター

<table>
  <tr>
    <th>パラメーター名</th>
    <th>説明</th>
  </tr>
  <tr>
    <td><strong>ソースカラーモード:</strong></td>
    <td>ソースカラーのソースを選択します。<br><ul><li><strong>平均</strong>：既存のマテリアル色をソース色として使用します。 注意：これには、レイヤー描画モードを<strong>通過</strong>に設定する必要があります。</li><li><strong>パラメーター</strong>:パラメーターを使用してソースの色を設定します。</li><li><strong>入力</strong>：画像入力を使用してソースカラーを設定します。</li></ul></td>
  </tr>
  <tr>
    <td><strong>ソースカラー：</strong></td>
    <td><strong>ソースカラーモード</strong>が<strong>パラメーター</strong>に設定されている場合、ソースカラーを調整します。</td>
  </tr>
  <tr>
    <td><strong>ターゲットカラーモード：</strong></td>
    <td>ターゲットカラーのソースを選択します。<br><ul><li><strong>パラメーター</strong>:パラメーターを使用してターゲットの色を設定します。</li><li><strong>入力</strong>：画像入力でターゲットの色を設定します。</li></ul></td>
  </tr>
  <tr>
    <td><strong>ターゲットカラー：</strong></td>
    <td><strong>ターゲットカラーモード</strong>が<strong>パラメーター</strong>に設定されているときに、ターゲットカラーを調整します。</td>
  </tr>
  <tr>
    <td><strong>カスタムカラーバリエーション:</strong></td>
    <td>カスタムの色相、クロマ、輝度のバリエーションコントロールを切り替えます。</td>
  </tr>
  <tr>
    <td><strong>色相：</strong></td>
    <td>結果に適用される色相のバリエーションを調整します。</td>
  </tr>
  <tr>
    <td><strong>クロマ：</strong></td>
    <td>結果に適用されるクロマバリエーションを調整します。</td>
  </tr>
  <tr>
    <td><strong>ルミナンス：</strong></td>
    <td>結果に適用される輝度のバリエーションを調整します。</td>
  </tr>
</table>