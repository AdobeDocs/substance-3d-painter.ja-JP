---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/display-settings/environment-settings.html"
breadcrumb-title: ''
description: Substance 3D Painterで環境設定を行い、マテリアルプレビューの照明と背景を制御する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Environment settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 環境設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---


# 環境設定

**表示設定**&#x200B;のこのセクションは、ビューポートの照明を制御します。

## 環境

![](../../assets/env-settings.png)

| *設定* | *説明* |
| --- | --- |
| **環境マップ** | シーンのライティングに使用する環境マップテクスチャ。 「環境」プリセットを使用して、[アセット](../assets/assets.md)ウィンドウで見つけることができます。ボタンをクリックしてミニシェルフを開き、別の環境マップを選択します。 |
| **環境マップのカラースペースを上書き** | 現在のプロジェクトで[カラーマネジメント](../../features/color-management/color-management.md)を使用している場合、この設定を有効にして、環境マップのカラースペースを上書きできます。 |
| **環境の不透明度** | ビューポートのバックグラウンドでの環境テクスチャの可視性/不透明度を制御します。 この設定は、シーンのライティングには影響しません。 |
| **環境の露出** | 露出値(EV)は、固定されたシーンの輝度を表す数値です。 この設定により、デフォルトのルミナンス値をオフセットできます。アプリケーションに付属の環境マップを使用する場合、この設定は0のままにする必要があります。 誤った露光量の値でアセットをテクスチャリングすると、他のアプリケーションでカラーキャリブレーションの問題が発生する可能性があります。 |
| **環境のローテーション** | 環境テクスチャの水平方向の回転を制御します。 シーン内の照明を回転させ、オブジェクトの反応を変更する場合に便利です。 [ショートカット](../settings/shortcuts.md)で制御できます。 |
| **環境ぼかし** | ビューポートのバックグラウンドに表示される環境テクスチャのシャープまたはぼかしの度合いを制御します。 この設定は、照明には影響しません。 |
| **環境の調整** | ビューポート内の3Dモードを中心に環境テクスチャを回転させる方法をコントロールします。 この設定をローカルに設定すると、3Dモデルの下の領域を明るくすることができます。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ワールド</strong> （既定値）：環境はシーンに合わせて、3Dモデルの上軸を中心に回転します。</li><li data-preserve-html="true"><strong>ローカル</strong>：環境はカメラに位置合わせされ、カメラの上軸を中心に回転します。</li></ul> |

## シャドウ

![](../../assets/shadow-2.png)

| *設定* | *説明* |
| --- | --- |
| **シャドウ** | ビューポートでのシャドウのレンダリングを有効/無効にします。 |
| **計算モード** | シャドウの計算速度を制御します。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>負荷の高い</strong> ：高速に計算できますが、ビューポートのレンダリングはフリーズする可能性があります。</li><li data-preserve-html="true"><strong> Average </strong> ：集中型モードとライトウェイトモードの平均です。</li><li data-preserve-html="true"><strong>軽量</strong> : （既定）計算すると数秒間で影の速度が遅くなりますが、ビューポートのパフォーマンスは低下しません。</li></ul> |
| **シャドウの不透明度** | シーンに表示されるシャドウの量を制御します。 |
