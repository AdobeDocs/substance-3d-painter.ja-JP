---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/subsurface-scattering/subsurface-parameters.html"
breadcrumb-title: ''
description: Substance 3D Painterでサブサーフェス拡散パラメーターを設定して、リアルな半透明マテリアルを作成する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Subsurface Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: サブサーフェスパラメータ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# サブサーフェスパラメータ

Substance 3D Painterのリアルタイムのサブサーフェスの実装は、画面空間のサブサーフェスのスキャッタリング効果です。 制御するパラメーターについては、このページで説明します。\
現在の実装は、PIXAR[&#128279;](http://graphics.pixar.com/library/ApproxBSSRDF/)によって公開された「効率的なサブサーフェス散乱のための近似反射プロファイル」手法に基づいています。

これらのパラメーターに基づくマテリアルの例については、[サブサーフェスマテリアルタイプ](subsurface-material-type.md)を参照してください。

## シェーダ/MDLパラメータ

![](../../assets/shader-parameters.png)

[シェーダ設定](../../interface/shader-settings/shader-settings.md)ウィンドウで使用できます。

| *設定* | *説明* |
| --- | --- |
| **有効にする** | このシェーダ/mdlインスタンスのサブサーフェススキャタリングエフェクトをアクティブまたは非アクティブにします。  不要なマテリアルのSSS効果を無効にする場合に使用します。 |
| **散布の種類** | マテリアル内のライト吸収の動作を定義します。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>半透明</strong>：光がオブジェクトに深く浸透できる、ヒスイや大理石などの一般的なマテリアルに適しています。</li><li data-preserve-html="true"><strong>スキン</strong>：光がすばやく吸収され、表面近くの散乱のみが吸収されるオーガニックスキンに適しています。</li><li data-preserve-html="true"><strong>赤のシフト/レイリー</strong>：人間または生物のサーフェスの肌をシミュレートする場合は、肌の設定よりも正確です。</li></ul> |
| **スケール** | マテリアル内のライトの吸収の半径/深度を制御します。 このパラメータの動作は、シーン内のメッシュのサイズに応じて変化します。人間の大きさの頭のスケール0.0、0.2、1.0の比較：   <div><img data-preserve-html="true" src="../../assets/scale-sss.jpg" width="650"/></div> |
| **色** | マテリアルに吸収されたときの光のカラー。3色の比較：   <div><img data-preserve-html="true" src="../../assets/color-sss.jpg" width="650"/></div> |

### 表示設定パラメータ

![](../../assets/display-settings-1.png)

[表示設定](../../interface/display-settings/display-settings.md)ウィンドウで使用できます。

>[!NOTE]
>
> このパラメーター&#x200B;**は、サブサーフェス散乱効果の**&#x200B;リアルタイム&#x200B;**バージョンにのみ**&#x200B;影響します。

| *設定* | *説明* |
| --- | --- |
| **サンプル数** | 画面空間でサブサーフェスぼかしを生成するために実行されるサンプルの量を制御します。 サンプルが多いほどノイズは少なくなりますが、パフォーマンスに影響を与えます。サーフェスの近くで見たときの8、32、64のサンプルの比較：   <div><img data-preserve-html="true" src="../../assets/samples-sss-v2.jpg" width="650"/></div>  **注意：**&#x200B;サンプルの量を増やすことなく[カメラの設定](../../interface/display-settings/camera-settings.md)を有効にすることで、ノイズの量を減らすこともできます。 |
