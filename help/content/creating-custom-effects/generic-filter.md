---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/content/creating-custom-effects/generic-filter.html"
breadcrumb-title: ''
description: Substance 3D Painterの汎用フィルターエフェクトを使用して、カスタム画像処理とテクスチャフィルターを適用する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Generic filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 汎用フィルター
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# 汎用フィルター

一般的な効果は、不透明度を含むすべてのドキュメントチャンネルに適用されます。 汎用フィルターには、次の種類があります。

* **グレースケール**、各チャンネル（ベースカラー、メタリック、粗さなど）の各コンポーネント(R、G、B、A)に適用されます
* **カラー**&#x200B;です。これは、カラーチャンネルにそのまま適用されるか、内部でグレースケールに変換されて、グレースケールチャンネルに影響を与えます

エフェクトの入力ノードには、**識別子**&#x200B;または&#x200B;**使用方法**&#x200B;が定義されている&#x200B;**入力**&#x200B;が必要です。出力ノードには、**出力**&#x200B;が必要です。 **カラー**&#x200B;ベースのフィルターはレイヤーのマスクには使用できません。互換性があるのは&#x200B;**グレースケール**&#x200B;フィルターのみです。

>[!NOTE]
>
> 入力ノードで&#x200B;**使用法**&#x200B;または&#x200B;**識別子**&#x200B;のいずれかを使用できます（使用法が優先されます）。

例：

![](../../assets/generic-filter.png)![](../../assets/generic-rgba.png){width="575px"}
