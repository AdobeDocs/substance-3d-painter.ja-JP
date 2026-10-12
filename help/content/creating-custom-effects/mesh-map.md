---
breadcrumb-title: ""
description: Substance 3D Painterのカスタムエフェクトでメッシュマップを使用して、ジオメトリベースのテクスチャ情報にアクセスする方法について説明します。
title: メッシュマップ
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%
---

# メッシュマップ

エフェクトがレイヤーにベイクされたときにメッシュマップ（追加されたテクスチャ）を自動的に接続するには、所定の命名規則に従う必要があります。

>[!NOTE]
>
> 入力ノードで&#x200B;**使用**&#x200B;または&#x200B;**識別子**&#x200B;のいずれかを使用できます（使用が優先されます）。

各メッシュマップの命名規則は次のとおりです。

| メッシュマップ | 使用状況 | 識別子 |
| --- | --- | --- |
| *Ambient occlusion* | **ambientOcclusionBase** | **アンビエント\_オクルージョン** |
| *ID* | **id** | **id** |
| *曲率* | **曲率** | **曲率** |
| *標準* | **normalBase** | **normal\_base** |
| *ワールド空間法線* | **normalWS** | **world\_space\_normals** |
| *位置* | **位置** | **位置** |
| *Thickness* | **Thickness** | **Thickness** |
| *Height* | **heightBase** | **Height\_ベース** |
| *Bent normals* | **bentNormalsBase** | **bent\_normals\_base** |
| *不透明度* | **不透明度ベース** | **不透明度\_base** |
