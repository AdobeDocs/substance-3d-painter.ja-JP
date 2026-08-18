---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/sparse-virtual-textures.html"
breadcrumb-title: ''
description: Substance 3D Painterで希薄なバーチャルテクスチャを使用して、超高解像度テクスチャを効率的に操作する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Sparse Virtual Textures
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: スパース仮想テクスチャ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# スパース仮想テクスチャ

![](../assets/svt-header.jpg)

Substance 3D Painterのバージョン&#x200B;**2018.3**&#x200B;以降、リアルタイムビューポートで&#x200B;**スパース仮想テクスチャ** (**SVT**)を使用して、大量のテクスチャを管理します。 このテクノロジーを使用すると、特定の視点からのみ必要なテクスチャをストリーミングして、GPUメモリ上の特定のフットプリントを維持することができます。 これにより、大量のテクスチャセット（またはUDIM）を使用するプロジェクトのパフォーマンスが向上します。

## サポート対象プラットフォーム

![](../assets/sparse-settings.png)

スパーステクスチャは、十分なパフォーマンスを得るために特定のハードウェア構成に依存します。 現在の構成が正しくサポートされていない場合、Substance 3D Painterは代わりに&#x200B;**フォールバック**&#x200B;をソフトウェアの実装に適用します（これは、精度が低く、パフォーマンスが低くなります）。

[設定](../interface/settings/settings.md)に移動すると、Substance 3D Painterでハードウェアアクセラレーションの代わりにソフトウェアフォールバックを強制的に使用できます。

ハードウェアアクセラレーション対応のスパース仮想テクスチャをサポートする構成は次のとおりです。

| Platform | サポート（ハードウェアアクセラレーション） | サポートなし（ソフトウェアフォールバック） |
| --- | --- | --- |
| **ウィンドウ** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce（ドライバー411.63以降）</li><li data-preserve-html="true">Nvidia Quadro（ドライバー411.63以降）</li><li data-preserve-html="true">AMD FireProおよびRadeon Pro （ドライバー18.9.3以降） <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon （ドライバー18.9.3以降）&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true"> Nvidia Quadro M2000 </li><li data-preserve-html="true">  Nvidia Geforce GTX 970 </li><li data-preserve-html="true"> Intel GPU </li></ul> |
| **Mac OS** | <ul data-preserve-html="true"><li data-preserve-html="true"> オペレーティングシステムでサポートされていないハードウェア機能 </li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">任意のGPUモデル</li></ul> |
| **Linux** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce（ドライバー410.73以降）</li><li data-preserve-html="true">Nvidia Quadro（ドライバー410.73以降）</li><li data-preserve-html="true">AMD FireProおよびRadeon Pro （ドライバー18.9.3以降） <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon （ドライバー18.9.3以降）&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Intel GPU</li></ul> |


* **\*** ：既定で無効になっているハードウェアアクセラレータは、[設定](../interface/settings/settings.md)で手動で有効にすることができます。

## Substance 3D Painterで疎な仮想テクスチャを使用するのはなぜですか？

Substance 3D Painterは、メインエンジンを使用してテクスチャを計算し、ビューポートに表示します。 つまり、エンジンとビューポートは、これらのテクスチャを計算および表示するためにGPUメモリ(VRam)を共有する必要があります。 プロジェクトに&#x200B;**テクスチャセット** （またはUVタイル）が多いほど、ビューポートに必要なメモリが多くなります。 ビューポートがGPUでメモリを消費しすぎると、メインエンジンにテクスチャを計算するための十分な容量がなく、テクスチャをシステムメモリ(Ram)に削除する必要があります。 これにより、パフォーマンスが低下し、計算速度が低下します。

SVTの目標は、ビューポートがGPUメモリで使用できる容量を割り当て、メインエンジンが計算を行うスペースをできる限り確保することです。 このシステムの利点は、通常どおり作業しながら、Substance 3D Painterにさらに大きなプロジェクトを読み込める機能が利用できることです。

## スパーステクスチャの機能について教えてください。

スパース仮想テクスチャは、完全ではないテクスチャの一種です。 つまり、アプリケーションはテクスチャの一部のみをメモリにロードします。 必要なもののみがロードされ、残りはシステムメモリまたはディスク（キャッシュ）に格納されます。 再び必要な場合、テクスチャはキャッシュから取得され、ビューポートに戻されます。 転送をすばやく行うには、システムは&#x200B;**mipmaps**&#x200B;を使用して、テクスチャの解像度の違いをすばやくジャンプします。 そのため、ビューポートにすばやく移動すると、最初はぼやけたテクスチャが表示され、数秒後に品質が向上することがあります。

技術的な知識については、 [スパースな仮想テクスチャ](https://silverspaceship.com/src/svt/)を参照してください。

## キャッシュの場所

![](../assets/settings-temp.png)

SVTキャッシュを保存するのに十分なシステムメモリ(Ram)がない場合、Substance 3D Painterはキャッシュを保存する代わりにコンピューターのハードドライブに切り替えます。\
このキャッシュの既定の場所は、オペレーティングシステムの一時ファイルフォルダーです。 この場所は、アプリケーションのメイン設定で変更できます。[一般環境設定](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/general-71008262.html)を参照してください。

## シェーダの互換性

SVTを最大限に活用するには、シェーダがSparseシステムにテクスチャを要求して読み取る必要があります。 そのため、**vec2テクスチャ座標**&#x200B;および&#x200B;**サンプラー**&#x200B;に基づく以前の関数は廃止されました。 Sparseテクスチャを使用する代わりに、ヘルパー関数が提供されるようになりました。

シェーダを更新するには：

* **既定のSubstance 3D Painterシェーダー**&#x200B;の場合： [シェーダーの更新](../interface/shader-settings/updating-a-shader.md)ページから順を追って手順を実行します。
* **カスタムシェーダー**&#x200B;の場合：ログおよび[シェーダー API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html)ページのエラーメッセージを確認します。

>[!WARNING]
>
> 古いプロジェクトのシェーダが最新でない場合は、白いフラッシュが表示されることがあります。 詳しくは、このページを参照してください。[カメラを移動すると、メッシュフラッシュが白くなります](../technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.md)。
