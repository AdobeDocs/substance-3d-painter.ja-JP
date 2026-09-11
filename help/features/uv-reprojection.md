---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Substance 3D PainterでUVの再投影を使用して、異なるUVレイアウト間でテクスチャを転送する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > UV Reprojection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV再投影
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# UV再投影

UV再投影は、メッシュの解像度を変更した場合、または新しいテクスチャを読み込んだ場合に実行される自動プロセスです。\
（[プロジェクト構成](https://substance3d.adobe.com/display/draftpainter/project%20configuration)ウィンドウを介して）文書に新しいメッシュを読み込むと、すべての操作がその新しいメッシュに再投影されます。 トポロジが変更されても（似ている場合）、UVが変更されても問題ありません。 再投影はすべてのレイヤーとブラシストロークを再計算するので、少し時間がかかる場合があります（特に高テクスチャ度の解像度の場合）。

2D ビューのペイント

2D ビューに加えられたストロークはすべてUV空間で実行されるため、再読み込み後にメッシュのUVが大幅に変化した場合に正しく再投影することはできません。 プロジェクトの再投影を証明する最も良い方法は、3D ビューの代わりにID マップやその他の種類の選択範囲およびペイントによるマスクを使用することです。

## 再投影はどのように行われますか？

Substance 3D Painterは、データをワールド空間して3Dに保存し、すべてを非破壊的な状態に保ちます。 つまり、メッシュを再読み込みする際、Substance 3D Painterは再読み込み前のメッシュの場所をペイントしようとします。そのため、一部の要素の移動先を把握する手段がありません。

Substance 3D Painterでは、メッシュを読み込むときにも、バウンディングボックスを計算してスペースを登録し、ツール（ペイントブラシ、パーティクルなど）の相対尺度を定義します。 このバウンディングボックスは、すべての軸で1ユニット幅です。 新しいメッシュを読み込むとき、「ストロークを保持」をオフにすると、バウンディングボックスが新しいメッシュに再正規化されます。 そのため、メッシュのサイズが大きく変化すると、ストロークが動く可能性があります。 ただし、「ストロークを保持」にチェックを入れると、ブラシストロークを正しく投影し直すために、元のバウンディングボックスが新しいバウンディングボックスに拡大・縮小されます。

>[!WARNING]
>
> 3D メッシュの単位を変更すると、UVの再投影が機能しなくなる可能性があります。トポロジは変更されていなくても、新旧のメッシュは大きく異なるスケールと解釈できます。 修正が困難な場合があるため、ユニットの設定を変更しないことが理想的です。
