---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Substance 3D PainterでUV再投影を使用して、異なるUVレイアウト間でテクスチャを転送する方法を説明します。
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

UV再投影は、テクスチャ解像度を変更した場合、または新しいメッシュを読み込んだ場合に実行される自動処理です。\
（[プロジェクト構成](https://substance3d.adobe.com/display/draftpainter/project%20configuration)ウィンドウを介して）ドキュメントに新しいメッシュを読み込むと、すべてのアクションがその新しいメッシュに再投影されます。 トポロジが変更されても（似ている場合）、UVが変更されても問題ありません。 再投影はすべてのレイヤーとブラシストロークを再計算するので、少し時間がかかる場合があります（特に高テクスチャ解像度の場合）。

2Dビューでペイントする

2Dビューで作成されたストロークはすべてUV空間で実行されるため、再読み込み後にメッシュのUVが急激に変化した場合でも、ストロークを正しく再投影する方法はありません。 プロジェクトの再投影を証明する最もよい方法は、3Dビューの代わりに、IDマップやその他の種類の選択やペイントでマスクすることです。

## 再投影はどのように機能しますか？

Substance 3D Painterは、データをワールド空間の3Dに保存して、すべてを非破壊的に保ちます。 つまり、メッシュを再読み込みする場合、Substance 3D Painterは再読み込みの前にメッシュがあった場所をペイントしようとします。そのため、一部のピースが動く可能性があるかどうかは判断できません。

また、Substance 3D Painterはメッシュを読み込むときにも、スペースを登録し、ツール（ペイントブラシ、パーティクルなど）の相対尺度を定義するためのバウンディングボックスを計算します。 このバウンディングボックスは、すべての軸で1ユニット幅です。 新しいメッシュを読み込むときに、「ストロークを保持」をオフにすると、バウンディングボックスが新しいメッシュに再正規化されます。 したがって、メッシュのサイズが大幅に変更されると、ストロークが移動する可能性があります。 ただし、「ストロークを保持」にチェックを入れると、ブラシストロークを正しく投影し直すために、元のバウンディングボックスが新しいバウンディングボックスに拡大・縮小されます。

>[!WARNING]
>
> 3Dメッシュの単位を変更すると、UV再投影が機能しなくなる可能性があります。トポロジは変更されていませんが、古いメッシュと新しいメッシュは大きく異なるスケールとして解釈できます。 修正が困難な場合があるため、ユニットの設定を変更しないことが理想的です。
