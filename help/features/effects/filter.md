---
title: フィルター
description: Substance 3D Painterでフィルター効果を使用して、画像処理フィルターとテクスチャ補正を適用する方法を説明します。
source-git-commit: 4b8afda243f2969b036efe14588f201177ee3139
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 3%
---

# フィルター

フィルターエフェクトは、レイヤーまたはマスクの内容を変形する物質です。 通過描画モードでは、レイヤーでレイヤースタック結果を編集できます。通過描画モードのレイヤーでフィルターを使用すると、フィルターを使用してレイヤースタック全体を編集できます。

## フィルターを適用するにはどうすればよいですか？

フィルターの種類に応じて、レイヤーのコンテンツまたはマスクにフィルター効果を作成する必要があります。 フィルターを適用するには、次の2つの方法があります。

* 手動アプローチでは、フィルタを設定するために複数のステップが必要ですが、プロセスの各ステップを直接制御できます。
* ドラッグ&amp;ドロップを使用すると、フィルターをすばやく追加して、描画モードをすべてのチャンネルを通過するように自動的に設定できます。

### 手動でフィルターを追加する

次の例ではぼかしフィルターがレイヤーのコンテンツに適用されていますが、マスクへのフィルターの適用により広く使用されています。

**1. フィルター効果の追加**

まず、レイヤーのコンテンツまたはレイヤーマスクを選択し、**効果ボタン**&#x200B;をクリックします（または右クリックしてコンテキストメニューを開きます）。 リストの「 **フィルターを追加** 」オプションを選択します。

![](../../assets/filters/filter-add-manually.gif)

**2. プロパティウィンドウでフィルターを選択します**

**プロパティパネル**&#x200B;で、フィルターがまだ選択されていません。 「フィルターの選択」ボタンをクリックしてミニシェルフを開き、目的のフィルターを選択します。ここでは、**ぼかしフィルター**を選択します。
![](../../assets/filters/filter-select.gif)

>[!NOTE]
>
> フィルタを手動で適用する場合、そのフィルタが下層のレイヤのコンテンツに作用するようにするには、パススルー描画モードを使用する必要があります。

## シェルフからのフィルターのドラッグ&amp;ドロップ

このメソッドは、Layerstack全体に適用するフィルタのみを対象としています。 すべてのチャンネル[描画モード](../../interface/layer-stack/blending-modes.md)が自動的に設定されます。 マスクにフィルターを適用することはできません。

**1. シェルフ**&#x200B;のフィルター領域を開きます

シェルフで、左側にある「フィルター」セクションをクリックします。

![](../../assets/shelf-filters.gif)

**2. フィルター**&#x200B;をドラッグアンドドロップします

シェルフで使用するフィルターを選択します。 レイヤースタックにドラッグ&amp;ドロップして、正しい場所に配置されていることを確認します（例えば、不要なグループにドロップすることは避けます）。

![](../../assets/filter-dragdrop.gif)

上記の例では、ドロップされたフィルターには既に通過描画モードが設定されています。 これは、ドキュメントのすべてのチャンネルに当てはまります。

## Painterに新しいフィルターを追加する

Painterに取り込む新しいフィルターがある場合は、通常のリソースを追加する場合と同様に追加できます。Sbsar ファイルを&#x200B;**アセットパネル**&#x200B;にドラッグ&amp;ドロップするだけで、新しいフィルターの読み込みを管理できるようになります。

## 独自のフィルターの作成

すべてのフィルターはSubstanceで、Substance 3D Designerを使用して作成できます。 Substance 3D Designerには、すぐに使い始めるのに役立つSubstance 3D Painter用のテンプレートが用意されています。

詳しくは、次のページを参照してください： [カスタムエフェクトの作成](../../content/creating-custom-effects/creating-custom-effects.md)

## Painterのデフォルトのフィルター

### 標準

* [ブラー](filters/standard/blur.md)
* [ブラー（方向）](filters/standard/blur-directional.md)
* [ぼかし勾配](filters/standard/blur-slope.md)
* [クランプ](filters/standard/clamp.md)
* [カラーバランス](filters/standard/color-balance.md)
* [カラー補正](filters/standard/color-correct.md)
* [コントラストの輝度](filters/standard/contrast-luminosity.md)
* [ドロップシャドウ](filters/standard/drop-shadow.md)
* [塗りつぶし領域のカラー](filters/standard/fill-area-color.md)
* [塗りつぶし領域マスク](filters/standard/fill-area-mask.md)
* [FXA（アンチエイリアス）](filters/standard/fxaa-anti-aliasing.md)
* [光彩](filters/standard/glow.md)
* [グラデーション](filters/standard/gradient.md)
* [グラデーション動的](filters/standard/gradient-dynamic.md)
* [グレースケール変換](filters/standard/grayscale-conversion.md)
* [ハイパス](filters/standard/highpass.md)
* [ヒストグラムスキャン](filters/standard/histogram-scan.md)
* [ヒストグラムシフト](filters/standard/histogram-shift.md)
* [HSL Perceptive](filters/standard/hsl-perceptive.md)
* [反転](filters/standard/invert.md)
* [ミラー](filters/standard/mirror.md)
* [ピクセル化](filters/standard/pixelate.md)
* [ポスタリゼーション](filters/standard/posterize.md)
* [シャープ](filters/standard/sharpen.md)
* [滑らかさ](filters/standard/smoothstep.md)
* [しきい値](filters/standard/threshold.md)
* [変形](filters/standard/transform.md)
* [縦糸](filters/standard/warp.md)

### 仕上げ

* [艶消し仕上げ線形ブラシ](filters/finishes/matfinish-brushed-linear.md)
* [MatFinish亜鉛メッキ](filters/finishes/matfinish-galvanized.md)
* [粒状マット仕上げ](filters/finishes/matfinish-grainy.md)
* [艶消し仕上げ](filters/finishes/matfinish-grinded.md)
* [MatFinishハンマー](filters/finishes/matfinish-hammered.md)
* [塗り潰し仕上げ穴あき円](filters/finishes/matfinish-perforated-circles.md)
* [艶消し仕上げ粉体塗装](filters/finishes/matfinish-powder-coated.md)
* [MatFinish Raw](filters/finishes/matfinish-raw.md)
* [粗い仕上げ](filters/finishes/matfinish-rough.md)

### MatFX

* [MatFXコミック](filters/matfx/matfx-comic-book.md)
* [MatFX詳細Edge Wear](filters/matfx/matfx-detail-edge-wear.md)
* [MatFXエッジの損害](filters/matfx/matfx-edge-damages.md)
* [MatFX HBAO](filters/matfx/matfx-hbao.md)
* [MatFX石油ペイント](filters/matfx/matfx-oil-paint.md)
* [MatFX剥離ペイント](filters/matfx/matfx-peeling-paint.md)
* [MatFX風化](filters/matfx/matfx-rust-weathering.md)
* [MatFXシャットダウンライン](filters/matfx/matfx-shut-line.md)
* [MatFX水彩画](filters/matfx/matfx-watercolor.md)
* [MatFX水滴](filters/matfx/matfx-water-drops.md)

### 光源

* [ベイク済み照明環境](filters/lighting/baked-lighting-environment.md)
* [ベイク照明スタイル化](filters/lighting/baked-lighting-stylized.md)

### アドバンス

* [異方性桑原](filters/advanced/anisotropic-kuwahara.md)
* [ベベル](filters/advanced/bevel.md)
* [ベベルスムーズ](filters/advanced/bevel-smooth.md)
* [カラーマッチ](filters/advanced/color-match.md)
* [方向の距離](filters/advanced/directional-distance.md)
* [グラデーションカーブ](filters/advanced/gradient-curve.md)
* [Height調整](filters/advanced/height-adjustments.md)
* [Heightを標準に](filters/advanced/height-to-normal.md)
* [アウトラインをマスク](filters/advanced/mask-outline.md)
* [PBR 検証](filters/advanced/pbr-validate.md)
* [量子化](filters/advanced/quantize.md)
* [スタイル化](filters/advanced/stylization.md)
* [3-平面上級](filters/advanced/tri-planar-advanced-filter.md)
