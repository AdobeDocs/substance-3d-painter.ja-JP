---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/assets/navigation.html"
breadcrumb-title: ''
description: Substance 3D Painterのアセットパネルを移動して、リソースライブラリを効率的に参照およびアクセスする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Navigation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ナビゲーション
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 1%

---


# ナビゲーション

「アセット」ウィンドウには、パンくず、検索フィールド、アセットタイプアイコンなど、いくつかのナビゲーション方法があります。 すべてのナビゲーションタイプは相互に依存するので、これらの検索を組み合わせて活用できます。\
例えば、アセットタイプアイコンで「マテリアル」が選択されていても、ブレッドクラムを使用してスマートマスクフォルダーに移動した場合、アセットパネルには何も表示されません。マテリアルを表示する場合は「すべてのライブラリ」に戻り、スマートマスクを参照する場合は「マテリアル」を選択解除します。

## パンくず

ブレッドクラムを使用すると、ライブラリ内をすばやく移動できます。 矢印をクリックすると、ディスクへのアセットの保存方法が表示され、表示された場所を選択できます。 グレー表示されている場合は、選択したタイプのアセットがそのフォルダー内に存在しないことを意味しますが、その場所に移動することはできます。

![](../../assets/00-05-breadcrumbs.jpg)

## 検索フィールド

検索フィールドを使用すると、入力されたクエリを含むリソースをフィルタリングできます。 リソースのタイトルだけでなく、リソースの場所やリソース内のタグでも検索されることに注意してください。\
入力された検索は、単なるキーワードよりも高度な機能です。 [高度な検索クエリ](advanced-search-queries.md)を参照してください。

![](../../assets/00-05-searchfield.jpg)

## アセットタイプ

>[!NOTE]
>
> クリック時に&#x200B;**Ctrl**&#x200B;を維持することで、アセットタイプのアイコンを複数選択できます。

デフォルトでは「マテリアル」が選択されていますが、他のアセットタイプアイコンをクリックすると、他のタイプのリソースが表示されます。

![](../../assets/00-05-assettypeicons.jpg)

| アセットタイプ | 説明 |
| --- | --- |
| マテリアル <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1-1.png"/></div> | *basematerial*&#x200B;としてインポートされた.sbsarと、塗りつぶしレイヤーから作成されたマテリアルを含みます（プリセットの作成について詳しくは、[こちら](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/creating-and-saving-a-preset-180191514.html)を参照してください）。これらは塗りつぶしレイヤーで使用できる基本マテリアルで、メッシュまたはテクスチャセットの領域全体に適用されます。 |
| スマートマテリアル <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-7.png"/></div> | フォルダー内に保存された複数のレイヤーから成るより複雑なマテリアルを含みます（スマートマテリアルは自分で作成できるプリセットでもあります）。ベースマテリアルと同様に、スマートマテリアルはメッシュー/テクスチャセット全体に適用されますが、曲率、オクルージョン、その他のサーフェスの詳細など、メッシュの個々の情報も考慮されます。 これらの画面の詳細を取得してスマートマテリアルを正しく使用するには、まずメッシュを[ベイク](../../baking/baking.md)する必要があります。 |
| スマートマスク <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-2.png"/></div> | 複数のレイヤーエフェクトやジェネレーターを使用する、より複雑なマスクが含まれています。 自分でスマートマスクプリセットを[作成](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)できます。スマートマテリアルと同様に、スマートマスクが正しく動作するには、メッシュからベイク処理された情報が必要です。 |
| フィルター <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-3.png"/></div> | *filter*&#x200B;としてインポートされた.sbsarファイルを含みます。フィルターとは、既に存在するテクスチャを取り込み、何らかの方法で変形するエフェクトです。 白黒のマテリアルのみで機能するフィルターもあれば、情報の入力のみで機能するフィルターもあります。つまり、すべてのフィルターをマスクで使用できるわけではありません。 |
| ブラシ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-4.png"/></div> | ブラシ、パーティクル、ツールが含まれています。 Painterで[作成](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)できるすべてのプリセットです。**ブラシ**&#x200B;はアルファを使用する基本的な白黒プリセットです。 ブラシを使用して、任意またはすべてのチャンネルまたはマスクでペイントを設定できます。**パーティクル**&#x200B;はブラシと同じ特性を持ちますが、メッシュとの物理的なインタラクションをシミュレートするパラメーターセットも備えています。 これらは、液体こぼれ、滴り、雨、または物理的なシミュレーションを必要とするその他の効果を生み出すことができます。**ツール**&#x200B;には、ブラシやパーティクルのビヘイビアーを含めることができますが、このプリセットはマテリアルチャンネル情報とともに保存されます。 |
| アルファ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-5.png"/></div> | 様々なアルファと、より複雑な効果（Photoshopのような、動的ストローク、ペイントローラー）を持つブラシを[作成](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)できる複数のブラシメーカーを含みます。Alphaは、黒い部分が透明に見えるグレースケールイメージです。 |
| テクスチャ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-6.png"/></div> | グランジ、手続き、ベイク済みマップ、ハードサーフェス法線、およびLUTを含みます。**グランジ**&#x200B;は、興味深いノイズとテクスチャを持つグレースケールイメージです。 これを使用して、マスクを介して、またはチャンネルに直接プラグインすることで、メッシュのサーフェスにバリエーションを追加できます。**プロシージャ**&#x200B;も、ノイズや規則的なパターンで構成されるグレースケールのテクスチャです。 ただし、一部の静的なグランジとは異なり、プロシージャは繰り返しなしでスケールでき、（ランダムシードを介して）無限のバリエーションを持つ動的なビットマップです。**ベイク済みマップ**&#x200B;は、メッシュから抽出されたサーフェスとシェイプの情報を表します。 ベイク処理の詳細については、こちらを参照してください。**ハードサーフェス法線**&#x200B;は、法線チャンネルを使用してメッシュに直接スタンプできる詳細です。**LUT** （参照テーブル）は、表示テクスチャで使用してビューポートのカラープロファイルのビヘイビアーをシミュレーションできるカラープロファイル設定です。 カラープロファイルについて詳しくは、[こちら](../../features/post-processing/color-profile.md)を参照してください。 |
| 環境マップ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1.jpg"/></div> | *environment*&#x200B;として読み込まれたイメージを含みます（通常は.hdrまたは.exr）。環境マップは、照明の設定を自動的に生成する背景イメージです。 環境マップを使用するには、ビューポートに直接ドラッグするか、[表示設定]を使用します。 |
