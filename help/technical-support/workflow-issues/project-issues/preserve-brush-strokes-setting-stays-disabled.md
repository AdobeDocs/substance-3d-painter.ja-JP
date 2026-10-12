---
breadcrumb-title: ""
description: Substance 3D Painterで「ブラシストロークを保持」設定を無効のままにし、ブラシストロークを適切に保持する方法を説明します。
title: ブラシストローク設定を保持は無効のままです
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%
---

# ブラシストローク設定を保持は無効のままです

Substance 3D Painter 1.5で導入された不運なバグ（1.7で一部修正）のために、一部のプロジェクトではメッシュに関連するメタデータが失われています。 したがって、このバグにより、[プロジェクト構成](../../../interface/project-configuration.md)ウィンドウの「メッシュ時にストロークの位置を保持」設定が無効なままになります。

この問題を解決するには、いくつかの特定の手順に従う必要があります。

* Substance 3D Painter 1.7以降で、問題があるプロジェクトを開きます
* 編集/プロジェクト構成に移動します
* 現在のプロジェクトで（更新されたメッシュではなく）使用していた元のバージョンを選択して再度読み込みます
* Substance 3D Painterでレイヤーを検証して計算します。同じメッシュであれば何も変わりません
* 編集/プロジェクト構成に再度移動します
* 「メッシュ時にストロークの位置を保持」が再度有効になり、新しいメッシュを読み込めるようになりました
