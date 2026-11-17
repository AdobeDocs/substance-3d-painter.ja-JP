---
breadcrumb-title: ""
description: Substance 3D Painterのカスタムエフェクトでメッシュに基づく入力を使用して、ジオメトリに応じたテクスチャエフェクトを作成する方法について説明します。
title: メッシュベースの入力
user-guide-description: ""
user-guide-title: ""
source-git-commit: 4432887b652896f77fc3c99010436ef44aeb8a3e
workflow-type: tm+mt
source-wordcount: '279'
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
| *位置(RGB)* | **メッシュ\_位置** | **meshPosition** | 頂点位置を含むテクスチャを取得します。 |
| *ワールド空間法線 (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | ワールド空間内のnormal頂点を含むテクスチャを取得します。 |
| *正接(RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | ワールド空間内の頂点正接を含むテクスチャを取得します。 |
| *ワールド空間のBitangent (RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | ワールド空間内の頂点のバイ正接(bi-normal)を含むテクスチャを取得します。 |
| *テキストサイズ（グレースケール）* | **メッシュ\_texel\_size** | **meshTexelSize** | テクセルサイズ（ピクセル密度とUVの差）を含むテクスチャを取得します。 |
| *UV マスク （グレースケール）* | **メッシュ\_uv\_mask** | **meshUVMask** | テクスチャをメッシュUV アイランドの黒（外側）マスクおよび白（内側）マスクとして取得します。 |
| *UV近隣ノード(RGB)* | **メッシュ\_uv\_neighbor** | **meshUVNeighbor** | 2つの情報を含むテクスチャを取得します。 UV アイランドの内側には、通常のUV座標が格納されます。 UV アイランドの外側には、UVシームの反対側の画素のUV座標が記憶されている。 このテクスチャを使用すると、シームレスな効果を作成できます。 |
