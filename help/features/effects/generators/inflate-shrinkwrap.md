---
title: シュリンクラップを膨張
description: Substance 3D Painterの展開シュリンクラップジェネレーターの使用方法について説明します。
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 3%

---


# シュリンクラップを膨張

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_inflate_shrinkwrap.webp" alt=""/><br><strong>インチ：</strong>シュリンクラップ、膨張、ジェネレータ、ランダムシード</td>
    <td style="border: 0;" valign="top"><strong>説明</strong><br>シュリンクラップの膨張ジェネレーターは、メッシュの表面に細い素材が引き伸ばされている効果を模倣したしわを追加します。<br><br>シュリンクラップの膨張ジェネレーターは、白黒のテクスチャを出力します。 これにより、シュリンクラップ効果を作成するマスクを生成するのに便利です。 ただし、塗りつぶしレイヤーに直接配置して、Heightチャンネルと法線チャンネルにしわを加えることもできます。<br><br>画像の入力には、ベイク処理された曲線マップが必要です。 <a href="../../../baking/baking.md">ベーキングの詳細については、こちらを参照してください</a>。</td>
  </tr>
</table>

## 入力

| 名前を入力 | 説明 |
| --- | --- |
| **曲線**&#x200B;グレースケール | ベイク処理された曲率マップを使用します。 |

## パラメーター

<table>
  <tr>
    <th>パラメーター名</th>
    <th>説明</th>
  </tr>
  <tr>
    <td><strong>プリセット</strong></td>
    <td>膨張プリセット、バキュームプリセット、タイトプリセットの間で切り替えます。</td>
  </tr>
  <tr>
    <td><strong>シード</strong></td>
    <td>Dirtテクスチャの作成に使用するシード値を設定します。 <br><ul><li>別のランダムシードに切り替えるには、「ランダム」をクリックします。</li><li>鉛筆をクリックして現在のシード値を表示し、必要に応じて特定の値を入力します。</li></ul></td>
  </tr>
  <tr>
    <td><strong>膨張または縮小</strong></td>
    <td>膨張モードとシュリンクラップモードを切り替えます。</td>
  </tr>
  <tr>
    <td><strong>継ぎ目の強度</strong></td>
    <td>エッジの明瞭度を調整します。</td>
  </tr>
  <tr>
    <td><strong>エッジ幅を上げる</strong></td>
    <td>膨らませたエッジを引き締める度合いを調整します。</td>
  </tr>
  <tr>
    <td><strong>エッジの強さを上げる</strong></td>
    <td>エッジを浮かす効果の強さを調整します。</td>
  </tr>
  <tr>
    <td><strong>しわの密度</strong></td>
    <td>しわの数を調整します。</td>
  </tr>
  <tr>
    <td><strong>しわの張り</strong></td>
    <td>UV境界でしわを引き寄せる度合いを調整します。</td>
  </tr>
  <tr>
    <td><strong>リンクルの範囲</strong></td>
    <td>しわがUV境界からどこまで届くかを調整します。</td>
  </tr>
  <tr>
    <td><strong>リンクルスケール</strong></td>
    <td>しわのサイズを調整します。</td>
  </tr>
</table>

### 技術パラメーター

| パラメーター名 | 説明 |
| --- | --- |
| **Height範囲** | Height範囲を設定します。 |
| **Heightの位置** | Heightを黒(0)または白(1)側に調整します。 |
| **表面のサイズ(cm)** | サーフェスの物理サイズを設定します。 |
| **表面の深度(cm)** | サーフェスの物理的な深度を設定します。 |
