---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/painting/advanced-channel-painting/ambient-occlusion-painting.html"
breadcrumb-title: ''
description: Substance 3D Painterでambient occlusionマップに直接ペイントを付けて、リアルなシャドウと深度をテクスチャに加える方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Ambient Occlusion Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ambient occlusionペイント
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Ambient occlusionペイント

ambient occlusionチャンネルを使用すると、オブジェクトのアンビエントシャドウのディテールをペイントできます。 マテリアルから送信されるAOの詳細情報を入力したり、必要に応じて手動でベイクしたエラーを修正したりできます。

&#x200B;>> 

コンピューターグラフィックスでは、ambient occlusionはシェーディングとレンダリングの手法の1つであり、シーンの各点が周囲光にどの程度表示するかを計算するために使用されます。 一般的に、チューブの内部は表示された外側のサーフェスよりも塞がれているため、内側に入るほど照明は塞がれていきます（暗くなります）。 Ambient occlusionは、各サーフェスポイントについて計算されるアクセシビリティ値と見なすことができます。\
出典： &lt;https://en.wikipedia.org/wiki/Ambient_occlusion>

この計算の&#x200B;**result**&#x200B;は、「Ambient occlusion」マップという名前のビットマップに格納されています。 このマップは、アプリケーションで直接ベイクできます。[ベイク](../../baking/baking.md)を参照してください。

## ペイントAmbient occlusion

カスタムオクルージョンの詳細をペイントするには、Ambient occlusionチャンネルが必要です。 [テクスチャセット設定](../../interface/texture-set/texture-set-settings.md)で追加できます：

![](../../assets/add-ao-channel.png)

チャンネルがテクスチャセットに追加されると、任意のレイヤーを使用して新しい情報をペイントできます。 AOチャンネルにはグレースケール情報のみが含まれているため、推奨される描画モードは&#x200B;**通常** （ペイントオーバー）および&#x200B;**乗算** （結合）です。

描画モードとチャンネルごとに変更する方法の詳細については、[描画モード](../../interface/layer-stack/blending-modes.md)を参照してください。

## ambient occlusion上の追加マップのペイント

状況によっては、詳細を非表示にしたり、ベイクの問題を解決したりするために、ベイクされたAmbient occlusionの上にペイントを置くと便利です。

Substance 3D Painterのプロジェクトのデフォルト設定では、Ambient occlusion **チャンネル**&#x200B;が&#x200B;**追加のマップ**&#x200B;のAmbient occlusionのマップと組み合わされます。 つまり、既定では、ベイクされた追加マップをペイントすることはできません。各マップ（ベイク済みマップとチャンネル）の結果は合成されます。 この設定は次の設定で変更できます。

### 1 -Ambient occlusionチャンネルを追加する

現在のテクスチャセットにambient occlusionチャンネルを追加します。\
![](../../assets/edit-ao-channel-optimized.gif)

混合モードを「 **multiply** 」ではなく「 **replace** 」に設定します：\
![](../../assets/ao-mix-mode.gif)

### 2 -ベイクされたambient occlusionを使用した塗りつぶしレイヤーの設定

新しい塗りつぶしレイヤーを作成し、プロパティパネルを使用して、ベイクしたambient occlusionを「ambient occlusion」スロットに入れます。 まだ1に設定されていない場合は、塗りつぶしレイヤーのデフォルトのタイリングを忘れずに変更してください。\
![](../../assets/ao-stack.png)

### 3 - 塗りつぶしレイヤー描画モードの変更

デフォルトでは、新しいレイヤー上のAOチャンネルの描画モードは「 **乗算** 」に設定されています。 ビットマップにはアルファがないため、ベースとして塗りレイヤを使用することをお勧めするので、ここでは「通常」のブレンドモードを選択しました。これは、ビットマップにはアルファが存在せず、シェーダのデフォルトカラーを含めて、その下のすべてが置き換えられるためです。\
![](../../assets/ao-blend-mode.gif)

### 4 -ベイクしたambient occlusionマップ上にペイントするレイヤーを作成する

新規レイヤー（通常レイヤーまたは塗りつぶしレイヤー）を作成し、AOチャンネルの描画モードを「通常」に変更します。 この設定が完了すると、AOチャンネルにペイントされたオブジェクトは、下のレイヤにあるベイクされたAOマップを引き継ぎます。\
![](../../assets/paint-over-ao-optimized.gif)
