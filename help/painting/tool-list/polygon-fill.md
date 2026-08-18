---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/polygon-fill.html"
breadcrumb-title: ''
description: Substance 3D Painterの多角形の塗りつぶしツールを使用して、選択した多角形をペイントで塗りつぶすことで、効率的にテクスチャペイントを行います。
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Polygon fill
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ポリゴン塗りつぶし
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 1%

---


# ポリゴン塗りつぶし

**多角形の塗りつぶし**&#x200B;ツール(![](../../assets/image2018-6-12-18-15-12.png))を使用すると、選択した多角形をピクセルマスクに変換することで、マスクをすばやく描画できます。 他の3DCCアプリケーションの3D選択ツールのように見えるかもしれませんが、実際にはピクセルデータを生成するペイント塗りつぶしツールです。 つまり、選択と選択解除を切り替えて、白または黒にペイントします。

多角形の塗りつぶしツールは、[ペイントレイヤー](../../interface/layer-stack/layer-stack.md)で機能しますが、ベースカラーのみに制限され、この目的には使用できません。 [マスクのみに使用](../../interface/layer-stack/masking-and-effects.md)。

4つの選択モードがあります。

* ![](../../assets/image2020-9-30-11-31-53.png) **三角形の塗りつぶし** – 個々のメッシュの三角形を塗りつぶします。
* ![](../../assets/image2020-9-30-11-32-12.png) **ポリゴン塗りつぶし** – ポリゴン全体を塗りつぶします。 書き出し時にメッシュがすでに三角形分割されている場合は、「三角形塗りつぶし」以外の操作は行わないでください。
* **![](../../assets/image2020-9-30-11-32-42.png)メッシュ塗りつぶし** – 接続されたサブメッシュ全体を塗りつぶします。 3Dアプリケーションの「サブオブジェクト」モードと同様に、クリックしたポリゴンに接続されているすべてのポリゴンを塗りつぶします。
* **![](../../assets/image2020-9-30-11-32-54.png)UVチャンクの塗りつぶし** - UVチャンクまたは「島」全体を塗りつぶします。 メッシュフィルと同様に機能しますが、UV空間で接続されたポリゴンを見ることによって動作します。 UV境界で塗りつぶしが停止します。

![](../../assets/polygon-fill.gif)

これらの4つのモードは組み合わせたり切り替えたりすることができます。つまり、ある程度のスマートな使用方法により、メッシュおよびUVチャンクモードを使用して、マスク内のセクションをすばやくマークおよびアンマークできます。

（デフォルト）ポリゴンフィルツールに関連するホットキーは次のとおりです。

* *数値キー4* – 多角形の塗りつぶしツールを選択します。
* *X* – マスクをペイントするときに現在の色を反転します。 黒を白にすばやく入れ替えます。 マテリアルペイントモードでは、このホットキーは無効です。
