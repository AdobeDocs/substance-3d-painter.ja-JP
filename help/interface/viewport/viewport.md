---
helpx_url: 'https://helpx.adobe.com/jp/substance-3d-painter/interface/viewport.html'
description: Substance 3D Painterのビューポートを使用して、ペイントプロセス中に3Dモデルおよびテクスチャを視覚化する方法を説明します。
helpx_description: Painter > Interface > Viewport
title: ビューポート
source-git-commit: 307c4f1121ae6841d68f8ea5dc597790e0d18a14
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 2%

---


# ビューポート

![](../../assets/viewports-progress.jpg){width="600px"}

ビューポートには、3Dメッシュとそのテクスチャが表示されます。 また、3Dメッシュのサーフェス上でもペイントできます。

## 概要

ビューポートは、4つの部分に分割されます。

* **コンテキストツールバー** ：このツールバーはビューポートの上部にあり、現在のコンテキスト（ペイント時のブラシパラメーターなど）に応じて様々なプロパティへのショートカットを提供します。
* **3Dビュー**：このビューは、カメラによって定義された特定の角度から3Dメッシュを表示します。
* **2Dビュー**：このビューは、現在選択されている[テクスチャセット](../texture-set/texture-set-list.md)の3DメッシュのUVアンラップを表示します。
* **進行状況バー**:ビューポートの下部にある灰色/緑色のバーは、計算が進行中の場合（エンジンがテクスチャを生成している場合など）に表示されます。

詳しくは、専用ページを参照してください。

* [2D ビュー](2d-view.md)
* [3D ビュー](3d-view.md)
* [カメラ管理](camera-management.md)

3Dビューおよび2Dビューは、[表示設定](../../interface/display-settings/display-settings.md)を使用して、追加または異なる情報を表示するように調整できます。

## ビューポートナビゲーションコントロール

ビューポート内を移動するコントロールは、2Dビューでも3Dビューでも同様です。

<table>
  <tr>
    <th>移動タイプ</th>
    <th>ショートカット</th>
    <th>説明</th>
  </tr>
  <tr>
    <td>オービット/回転<br></td>
    <td><strong>Alt +左クリック</strong></td>
    <td><ul><li>3Dビュー：カーソル位置を中心にカメラをオービットします。</li><li>2Dビュー：カーソル位置を中心にUV空間を回転します。</li></ul></td>
  </tr>
  <tr>
    <td>パン</td>
    <td><strong>Alt +中マウスボタンをクリック</strong></td>
    <td>カメラを上、下、左または右に移動します。</td>
  </tr>
  <tr>
    <td>ズーム/ドリー</td>
    <td><strong>Alt +右クリック</strong></td>
    <td>メッシュ/UVの近くまたは遠くにズームします。</td>
  </tr>
</table>

>[!NOTE]
> 2Dビューと3Dビューのいずれでも、**Alt + Shift +左クリック**&#x200B;でオービット/回転するときに、直交角度にスナップできます。

## レイアウトを変更する

既定のレイアウトでは、3Dビューは左側に配置され、2Dビューは右側に配置されます。 レイアウトを変更できる&#x200B;**コンテキストツールバー**&#x200B;からいくつかのパラメーターを使用できます。

<table>
  <tr>
    <th><em>設定</em></th>
    <th><em>説明</em></th>
  </tr>
  <tr>
    <td><strong>ビューポートモード</strong><br><img src="../../assets/viewport-viewmode.png"/></td>
    <td>次の設定は、ビューポートのレイアウトをコントロールします。<br><ul><li><strong>3D/2D</strong> （既定）: 3Dビューと2Dビューの両方をビューポートに表示します</li><li><strong>3Dのみ</strong>: 3Dビューを最大化し、2Dビューを非表示にします。</li><li><strong>2Dのみ</strong>: 2Dビューを最大化し、3Dビューを非表示にします。</li><li><strong>3D/2Dの入れ替え</strong>:ビューが表示される順序を交換します。 3Dビューが左側にある場合、このアクションを選択すると右側に表示されます。</li></ul></td>
  </tr>
  <tr>
    <td><strong>遠近モード</strong><br><img src="../../assets/viewport-camera-projection.png"/></td>
    <td>これらの設定は、3Dビューでの3Dメッシュの表示方法を制御します。<br><ul><li><strong>パースペクティブビュー</strong> （既定値）：人間の目やカメラで見えるとおりに3Dメッシュを表示します。</li><li><strong>直交投影ビュー</strong>：すべての方向が同じ長さを測定するように、3Dメッシュを表示します。</li></ul></td>
  </tr>
  <tr>
    <td><strong>カメラの回転モード</strong><br><img src="../../assets/viewport-camera-axis.png"/></td>
    <td>この設定は、ビューポートカメラが回転できる軸の数を制御します。<br><ul><li><strong>自由回転</strong>:カメラはX、Y、Z軸を中心に回転します。</li><li><strong>制約付き回転</strong> （既定）:カメラはX軸とY軸でのみ回転します（回転なし）。</li></ul></td>
  </tr>
  <tr>
    <td><strong>レンダリングモード</strong><br><img src="../../assets/viewport-rendering.png"/></td>
    <td><a href="../../features/iray-renderer/iray-renderer.md">レンダリングモード</a>に切り替えます。</td>
  </tr>
</table>
