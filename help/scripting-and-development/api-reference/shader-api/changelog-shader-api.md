---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/changelog-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter シェーダー APIの更新ログを確認して、更新、新機能、変更を経時的に追跡します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Changelog - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Changelog - シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 3%

---


# Changelog - シェーダー API

## Changelog

## 2018.3.2

* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md):サンプリング関数は、単純なミップマップレベルではなくテクスチャ微分を使用します。 これは、異方性サンプリングをサポートするための要件です。 サンプリング関数のシグネチャは変更されません。
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): *getParallaxOffset*&#x200B;関数シグネチャが、テクスチャ微分を使用するために変更されました

## 2018.3.0

* 新しい[lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md)ライブラリを追加して、異方性Specularハイライトを視覚化します
* 新しい[lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md)ライブラリを追加して、mipmapsの可用性を考慮することでチャネルサンプリングを支援します
* この安全なサンプリングを処理するために、シェーダライブラリインターフェイスを更新します
* **廃止**: vec2テクスチャ座標およびテクスチャサンプラーに基づく以前の関数は廃止されました（新しい署名を使用してください）
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): *applyParallaxOffset*&#x200B;関数を追加して、パララックスオクルージョンエフェクトの使用を簡略化します
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md):ブルーノイズのランダム値ジェネレーターと時間的な代替文字を追加します
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md)：値の解釈とサンプリングヘルパーの両方を持つすべてのチャンネルサンプリングヘルパーを分割します

## 2018.2.0

* **サーフェスシェーダー APIの変更**: *shade*&#x200B;関数シグネチャが変更されました。[surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)を参照してください。
* *shadeShadow*&#x200B;関数はもう使用されておらず、カスタムサーフェスシェーダから安全に削除できます
* サブサーフェススキャタリングのサポートを追加します。詳細については、[surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)および[lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md)を参照してください。
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md): *pbrComputeBRDF*&#x200B;関数が削除されました。 ライブラリの使用方法については、[pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md)の例を参照してください
* 新しいエンジンパラメーターが追加されました： *texture\_blue\_noise*、*aspect\_ratio*、*camera\_vp\_matrix\_inverse*、*environment\_exposure*、*environment\_rotation*、*fovy*、*main\_light*&#x200B;および&#x200B;*screen\_size*。 詳細については、[all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)を参照してください
* *説明*&#x200B;メタデータを追加して、カスタムシェーダーパラメーターのツールヒントを提供します

## 2017.4.2

* ドキュメントのサンプルに含まれていないシェーダ（ピクセル化およびトーンシェーダ）の修正
* 高解像度のディザリングの修正
  * [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md): **bayerMatrix8()**&#x200B;は座標> 4kの有効な値を返します

## 2017.4.1

* pbrでコーティングされたシェーダを修正する
  * [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md): **tangentSpaceToWorldSpace()**&#x200B;および&#x200B;**worldSpaceToTangentSpace()**&#x200B;の出力が正規化されました

## 2017.4.0

* 特定のメッシュの2DビューでのSpecularのリフレクションが正しくない

## 2017.3.1

* より安価なディザリング

## 2017.2.0

* Substance Designerとベーカーのビヘイビアーに合わせて、補間されたtbn正規化を削除します
* [ビューポート] Hammersleyテーブルをフィボナッチスパイラルで置き換える

## 2.6.0

* シェーダのブレンドモードとカリングモードを修正する
* ディザリングを再実行します。 線形のレンダリングがある場合は、カラープロファイルの後に適用します

## 2.5.0

* ビューポートにカラープロファイル(LUT)のサポートを追加（オプションsRGB変換）
* シェーダの不透明度にディザリングを追加する
* パララックスオクルージョンマッピングをPBRシェーダに追加する
* デフォルトシェーダUIからカスタムパラメータを非表示にする方法を追加する
* レイヤシェーダドキュメントのチャンネルタグリストにリンクを追加する
* &#39;channel\_ao&#39;タグを&#39;channel\_ambientocclusion&#39;に置き換えます
* [ビューポート]一部の法線マップにはクランプされた値があり、アーティファクトとして表示されます
* Shadersドキュメントの使用可能なチャンネルを修正する
* カスタムシェーダUIの定義を許可
* マテリアルのレイヤシェーダ用に標準のカスタムシェーダUIを追加する
* シェルフ内のshaders/custom-uiフォルダ（mdlなど）に対して、カスタムUIファイルが検索されるようになりました
* デフォルトシェーダでSpecular levelチャンネルを使用する
* Fix vec3 shader paramsの例
* PainterをOpenGLコアプロファイルにアップグレード

## 2.4.0

* 書き出された結合された法線マップとビューポートに表示された法線マップの差を修正

## 2.2.0

* 非ドキュメントテクスチャ用の汎用マテリアルで、バインドレステクスチャのサポートが追加されました。
* カスタムシェーダースライダーのドキュメントの更新
* スライダーのステップの精度を定義できます
* 動的マテリアルレイヤリング用ドキュメント

## 2.1.1

* lib-utilsに&#39;RGB2Gray&#39;関数を追加する

## 2.1.0

* シェーダパラメータとマテリアル/マスクのグループを定義できます
* ドキュメントで不足しているチャンネルを追加(&#39;ao&#39;、&#39;diffuse&#39;、&#39;specularlevel&#39;)

## 2.0.4

* アルファ値が低いと、通常のアンパック機能が正しく機能しない
* カスタムシェーダのメッシュ頂点カラーの読み込みを許可
* [ビューポート]一部のコンピュータで拡張された環境マップ

## 2.0.0

* 法線/AOの追加マップを専用チャンネルで上書きできるようにします
* Height2Normal関数をSobelメソッドに変更します。
* シェーダごとにmdlを定義する可能性を追加する
* シェルフに新しいmdlフォルダを追加します。
* 拡散チャンネルプリセットおよびSpecular levelチャンネルプリセットの追加
* トーンマッピングに関するドキュメント更新
* 正射投影モードで反射を修正する
* 環境マップの特定の場所に表示される白い垂直のグリッチを修正しました
* テクスチャパラメーターに&#39;default\_color&#39;を定義できるようにします

## 1.7.0

* 外部テクスチャを（シェルフから）サンプリングできます。

## 1.6.0

* 上書きできるガンマ/トネマッピング関数を公開します
* 複数のテキストコードの表示

## 1.5.0

* シェーダエラーレポートに行番号とファイル名を追加する

## 1.4.1

* 近似の近いシェーダで行われる変換を除いて、すべてのsRGB変換はsRGB標準に従います
* Heightチャンネルから法線マップが間違ったカラースペースに変換される

## 1.4.0

* 周囲オクルージョンチャンネルを追加
* 通常エディションの新しいワークフローを追加
* テクスチャ関連の自動パラメーターに&#39;or&#39;式構文を追加します
* OSXでのIntel gpuのpbrシェーダーの修正

## 1.3.4

* フラグメントシェーダの従法線の補間を許可
* Mikkt接線空間を修正

## 1.3.3

* 負の光強度を生成する球面高調波の補正
* 露光量の計算が露光量（およびSubstance Designer量スライダーを固定）と異なる
* シャドウは100%の金属表面には表示しないでください

## 1.3.0

* シャドウ関数の追加
* 不透明度のサポートを追加（「alpha\_test」および「alpha\_blend」）

## 1.2.0

* 必要なopenGLステートをカスタムシェーダに設定する機能
* 反転したビットマップを修正
* 通常チャンネルのサポートを追加

## 1.0

* カスタムシェーダのサポートの追加
