---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/display-settings/camera-settings.html"
breadcrumb-title: ''
description: Substance 3D Painterでカメラを設定し、ビューポートカメラのビヘイビアーと投影を制御する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Camera settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: カメラ設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 3%

---


# カメラ設定

**ディスプレイの設定**&#x200B;のこのセクションでは、ビューポートの動作とカメラの最終的な外観を制御します。

## カメラ

| *設定* | *説明* |
| --- | --- |
| **視野** | カメラの視野を（度単位で）コントロールできます。 |
| **焦点距離** | フォーカスポイントが位置する距離を定義します。  このポイントは「フィールドの深度」エフェクトで使用されます。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **注意：** メッシュのポイントをショートカット **CTRL +マウスの中央ボタン**&#x200B;でクリックすると、フォーカスの距離を自動で設定できます |
| **アパーチャ** | フィールドの深度の幅を指定します。 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **注意：** Irayがこのパラメーターを制御している場合、このパラメーターを変更すると計算が再トリガーされます。 |

## ポストエフェクト

![](../../assets/post.png)

詳細については、[効果の適用後のページ](../../features/post-processing/post-processing.md)を参照してください。

## テンポラルアンチエイリアシング

![](../../assets/taa.png)

有効にすると、**テンポラルアンチエイリアシング** (**TAA**)はビューポート内のギザギザのエッジを削除します。\
**TAA**&#x200B;は、複数のレンダリングフレームに渡って情報を蓄積することで機能します。つまり、カメラが動かなくなるまで、またはその他の処理が行われるまで、このエフェクトは無効になります。

| *設定* | *説明* |
| --- | --- |
| **累積** | エイリアスを減らすために累積するフレームの数を指定します。<ul data-preserve-html="true"> <li data-preserve-html="true">16：ほとんどの場合、お勧めの価値があります。</li> <li data-preserve-html="true">64：高コントラスト値（Alphaテストシェーダーとディザリングの組み合わせなど）を補正する場合に有用</li> </ul>  **注意：**&#x200B;この設定はパフォーマンスに影響しませんが、値を大きくすると、適切な結果が得られるまでに時間がかかる場合があります。 |

![](../../assets/temporal-anti-aliasing.gif){width="500px"}

設定「**シェーダー**」が有効になっている場合は、アンチエイリアスを使用して&#x200B;**Alphaテスト**&#x200B;のアルファディザリングをフィルターすることもできます。

![](../../assets/dithering-aa.gif){width="500px"}

## サブサーフェススキャッタリング

![](../../assets/subscat.png)

詳細については、[表面化散乱](../../features/subsurface-scattering/subsurface-scattering.md)のページを参照してください。

## カラープロファイル

![](../../assets/profile-13.png)

詳細については、[カラープロファイルページ](../../features/post-processing/color-profile.md)を参照してください。

## トーンマッピング

| 設定 | 説明 |
| --- | --- |
| **関数** | モニターの表示能力（LDR範囲へのHDR 値の再マッピング）を超えるカラー値に合わせるために使用する関数を指定します。指定できる値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>線形</strong> （既定値）：変換なし。1.0を超える値はクランプされます。</li><li data-preserve-html="true"><strong>ACE</strong>: ACE Filmicトーンマッピングカーブを使用します。</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/linear-vs-aces.jpg" width="450px"/></div> **注意：**&#x200B;一部のゲームエンジンおよびレンダリングソフトウェアでは、ACEトーンマッパーが使用されています。 この機能を有効にすると、アプリケーション間で色を一致させることができ、違いを避けることができます。 |
