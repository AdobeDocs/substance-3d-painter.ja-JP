---
title: ベイク界面
description: ベイクモードインターフェイスとペイントモードの違いについて説明します。
source-git-commit: 987b94e15c1dbe4ddf392ea7878126ecdf989423
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 3%

---


# ベイク処理モード

**ベイク処理モード**&#x200B;では、優れた高品質のベイクを作成するために必要なすべてのツールとパラメーターにアクセスできます。

**ベイク処理モード**&#x200B;にアクセスするには、ビューポートの右上にある(ベイク)クロワッサンボタンをクリックします。 または、[キーボードショートカット&#x200B;](../interface/settings/shortcuts.md)**F8**&#x200B;を使用するか、**モード/メッシュマップをベイク**&#x200B;を選択します

![](../assets/baking/mode_select_buttons.png)

ベイクモードでは、UIレイアウトが変更され、ベイクメッシュマップ専用の様々なパネルが使用できるようになります。

## インターフェイス

ベイク処理モードインターフェイスは、デフォルトで&#x200B;[**ビューポート**](../interface/viewport/viewport.md)&#x200B;とパネルエリアで分割されています。

### ビューポート

[**ビューポート**](../interface/viewport/viewport.md)&#x200B;の動作は、**ペイントモード**&#x200B;の動作と同じです。 同じコントロールを使用して移動し、**[チャンネル]ドロップダウン**&#x200B;を使用して、表示するチャンネルを変更できます。

**ベイク処理モードのビューポート**&#x200B;は、**ペイントモード**&#x200B;とは次の2つの点で異なります。

* ビューポートの左上に、[**ベイク視覚化設定パネル**](baking-visualization-settings.md)&#x200B;があります。
* ビューポートの下部には、現在選択されているメッシュマップを&#x200B;**ベイク**&#x200B;するボタンや、**ペイントモード**&#x200B;に戻るボタンがあります。

### ベイク処理モードパネル

ベイクモード専用のパネルは4つあります。

* [**メッシュマップのベイカー**](../interface/baking-panels/mesh-map-bakers.md): ベイクするメッシュマップを選択します。
* [**共通の設定**](../interface/baking-panels/common-mesh-map-settings.md)：すべてのメッシュマップに共通のベイク設定を調整します。
* [**メッシュマップ設定パネル**](../interface/baking-panels/mesh-map-settings.md) ：選択したメッシュマップのベイク設定を調整します。
* [**ベイクログ**](../interface/baking-panels/baking-log.md):ベイク結果を確認し、問題を診断します。

>[!NOTE]
>
> **共通メッシュマップ**&#x200B;および&#x200B;**メッシュマップ設定パネル**&#x200B;で利用可能なすべてのオプションの一覧については、[**設定**](mesh-map-settings.md)&#x200B;を参照してください。

追加のパネルが利用可能で、**ペイントモード**&#x200B;と同じように動作します。

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../assets/right-bar.png" alt=""/></td>
    <td style="border: 0;" valign="top"><ul><li><a href="../interface/texture-set/texture-set-list.md"><strong>テクスチャセット一覧</strong></a></li><li>右側のバーから利用可能：<ul><li><a href="../interface/miscellaneous/log.md"><strong>ログ</strong></a></li><li><a href="../interface/display-settings/display-settings.md"><strong>表示設定</strong></a></li><li><a href="../interface/history.md"><strong>履歴</strong></a></li></ul></li></ul></td>
  </tr>
</table>