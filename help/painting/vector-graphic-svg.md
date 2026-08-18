---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/painting/vector-graphic-svg.html"
breadcrumb-title: ''
description: Substance 3D Painterでベクターグラフィック（SVGおよびAIファイル）を使用して、スケーラブルなベクターアートワークをテクスチャに加える方法について説明します。
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ベクターグラフィック(SVG)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---


# ベクターグラフィック（.svgおよび.ai）

![パラメーターのリストの横のメッシュに投影されたSVGファイルを示す画像](../assets/svg_overview.png)

ベクターグラフィックファイル（<b>.svg</b>とIllustrator <b>.ai</b>）は、Painter内に通常の画像のように読み込むことができます。 いくつかの設定を使用して、グラフィックの外観を調整し、テクスチャリングの残りの部分に合わせることができます。

* SVGファイルの詳細については、[このページを参照](https://www.adobe.com/creativecloud/file-types/image/vector/svg-file.html)してください。
* AIファイルの詳細については、[このページを参照](https://www.adobe.com/ie/creativecloud/file-types/image/vector/ai-file.html)してください。

[レイヤースタック](../interface/layer-stack/layer-stack.md)内で使用すると、SVGおよびAIファイルが自動的にピクセルイメージに変換されます（選択した設定によって異なります）。 これは非破壊的なプロセスであり、解像度を変更したり、ソースファイルを更新したりすると、それに応じて最終結果が更新されます。

## プロパティ

ベクターファイルを読み込み、レイヤーまたはツールプロパティ内に読み込むと、以下の一連のパラメーターを使用できます。

| セクション | 設定 | 説明 |
| --- | --- | --- |
| <b>アートボード</b> | <b>アートボード</b> | ファイルに含まれている、使用するアートボードを選択します。  **注意：**&#x200B;この設定は、Illustrator (.ai)ファイルでのみ使用できます。 |
| <b>解決策</b> | 解決策 | レイヤースタック内でテクスチャリングに使用する際にsvgがビットマップ画像（ピクセル）に変換されるサイズを定義します。   有効な値：<ul data-preserve-html="true"> <li data-preserve-html="true"><b>自動</b>：解像度は、現在のテクスチャセットの解像度（塗りつぶしレイヤー/効果で使用した場合）、またはブラシツールで使用した場合は512ピクセルの解像度によって決定されます。<br/> </li> <li data-preserve-html="true"><b>アセット</b>：解像度は、SVGファイル自体の内部で定義されたピクセルサイズによって決定されます。<br/> </li> <li data-preserve-html="true"><b>カスタム</b>：解像度は、インターフェイスのすぐ下にある解像度の設定によって決定されます。</li> </ul>  <div><img alt="svg解像度の設定" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-ad42696-column-7212622_image" src="../assets/svg_resolution_custom.png" title="svg解像度の設定"/></div> |
|  |  |  |
| <b>切り抜き領域</b> | トリミング先 | レンダリングされた領域にSVGのシェイプを制限する方法を定義します。   有効な値：<ul data-preserve-html="true"> <li data-preserve-html="true"><b>アセットの境界</b>：領域は、SVGファイル内で定義された境界によって定義されます。</li> <li data-preserve-html="true"><b>カスタム</b>：領域は、すぐ下のインターフェイスの設定を使用して明示的な値で定義されています。<br/> </li> </ul> |
|  | 正方形のアスペクト比 | 切り抜き領域が<b>アセットの境界</b>で定義されている場合、この設定によって元の縦横比が確実に維持され、SVGを正方形の画像としてレンダリングする際に誤った伸縮が行われるのを防ぐことができます。   この設定により、一部の要素が予期せずに表示される場合があります。 この問題を回避するには、この設定を無効にし、塗りつぶしレイヤー/エフェクト内でUV設定を手動で調整します。 |
|  | 左上、右下 | 切り抜きがカスタム領域に設定されている場合、これらの設定を使用して左上と右下のコーナーを指定することで、手動で領域を定義できます。 |
|  |  |  |
| <b>スコープ</b> | 範囲 | SVGファイルをレンダリングする前に、ファイル内のどのエレメントを含めるかを指定します。   デフォルトは<b>Document</b>で、SVGファイルのすべてのコンテンツが使用されます。 <b>変更</b>ボタンを使用して、含める要素を調整します。 |

### スコープウィンドウ

ベクターグラフィックの範囲を編集すると（上記の設定を参照）、最終的なレンダリングイメージに含めるまたは除外する要素を指定する選択をする要素のリストがウィンドウに表示されます。

各要素の画像を表示するには、<b>[サムネイルの表示]</b>チェックボックスを使用します。

![](../assets/v10_ai_thumbs.jpg)
