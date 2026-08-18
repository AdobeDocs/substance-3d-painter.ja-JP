---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterのシェーダー APIリファレンスにアクセスして、カスタムシェーダを作成し、レンダリング機能を拡張します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---


# シェーダー API

![](../../../assets/header-shader.jpg)

Substance Painterでは、シェーダを使用して、リアルタイムビューポートでマテリアルをレンダリングします。 カスタムシェーダを作成して、新しい動作を実装したり、ビューポートを他のレンダラーに一致させたりすることができます。

Substance Painter用のその他のシェーダーが[Substance share](https://share.allegorithmic.com/libraries?by_category_type_id=6)にあります。

>[!NOTE]
>
> シェーダー APIは、メニュー&#x200B;**ヘルプ/ドキュメント/シェーダー API**&#x200B;に移動して、アプリケーションから直接利用することもできます。

## シェーダリファレンス

## Changelog

* [完全な変更ログファイル](changelog-shader-api.md)

## ウォームアップ

Substance Painterでは、独自のシェーダを&#x200B;*GLSL*&#x200B;に書き込むことができます。 フラグメントシェーダーの&#x200B;*部分*&#x200B;のみを書き込むことができます。これは&#x200B;*サーフェスシェーダー*&#x200B;とも呼ばれます。 簡単に説明するために、「Hello world」Substance Painterサーフェスシェーダを使用してみましょう。

```
void shade(V2F inputs) { 

  diffuseShadingOutput(vec3(1.0, 0.0, 1.0)); 

}
```


このスニペットを&#x200B;*.glsl*&#x200B;ファイルに保存し、シェルフのシェーダタブにドロップしてSubstance Painterにロードすると、スニペットを使用して、メッシュ上で美しい均一なピンク色を確認できるようになりました。

## Surfaceシェーダ

* [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)

## エンジンが提供するデータ（または自分のチャネルにアクセスする方法）

Substance Painterでは、レンダリングエンジンパラメーター（ドキュメントのチャンネル、追加のテクスチャ、カメラ関連のデータなど）にアクセスできます。 以下は、エンジンが提供するすべてのパラメーターの完全なリストです。

* [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)

## エンジンの設定（またはレンダリング状態を指定する方法）

場合によっては、効果に特定のレンダリング設定（カリング、ブレンド、サンプリング局所性など）を使用することがあります。 一部のレンダリング状態が公開され、シェーダで設定できます。 公開されたすべてのレンダリング状態の包括的なリストを次に示します。

* [all-rendering-states-params.glsl](parameters-shader-api/all-rendering-states-params-shader-api.md)

## カスタムツイーク（またはシェーダをツイークする方法）

通常、シェーダにはカスタムツィークがあります。 これをSubstance Painterのシェーダで行うために、カスタムツィークを指定する方法を導入しました。 以下は、すべてのカスタムシェーダのツイークの種類の包括的なリストです。

* [all-custom-params.glsl](parameters-shader-api/all-custom-params-shader-api.md)

## 埋め込みライブラリ

すべてのシェーダに大量のボイラープレートコードを記述することを避けるために、便利な関数の小さくても実用的なライブラリを作成しました。 **現時点では編集したり、独自のデザインを作成したりすることはできません。**

* [lib-alpha.glsl](libraries-shader-api/lib-alpha-shader-api.md) ：不透明度に関連するヘルパーが含まれています
* [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md) :ベイヤーマトリックスヘルパーが含まれています
* [lib-defines.glsl](libraries-shader-api/lib-defines-shader-api.md) ：便利な数式の定数が含まれています
* [lib-emissive.glsl](libraries-shader-api/lib-emissive-shader-api.md) ：エミッシブプロパティヘルパーが含まれています
* [lib-env.glsl](libraries-shader-api/lib-env-shader-api.md) ：環境マップ関連のヘルパーが含まれています
* [lib-normal.glsl](libraries-shader-api/lib-normal-shader-api.md) ：法線マップ関連のヘルパー（およびHeightマップで生成された法線マップ）を含みます
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md) ：物理ベースのレンダリングヘルパーが含まれています
* [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) ：異方性物理ベースレンダリングヘルパーが含まれています
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) ：視差オクルージョンマッピングヘルパーが含まれています
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md) :ランダムなユーティリティが含まれています（不整合の低いシーケンス）
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md) :チャンネル取得ヘルパーが含まれています
* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) :セーフスパーステクスチャサンプリングヘルパーが含まれています
* [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) :サブサーフェススキャッタリングヘルパーが含まれています
* [lib-utils.glsl](libraries-shader-api/lib-utils-shader-api.md) :カラーユーティリティ関数（sRGB変換、トーンマッピング）が含まれています
* [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md) ：一般的なベクターを含むヘルパー

## メタデータ

レンダリングシステムにヒントを与えるために、不要な情報をさらに宣言できます。 シンタックスは次のとおりです。

```
//: metadata { 

//:   "key1":"value1", 

//:   "key2":"value2" 

//: }
```


サポートされているキー：

* **カスタムui**：標準シェーダーパラメーターのユーザーインターフェイスを、QMLモジュールとして記述されたカスタムビューに置き換えます（スクリプトのドキュメントを参照）。 パスは、シェルフ&#x200B;*custom-ui*&#x200B;フォルダーの1つに対する絶対または相対パスにできます。
* **mdl**:シェーダで使用するIray mdlマテリアルを定義します。 パスの構文は次のとおりです。 *mdl::folder1::folder2::mdl\_filename::material\_name*&#x200B;ここで、*folder1::folder2::mdl\_filename*&#x200B;はシェルフ&#x200B;*mdl*&#x200B;フォルダーの1つのmdlファイルへのパスで、*::material\_name*&#x200B;はこのmdlファイル内で宣言されたマテリアルの名前です。 （例： &quot;mdl&quot; : &quot;mdl::alg::materials::physically\_metallic\_roughness::physically\_metallic\_roughness&quot;）

## シェーダの例(yes, finally!)

実際のシェーダの外観を確認するために、複雑さを増して順序付けられたサンプルシェーダをいくつか紹介します。

* [pixelated.glsl](shaders-shader-api/pixelated-shader-api.md) :ピクセル化シェーダー
* [toon.glsl](shaders-shader-api/toon-shader-api.md) :トーンシェーダ
* [pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) : Substance Painterに埋め込まれたデフォルトのPBRシェーダ

## 動的マテリアルレイヤリング

この動的マテリアルレイヤリングは、シェーダ内でマテリアルを混ぜ合わせる特殊なワークフローであり、Substance Painterして描画マスクを動的に編集できます。 このワークフローを有効にするには、次の2つの新しい機能があります。

* シェーダ定義から編集可能なスタックを宣言します： [layering\_declare\_stacks.glsl](parameters-shader-api/layering-declare-stacks-shader-api.md)
* マテリアルをシェーダパラメータとしてバインド： [layering\_bind\_materials.glsl](parameters-shader-api/layering-bind-materials-shader-api.md)
