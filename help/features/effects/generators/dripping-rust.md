---
title: 滴下錆
description: Substance 3D Painterの滴下錆ジェネレーターの使用方法を説明します。
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 8%

---


# 滴下錆

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dripping_rust.webp" alt=""/><br><strong>イン：</strong>ジェネレーター、グレースケール、色</td>
    <td style="border: 0;" valign="top"><strong>説明</strong><br>滴下する錆発生装置は、錆が流れ下がる筋を作り、重力と水の流出によって生じる腐食をシミュレートします。<br><br>滴る錆ジェネレーターは、白黒のテクスチャを出力します。 そのため、滴る錆効果を生み出すマスクを作成する場合に便利です。<br><br>イメージ入力には、ベイク処理された位置、曲率、および環境オクルージョンが必要です。 <a href="../../../baking/baking.md">ベーキングの詳細については、こちらを参照してください</a>。</td>
  </tr>
</table>

## 入力

| 名前を入力 | 説明 |
| --- | --- |
| **曲線**&#x200B;グレースケール | ベイク処理された曲率マップを使用します。 |
| **環境オクルージョン**&#x200B;グレースケール | ベイク処理されたアンビエントオクルージョンマップを使用します。 |
| **位置**&#x200B;の色 | ベイク処理された位置マップを使用します。 |

## パラメーター

<table>
  <tr>
    <th>パラメーター名</th>
    <th>説明</th>
  </tr>
  <tr>
    <td><strong>シード</strong></td>
    <td>Dirtテクスチャの作成に使用するシード値を設定します。 <br><ul><li>別のランダムシードに切り替えるには、「ランダム」をクリックします。</li><li>鉛筆をクリックして現在のシード値を表示し、必要に応じて特定の値を入力します。</li></ul></td>
  </tr>
  <tr>
    <td><strong>反転</strong></td>
    <td>特定の内部マップ（曲率、AOなど）を反転してから、最終的なマスクに結合します。</td>
  </tr>
  <tr>
    <td><strong>赤褐色の拡散</strong></td>
    <td>滴下錆の広がりを調整します。</td>
  </tr>
  <tr>
    <td><strong>赤褐色のコントラスト</strong></td>
    <td>滴下錆効果のコントラストを調整します。</td>
  </tr>
  <tr>
    <td><strong>拡散の滑らかさ</strong></td>
    <td>滴る錆効果の広がる柔らかさを調整します。</td>
  </tr>
  <tr>
    <td><strong>水滴の強度</strong></td>
    <td>滴下錆効果の長さを調整します。</td>
  </tr>
  <tr>
    <td><strong>水滴の滑らかさ</strong></td>
    <td>滴下錆効果の柔らかさを調整します。</td>
  </tr>
  <tr>
    <td><strong>水滴のサンプル量</strong></td>
    <td>効果の品質を調整します（サンプル数を増やすと品質が向上します）。</td>
  </tr>
  <tr>
    <td><strong>軸を配置</strong></td>
    <td>Y – 緑チャンネル、X – 赤チャンネル、B – 青チャンネルを切り替えて、滴り落ちる錆効果の向きを変えます。</td>
  </tr>
</table>
