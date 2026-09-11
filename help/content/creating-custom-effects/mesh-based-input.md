---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/content/creating-custom-effects/mesh-based-input.html"
breadcrumb-title: ''
description: Substance 3D Painterのカスタムエフェクトでメッシュに基づく入力を使用して、ジオメトリに応じたテクスチャエフェクトを作成する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Based Input
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュベースの入力
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---


# メッシュベースの入力

メッシュベースの入力は、現在のプロジェクト内のメッシュから抽出されたSubstance 3D Painterのエンジンによって提供されるテクスチャです。 これらのテクスチャを使用すると、メッシュトポロジに基づいた高度なエフェクトを作成できます。

>[!NOTE]
>
> これらのメッシュ情報はトポロジ自体に基づいており、メッシュマップ(ベイクテクスチャ)は考慮されていません。
> 
> エンジンが提供する入力は32ビットの浮動小数点テクスチャで、Substanceグラフの入力の値に縮小/クランプされます。

| メッシュ情報 | 識別子 | 使用状況 | 説明 |
| --- | --- | --- | --- |
| *位置(RGB)* | **メッシュ\_位置** | **meshPosition** | 頂点の位置を含むテクスチャを読み込みます。 |
| *ワールド空間法線 (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | ワールド空間内のnormal頂点を含むテクスチャを取得します。 |
| *正接(RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | ワールド空間の頂点接線を含むテクスチャを取得します。 |
| *ワールド空間のBitangent (RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | ワールド空間の頂点の双接線（双法線）を含むテクスチャを取得します。 |
| *テキストサイズ（グレースケール）* | **メッシュ\_texel\_size** | **meshTexelSize** | テクセルサイズ（ピクセル密度とUVの差）を含むテクスチャを取得します。 |
| *UV マスク （グレースケール）* | **メッシュ\_uv\_mask** | **meshUVMask** | テクスチャをメッシュUV アイランドの黒（外側）マスクおよび白（内側）マスクとして取得します。 |
