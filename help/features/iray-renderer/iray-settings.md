---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/iray-renderer/iray-settings.html"
breadcrumb-title: ''
description: Substance 3D PainterでRayレンダラーを設定し、レンダリングの品質やパフォーマンスを制御する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Iray Renderer > Iray Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 画像設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---


# 画像設定

![](../../assets/iray-settings.png)

Iray設定は、IRayビューポートのレンダリング、実行時間、および品質を制御します。

## Iray情報

ウィンドウの上部には、画像のステータスと他の情報が表示されます。

| *設定* | *説明* |
| --- | --- |
| **ステータス** | ステータスは、画像の動作を示します。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>レンダリング</strong> （Irayはイメージを計算中）</li><li data-preserve-html="true"><strong>一時停止</strong> （Irayは計算を停止しましたが、完了していません）</li><li data-preserve-html="true"><strong>完了</strong> （Iray計算が終了したか、設定値に達しました）</li></ul> |
| **解決策** | イメージイメージの解像度（既定値はビューポートサイズに依存）。 |
| **シーンサイズ** | シーン/3Dメッシュのバウンディングボックスのサイズ。 単位はないが、センチメートル単位と推定される。 |
| **反復回数** | 設定で定義されている最大値を超えてIRayが実行する計算パスの数。 |
| **レンダリング時間** | 設定で定義された最大時間を超えてレンダリングを実行した経過時間。 |

>[!NOTE]
>
> 反復の数は、レンダーの最終的な品質を定義します。反復の数が多いほど、品質は高くなります。\
> ただし、反復には時間がかかるため、最大時間を定義できます。 反復は、サンプルの数によって定義されます。

## 設定

設定が変更されると、Irayはレンダリングの計算を開始します。\
この動作を回避するために、専用ボタンを使用してIRayを一時停止することができます。

![](../../assets/pause-2.png)

| *設定* | *説明* |
| --- | --- |
| **最小サンプル** | ピクセル単位で実行するサンプルの最小量 |
| **最大サンプル数** | ピクセル単位で実行するサンプルの最大量 |
| **最大時間** | IRayが計算を実行できる最大時間。  右側のドロップダウンでは、単位（秒、分、時間）を設定できます。 |
| **コースティックSamplerが有効になりました** | このオプションを使用すると、より高度なライティング反射（コースティクス）を計算できます。 |
| **Fireflyフィルターが有効になりました** | このオプションを使用すると、ときどき発生する単色の非常に明るいピクセルを除去できます。 |
| **ビューポートの解像度を上書き** | この設定を使用すると、現在のビューポートサイズを使用する代わりに、レンダリングのカスタムサイズを定義できます。 下の&#x200B;**幅**&#x200B;と&#x200B;**Height**&#x200B;の設定により、ピクセル数で定義できます。 |
| **レンダリングを保存** | 現在のレンダリングを（未完了の場合でも）ファイルに書き出すアクション。 |
| **共有** | 現在のレンダリングを[ArtStation](https://www.artstation.com/)に共有またはエクスポートできるようにします。 |
