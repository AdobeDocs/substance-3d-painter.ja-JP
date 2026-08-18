---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/dynamic-strokes/creating-custom-dynamic-strokes.html"
breadcrumb-title: ''
description: Substance 3D Painterでカスタム動的ストロークを作成し、独自のブラシストロークのビヘイビアーとエフェクトをデザインする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Creating Custom Dynamic Strokes
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: カスタム動的ストロークの作成
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# カスタム動的ストロークの作成

カスタム動的ストロークを作成するには、次の2つの方法があります。

* 既存のツールリソースを使用して新しいブラシ/Substanceプリセットを作成する
* 新しいSubstanceリソースを最初から作成します（[Substance 3D Designer](https://substance3d.adobe.com/display/SDDOC/Substance+Designer)が必要）。

また、問題を回避するために、カスタムSubstanceファイルを作成する前に、[動的なストロークのパフォーマンス](dynamic-stroke-performances.md)をお読みください。

## 既存のリソースの再使用

新しい動的ストロークを最初から作成するのは難しい場合があります。 最初に既存のリソースを使用し、調整して、新しいプリセットとして保存しておくと良いでしょう。

シェルフでニーズに合う互換性のあるリソースを見つけて、[プリセット](../presets/presets.md)のページを確認してください。

## 動的ストロークのカスタムSubstanceファイルの作成

以下に、Substanceグラフで動的ストロークに対してサポートされているパラメーターを示します。

| 変数ID | 説明 |
| --- | --- |
| <b>ランダムシード</b> | ランダムシードを表示した状態でSubstanceファイルを調理した場合、ダイナミックストローク機能を使用して調整できます。 |
| <b>stampIndex</b> | ブラシストロークをペイントするときに、<b>Integer1</b>がSubstance 3D Painterによって供給されます。 最小値と最大値は無視され、Substance 3D Painterでは無視されます。 |
| <b>stampCycleCount</b> | <b>Integer1</b> Painterは、Stamp Cycle Countパラメーターを表示するために、パラメーターのデフォルト、最小値、最大値を読み取ります。 このパラメーターは、作成される一意のSubstanceバリエーションの数を制御します。 |
| <b>$time</b> | <b>フロート1</b>は、経過時間（1ストロークあたり）に基づいてブラシストロークをペイントするときに、Substance 3D Painterによって送られます。 この特性は、多くのSubstanceバリエーションを生み出し、そのため性能に影響を与える可能性があります。 |
| <b>strokeSpacing</b> | <b>float1</b>ペイントされたストローク全体の現在の間隔値。 |
| <b>strokeSize</b> | <b>float1</b>ペイントされたストローク全体の現在のサイズ値です。 |
| <b>stampStrokePosition</b> | <b>integer1</b>ストロークの開始/開始を指定するために使用します。 終了値は、手動ペイントではなく、パスストロークでのみ使用できます。 有効な値：<ul data-preserve-html="true"> <li data-preserve-html="true">0 =中央</li> <li data-preserve-html="true">1 =開始</li> <li data-preserve-html="true">2 =終了</li> </ul>isstrokepositionactiveユーザータグを使用して無効にできます。 |
| <b>distanceAlongCurve</b> | <b>float1</b>パスに沿った指定スタンプの現在の距離。 この特性は、多くのSubstanceバリエーションを生み出し、そのため性能に影響を与える可能性があります。 <b>iscurvedistanceactive</b>ユーザータグを使用して無効にできます。 |
| <b>distanceMaxCurve</b> | <b>float1</b>パスツールで作成されたパスの全長です。 <b>iscurvedistanceactive</b>ユーザータグを使用して無効にできます。 |
| <b>pathCorner</b> | <b>integer1</b>リボンが使用しているコーナーの種類を示します。 有効な値：<ul data-preserve-html="true"> <li data-preserve-html="true">0 =コーナーなし</li> <li data-preserve-html="true">1 =左隅</li> <li data-preserve-html="true">2 =右隅</li> </ul> |
| <b>pathCornerAngle</b> | リボンパス上の角の<b>フロート</b>角度（ラジアン）。 正確な角度値に基づいてコーナーの外観を補正または調整するために使用できます。 |
| <b>patchLengthOnCurve</b> | <b>float</b> リボンパス上のセクション（パッチ）のサイズです。 <b>distanceAlongCurve</b>および<b>distanceMaxCurve</b>と組み合わせると、たとえば、パッチのサイズを正規化するために使用できます。 |
