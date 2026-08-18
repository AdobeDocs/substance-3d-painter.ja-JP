---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/workflow-issues/export-issues/my-exported-opacity-map-is-totally-black.html"
breadcrumb-title: ''
description: 透明を適切に書き出すために、書き出された不透明度マップがSubstance 3D Painterで完全に黒くなる問題を修正する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > My exported opacity map is totally black
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 書き出した不透明度マップが完全に黒くなる
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---


# 書き出した不透明度マップが完全に黒くなる

新しいプロジェクトを作成する場合、デフォルトの色はテクスチャではなくシェーダから取得されます。 したがって、ペイントしなかったすべてのパーツをエクスポートすると、アルファ値が0に設定された黒になります（これらのパーツにはデータが存在しないため）。

これを修正する最も簡単な方法は、レイヤースタックの一番下に塗りつぶしレイヤーを配置することです。これにより、すべてのUVが、シェーダのデフォルトカラーと同じデフォルトカラーで塗りつぶされます。
