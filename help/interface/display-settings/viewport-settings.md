---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/display-settings/viewport-settings.html"
breadcrumb-title: ''
description: Substance 3D Painterのビューポート設定を変更して、表示オプションとレンダリング品質をカスタマイズする方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Viewport settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ビューポート設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 2%

---


# ビューポート設定

**表示設定**&#x200B;のこのセクションでは、テクスチャフィルタやメッシュワイヤーフレームなど、ビューポートの表示に関連するさまざまな設定を制御します。

## テクスチャのフィルタリング

![](../../assets/texture-filtering.png)

異方性反射フィルタリングとミップマップバイアスを使用すると、ビューポート内のテクスチャの表示を制御できます。 これらの設定はテクスチャに直接影響せず、書き出し時には適用されません。ビューポートでレンダリング処理を調整するだけです。 MipMap Bias設定を使用すると、遠くのピクセルや斜めのピクセルに対して非常にシャープなテクスチャを使用できますが、場合によってはモアレパターンやジッターが生じることがあります。

デフォルト設定は品質とパフォーマンスの妥協であり、本当に必要な場合にのみ変更してください。

| *設定* | *説明* |
| --- | --- |
| **異方性フィルタリング** | 異方性フィルタリングを使用すると、斜めの角度で表示する場合のテクスチャの品質が向上します。 高品質の値を指定すると、フィルタリングは向上しますが、パフォーマンスが低下する可能性があります。 この設定は、フィルタリングに使用される1ピクセルあたりのサンプル数(spp)を制御します。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>無効</strong> :フィルター処理なし</li><li data-preserve-html="true"><strong>低</strong> (2spp)</li><li data-preserve-html="true"><strong>中</strong> (4spp) :デフォルト値</li><li data-preserve-html="true"><strong>高</strong> (8spp)</li><li data-preserve-html="true"><strong>非常に高い</strong> (16spp)</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/quality-anisotropic-filtering.jpg"/></div> |
| **MipMapバイアス** | ディテールのミップマップレベルをオフセットして、テクスチャの画質を向上させます。 シャープな値にすると、パフォーマンスが低下したり、テクスチャがギザギザになる可能性があります。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>0 – ソフト</strong> （軽量パフォーマンス） ：既定値</li><li data-preserve-html="true"><strong>1 – 中ソフト</strong></li><li data-preserve-html="true"><strong>2 – シャープ</strong></li><li data-preserve-html="true"><strong>3 – 非常にシャープ</strong> （負荷の高いパフォーマンス）</li></ul>(0 ～ -3) |

## カメラフレーム

![](../../assets/camera-frame.png)

カメラ管理の詳細については、[カメラ管理](../viewport/camera-management.md)を参照してください

## ツールの表示

![](../../assets/viewport-tool.png)

| *設定* | *説明* |
| --- | --- |
| **描画時にステンシルを非表示にする** | ステンシルを使用する場合（ペイントツールのプロパティを参照）、この設定を使用すると、メッシュでペイントするときにステンシルを一時的に非表示にすることができます。 |
| **ステンシルの表示不透明度** | ペイントしないときのビューポートレンダリング上でのステンシルの可視性を制御します。 |
| **プロジェクションプレビューチャンネル** | 投影ツールを使用するときに表示するマテリアルのチャンネルをコントロールします。 |

## メッシュワイヤーフレーム

![](../../assets/viewport-mesh.png)

| *設定* | *説明* |
| --- | --- |
| **メッシュワイヤーフレームを表示** | ビューポートでのメッシュワイヤーフレームの表示を有効または無効にします。 |
| **ワイヤーフレームの色** | メッシュワイヤーフレームの描画に使用する色をコントロールします。 |
| **ワイヤーフレームの不透明度** | メッシュの上に描画されるワイヤーフレームの表示量をコントロールします。 |

## チャンネル表示

![](../../assets/viewport-channel.png)

>[!NOTE]
>
> チャンネルの表示設定は、**単一チャンネル**&#x200B;表示モードを使用する場合にのみ使用できます。

| *設定* | *説明* |
| --- | --- |
| **照明なしで単独のビューを表示（消灯）** | シングルチャンネルモードで表示している場合、この設定を有効にすると、照明が削除され、チャンネルが単色で表示されます。 無効にすると、メッシュの境界にシャドウが適用されます。 |
| **HDR値のスケール** | シングルチャンネルモードでHeightなどの&#x200B;**HDR**&#x200B;テクスチャを表示する場合、この設定により合計値がスケールされます。 これは、-1より大きい値や–1より小さい値を表示する場合に便利です。 結果は&#x200B;**スケールで分岐**&#x200B;したチャンネルに等しくなります。次の例では、Heightチャンネルの値は最大3です。 ただし、デフォルトでは拡大・縮小の値が変更されない限り表示されません。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-hdr.jpg"/></div> |
| **HDR値に+/ – 色を使用する** | この設定により、正の値を最初のカラーで置き換え、負の値を2番目のカラーで置き換えることで、HDRテクスチャをより簡単に表示できます。 ニュートラル値(0)は黒です。例： <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/colored-hdr.jpg"/></div> |
| **カラーチャンネル** | ビューポートビューモードを変更して、現在のチャンネルのR、G、B、またはAlphaコンポーネントのみを個別に表示します。 この設定は、マテリアル表示モードでは使用できません。 有効にすると、選択したカラーチャンネルの名前がビューポートに表示されます。  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_image" src="../../assets/color-channel.png"/></div>  有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>RGBA</strong> （既定）:カラーチャンネルで、透明度を持つすべてのコンポーネントを表示します。</li><li data-preserve-html="true"><strong>グレースケール+ Alpha</strong> （既定値）:グレースケールチャンネルで、透明度のあるグレースケール値を表示します。</li><li data-preserve-html="true"><strong>R</strong>:カラーチャンネルでは、赤のコンポーネントのみを表示します。</li><li data-preserve-html="true"><strong>G</strong>:カラーチャンネルでは、緑のコンポーネントのみを表示します。</li><li data-preserve-html="true"><strong>B</strong> :カラーチャンネルでは、青コンポーネントのみを表示します。</li><li data-preserve-html="true"><strong>Alpha</strong>：任意のチャンネルで、テクスチャの透明度のみを表示します。</li></ul> |

## グリッド

![](../../assets/display-settings-grid.png)

グリッド設定を使用すると、3Dビューポート内の3Dグリッドの描画を表示および制御できます。

グリッドの分割は、ズームと角度の現在のカメラレベルに基づいて自動的に行われます。 現在のグリッド単位は、ビューポートの左下に表示されます。

| 設定 | 説明 |
| --- | --- |
| **グリッドの表示** | 有効になっている場合は、グリッドを3Dビューポートに表示します。 |
| **軸** | ビューポートでグリッドが表示される軸を定義します。 これがアプリケーションのアップ軸であるため、デフォルト値はYです。 |
| **グリッドの色** | ビューポートに描画したときのグリッドの色。 |
| **グリッドの不透明度** | ビューポート内のグリッドの不透明度。 |
