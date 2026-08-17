---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/assets/navigation.html"
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
| マテリアル <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1-1.png"/></div> | *basematerial*&#x200B;として読み込まれた.sbsarと、塗りつぶしレイヤーから作成されたマテリアルを含みます（プリセットの作成について詳しくは、[こちら](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/creating-and-saving-a-preset-180191514.html)を参照してください）。これは、塗りつぶしレイヤーで使用できる基本マテリアルであり、メッシュまたはテクスチャセットの表面全体に適用されます。 |
| スマートマテリアル <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-7.png"/></div> | ベースマテリアルと同様に、スマートマテリアルはメッシュ/テクスチャセット全体に適用されますが、メッシュの個々の情報（曲率、オクルージョン、その他のサーフェスの詳細など）も考慮されます。 これらの表面のディテールを取得し、スマートマテリアルを正しく使用するには、最初にメッシュを[ベイク処理](../../baking/baking.md)する必要があります。 |
| スマートマスク <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-2.png"/></div> | 複数のレイヤーエフェクトやジェネレーターを使用する、より複雑なマスクが含まれています。 自分で[スマートマスクプリセットを作成](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)できます。スマートマテリアルと同様に、スマートマスクが正しく動作するには、メッシュからベイク処理された情報が必要です。 |
| フィルター <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-3.png"/></div> | *filter*&#x200B;としてインポートされた.sbsarファイルを含みます。フィルターは、既に存在するテクスチャを利用して、何らかの方法で変形するエフェクトです。 一部のフィルターは白黒情報でのみ機能し、マテリアル入力でのみ機能するフィルターもあります。つまり、すべてのフィルターをマスクで使用できるわけではありません。 |
| ブラシ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-4.png"/></div> | ブラシ、パーティクル、ツールが含まれています。 Painterで[作成](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)できるすべてのプリセットです。**ブラシ**&#x200B;はアルファを使用する基本的な白黒プリセットです。 ブラシを使用して、任意のチャンネルまたはすべてのチャンネルまたはマスクでペイントできます。**パーティクル**&#x200B;はブラシと同じ特性を持ちますが、メッシュとの物理的な相互作用をシミュレートする追加のパラメーターセットも備えています。 これらは、液体こぼれ、滴り、雨、または物理的なシミュレーションを必要とするその他の効果を生み出すことができます。**ツール**&#x200B;には、ブラシやパーティクルのビヘイビアーを含めることができますが、このプリセットはマテリアルチャンネルの情報とともに保存されます。 |
| アルファ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-5.png"/></div> | さまざまなアルファと、より複雑な効果（Photoshopのような効果、動的ストローク、ペイントローラー）を持つブラシを[作成](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)できる複数のブラシ制作者が含まれています。Alphaは、黒い部分を使用すると透明に見えるグレースケール画像です。 |
| テクスチャ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-6.png"/></div> | グランジ、プロシージャ、ベイク済みマップ、ハードサーフェス法線、およびLUTを含めることができます。**グランジ**&#x200B;は、興味深いノイズやテクスチャを含むグレースケール画像です。 これを使用して、マスクを介して、またはチャンネルに直接プラグインすることで、メッシュのサーフェスにバリエーションを追加できます。**プロシージャ**&#x200B;も、ノイズや規則的なパターンで構成されるグレースケールのテクスチャです。 ただし、一部の静的なグランジとは異なり、プロシージャは繰り返しなしでスケールでき、（ランダムシードを介して）無限のバリエーションを持つ動的なビットマップです。**ベイク済みマップ**&#x200B;は、メッシュから抽出されたサーフェスとシェイプの情報を表します。 ベイク処理の詳細については、こちらを参照してください。**ハードサーフェス法線**&#x200B;は、法線チャンネルを使用してメッシュに直接スタンプできるディテールです。**LUT** （ルックアップテーブル）は、表示設定で使用できるカラープロファイルのテクスチャで、ビューポートでのカラープロファイルの動作をシミュレートします。 カラープロファイルについて詳しくは、[こちら](../../features/post-processing/color-profile.md)を参照してください。 |
| 環境マップ <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1.jpg"/></div> | *環境*&#x200B;として読み込まれた画像を含みます（通常は.hdrまたは.exr）。環境マップは、照明の設定を自動的に生成する背景画像です。 環境マップを使用するには、ビューポートに直接ドラッグするか、[表示設定]を使用します。 |
