---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/project-issues/preserve-brush-strokes-setting-stays-disabled.html"
breadcrumb-title: ''
description: Substance 3D Painterで「ブラシストロークを保持」設定を無効のままにし、ブラシストロークを適切に保持する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Preserve brush strokes setting stays disabled
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ブラシストローク設定を保持は無効のままです
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# ブラシストローク設定を保持は無効のままです

Substance 3D Painter 1.5で導入された不運なバグ（1.7で一部修正）のために、一部のプロジェクトでメッシュに関連するメタデータが失われています。 したがって、このバグにより、[プロジェクト構成](../../../interface/project-configuration.md)ウィンドウの「メッシュ上でストロークの位置を保持」設定が無効なままになります。

この問題を解決するには、いくつかの特定の手順に従う必要があります。

* Substance 3D Painter 1.7以降で、問題があるプロジェクトを開きます
* 編集/プロジェクト構成に移動します
* 現在のプロジェクトで使用したオリジナルメッシュを選択して再インポートします（更新されたバージョンではありません）
* Substance 3D Painterでレイヤーを検証して計算します。同じメッシュであれば何も変わりません
* 編集/プロジェクト構成に再度移動します
* 「メッシュ上のストローク位置を保持」が再度有効になり、新しいメッシュを読み込めるようになりました
