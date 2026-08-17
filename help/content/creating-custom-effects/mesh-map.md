---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/content/creating-custom-effects/mesh-map.html"
breadcrumb-title: ''
description: Substance 3D Painterのカスタムエフェクトでメッシュマップを使用して、ジオメトリベースのテクスチャ情報にアクセスする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Map
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュマップ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%

---


# メッシュマップ

エフェクトがレイヤーに追加されたときにメッシュマップ（ベイクドテクスチャ）を自動的に接続するには、特定の命名規則に従う必要があります。

>[!NOTE]
>
> 入力ノードで&#x200B;**使用法**&#x200B;または&#x200B;**識別子**&#x200B;のいずれかを使用できます（使用法が優先されます）。

各メッシュマップの命名規則は次のとおりです。

| メッシュマップ | 使用状況 | 識別子 |
| --- | --- | --- |
| *環境オクルージョン* | **ambientOcclusionBase** | **アンビエント\_オクルージョン** |
| *ID* | **id** | **id** |
| *曲線* | **曲率** | **曲率** |
| *標準* | **normalBase** | **normal\_base** |
| *ワールド空間法線* | **normalWS** | **world\_space\_normals** |
| *位置* | **位置** | **位置** |
| *Thickness* | **Thickness** | **Thickness** |
| *Height* | **heightBase** | **Height\_ベース** |
| *曲がった法線* | **bentNormalsBase** | **bent\_normals\_base** |
| *不透明度* | **不透明度ベース** | **不透明度\_base** |
