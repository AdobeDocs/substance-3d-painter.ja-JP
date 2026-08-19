---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/home.html"
breadcrumb-title: ''
description: Substance 3D Painterを使い始めて、テクスチャを3Dモデルに直接ペイントし、リアルなマテリアルサーフェスを作成しましょう。
helpx_creative_field: ""
helpx_description: Painter > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 9%

---


# Substance 3D Painter

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

Substance 3D Painterは、3Dメッシュにテクスチャを適用してレンダリングできる3Dペイントソフトウェアです。

このドキュメントは、このソフトウェアの基本的な使用方法から高度なテクニックまで学習できるように設計されています。

このマニュアルで回答されていない質問がある場合は、[フォーラム](https://community.adobe.com/t5/substance-3d-painter/bd-p/substance-3d-painter)で自由に質問してください。 PBR の詳細については、[物理ベースレンダリングガイド](https://helpx.adobe.com/jp/substance-3d/unlisted/tutorials.html)をダウンロードすることもできます。

</td>
<td width="58.30%" style="border: 0;" valign="top">

![](assets/2021.jpg){width="600px"}

</td>
</tr>
</table>

## はじめに

* [ライセンス認証とライセンス](getting-started/activation-and-licenses.md) – このページには、ライセンスの認証と管理の方法に関する情報が表示されるので、Painterの使用を開始できます。
* [必要システム構成](getting-started/system-requirements.md) – このページでは、必要システム構成とハードウェア互換性情報を再編成します。
* [プロジェクトの作成](getting-started/project-creation.md) – 新しいプロジェクト作成ウィンドウでは、3Dモデルとそのテクスチャリング情報を保存するプロジェクトファイルを作成できます。
* [書き出し](export/export.md) – プロジェクトをビットマップテクスチャに書き出して、他のソフトウェアで使用できます。 3Dモデルのジオメトリをエクスポートすることもできます。
* [用語集](getting-started/glossary.md) – このページには、アプリケーションで使用される最も一般的なキーワードと、その概念に関する簡単な説明が一覧表示されます。
* [パフォーマンス](technical-support/performances-guidelines/performances-guidelines.md) – このページでは、パフォーマンスを最大化し、物事をスムーズに実行する方法に関するヒントとコツを再編成します。

### インターフェイス

* [アセット](interface/assets/assets.md)
* [カラーピッカー](interface/color-picker.md)
* [表示設定](interface/display-settings/display-settings.md)
* [ヒストリー](interface/history.md)
* [レイヤースタック](interface/layer-stack/layer-stack.md)
* [メインメニュー](interface/main-menu/main-menu.md)
* [プロジェクト設定](interface/project-configuration.md)
* [プロパティ](interface/properties.md)
* [設定](interface/settings/settings.md)
* [シェーダー設定](interface/shader-settings/shader-settings.md)
* [テクスチャセット](interface/texture-set/texture-set.md)
* [ツールバー](interface/toolbars.md)
* [ビューポート](interface/viewport/viewport.md)

### ペイントツール

* [ツールリスト](painting/tool-list/tool-list.md) – このページでは、使用可能なすべてのペイントツールとその使用方法について説明します。
* [直線](painting/straight-line.md) – 直線を使用すると、クリック数が少なく、より正確に任意のペイントツールで簡単に線を描画できます。
* [怠惰なマウス](painting/lazy-mouse.md) – 怠惰なマウスは、マウスカーソルと実際のペイントとの間の距離オフセットであり、より正確で滑らかなストロークをペイントできます。
* [対称](painting/symmetry/symmetry.md) – 対称とは、幾何拘束に基づいて複数の場所を同時にペイントするアクションです。
* [塗りつぶし投影法](painting/fill-projections/fill-projections.md) – 塗りつぶしレイヤーおよび塗りつぶし効果は、特定のモードに基づいてメッシュに直接テクスチャを投影します。 このタイプのレイヤー/効果では、3Dモデルにテクスチャを手動でペイントする必要がありません。 プロジェクションの設定は、 Propertiesウィンドウで編集できます。
* [プリセット](painting/presets/presets.md) – プリセットは、ペイントツールの保存された設定です。 このページでは、それらの使用方法とその理由について説明します。
* [動的ストローク](painting/dynamic-strokes/dynamic-strokes.md) — 動的ストロークは、ブラシストローク内のスタンプごとに変わるSubstanceファイルを利用した通常のブラシストロークです。
* [高度なチャンネルペイント](painting/advanced-channel-painting/advanced-channel-painting.md) – シェーダで使用されている一部のデフォルトチャンネルをペイントして、高度なエフェクトや複雑なエフェクトを作成できます。 たとえば、ペイントHeight情報を通常のマップに変換します。

### ベイク処理

* [メッシュマップをベイクする方法](baking/how-to-bake-mesh-maps.md)
* [ベイク処理ビジュアライゼーション設定](baking/baking-visualization-settings.md)

### コンテンツ

* [カスタムエフェクトの作成](content/creating-custom-effects/creating-custom-effects.md)
* [アセットの読み込み](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/adding-content-to-the-shelf-142213317.html)

### 機能

* [UVの自動アンラップ](features/automatic-uv-unwrapping.md)
* [エフェクト](features/effects/effects.md)
* [物理サイズ](features/physical-size.md)
* [スマートマテリアルとマスク](features/smart-materials-and-masks.md)
* [表面下散乱](features/subsurface-scattering/subsurface-scattering.md)
* [動的マテリアルレイヤリング](features/dynamic-material-layering.md)
* [UV再投影](features/uv-reprojection.md)
* [UV タイル](features/uv-tiles/uv-tiles.md)
* [カラーマネジメント](features/color-management/color-management.md)
* [後処理](features/post-processing/post-processing.md)
* [Rayレンダラー](features/iray-renderer/iray-renderer.md)
* [プラグイン](features/plugins/plugins.md)
* [スパース仮想テクスチャ](features/sparse-virtual-textures.md)
* [カスタムシェーダ](features/custom-shaders.md)
* [SpaceMouse® by 3Dconnection](features/spacemouse-by-3dconnexion.md)
* [Universal Scene Description（米ドル）](features/universal-scene-description-usd.md)

### パイプラインと統合

* [インストールと環境設定](pipeline-and-integration/installation-and-pre/preferences-and-application-data-location.md)
* [構成](pipeline-and-integration/configuration/command-lines.md)
* [リソース管理](pipeline-and-integration/resource-management/adding-resource-paths-edi/adding-resource-paths-by-editing-preferences-manually.md)

### スクリプト作成と開発

* [スクリプトとプラグイン](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/script-and-plugins-197427392.html)

### テクニカルサポート

* [パフォーマンスに関するガイドライン](technical-support/performances-guidelines/performances-guidelines.md)
* [ペンとタブレットの設定](technical-support/configuring-pens-and-tablets.md)
* [ログファイルをエクスポートしています](technical-support/exporting-the-log-file.md)
* [DXDiagを書き出す](technical-support/exporting-a-dxdiag.md)

### リリースノート

* [すべての変更](release-notes/all-changes.md)
* [バージョン11.1](release-notes/version-11-1.md)
* [バージョン11.0](release-notes/version-11-0.md)
* [バージョン10.1](release-notes/version-10-1.md)

