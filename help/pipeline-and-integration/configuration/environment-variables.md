---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/pipeline-and-integration/configuration/environment-variables.html"
breadcrumb-title: ''
description: Substance 3D Painterで環境変数を使用して、アプリケーションのビヘイビアーとパイプラインの統合を設定する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Environment variables
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 環境変数
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 3%

---


# 環境変数

このページには、アプリケーションのデフォルトの動作を上書きするために使用できる環境変数が一覧表示されます。

| 変数 | 説明 | バージョン |
| --- | --- | --- |
| **SUBSTANCE\_PAINTER\_ライセンス** | 値：ライセンスファイル自体への直接パス。ライセンスファイルの既定の場所を上書きできるようにします。 例：ライセンスファイルが&#x200B;**H:/allegorithmic/licenses/substance\_painter.key**&#x200B;にある場合、変数データは&#x200B;**&quot;H:/allegorithmic/licenses/substance\_painter.key&quot;**&#x200B;である必要があります。  **注意：** 3.x (2017.x)より前のバージョンの場合は、SUBSTANCE\_PAINTER\_2\_LICENSEを使用してください。 | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALLEGO\_LICENSE\_IDLE\_DELAY** | 値： 7200マルチユーザー構成の場合、ライセンスシートをリリースするまでの時間（秒単位）を指定します。 デフォルトは2時間（7200秒）です。 | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_SKIP\_CHECK\_FOR\_UPDATES** | 値：0または1（1 =更新チェックを無効にする）アプリケーションの起動時に更新チェックをスキップします。 新機能パネルを無効にします。 | <ol data-preserve-html="true"><li data-preserve-html="true">2.2</li></ol> |
| **SUBSTANCE\_PAINTER\_SVT\_HARDWARE\_ACCELERATION** | 値： 0または1（1 =有効）GPUの疎機能を使用します。 GPUまたはオペレーティングシステムでサポートされていない場合、設定は無視されます。 互換性のあるハードウェア構成については、次のドキュメントを参照してください： [スパース仮想テクスチャ](../../features/sparse-virtual-textures.md)この変数は、[設定](../../interface/settings/settings.md)ウィンドウで使用できるパラメーターを上書きします。 | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_TEMP\_LOCATION** | 値： Substance Painterが一時ファイル（SVTキャッシュを含む）を書き込む場所を定義します。この変数は、[Settings](../../interface/settings/settings.md)ウィンドウで使用できるパラメーターを上書きします。 | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_PREVIEWS\_MEMORY\_BUDGET** | 値： 500アプリケーションが「アセット」ウィンドウからプレビューを読み込んだり一時的に保存したりするために使用できるメモリ(Ram)の容量を定義します。 予算の上限に達すると、古いプレビューがアンロードされます。 この値は、アセットウィンドウでのプレビューの表示のみを制御します。値はメガバイト単位で定義されます。 デフォルト値は500 MBです。 | <ol data-preserve-html="true"><li data-preserve-html="true">2</li></ol> |
| **SUBSTANCE\_PAINTER\_PLUGINS\_PATH** | 追加のPythonプラグインの場所。 | 6.1 |
| **PYTHONPATH** | アプリケーションのPython統合と共にロードする追加のPythonモジュール。 詳細については、[外部Pythonモジュールの読み込み](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/loading-external-python-modules-205363420.html)を参照してください。 | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **OCIO** | OpenColorIOで[カラーマネジメント](../../features/color-management/color-management.md)設定を駆動するために使用される&#x200B;**config.ocio**&#x200B;ファイルへのパスです。  **注意：**&#x200B;この環境変数は、**PAINTER\_ACE\_CONFIG**&#x200B;変数よりも優先されます。 | <ol data-preserve-html="true"><li data-preserve-html="true">4</li></ol> |
| **PAINTER\_ACE\_CONFIG** | Adobe ACEで[カラーマネジメント](../../features/color-management/color-management.md)設定を駆動するために使用されるJSONファイルへのパスです。 | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES** | アプリケーション内のいくつかの機能を無効にします。<ul data-preserve-html="true"><li data-preserve-html="true">外部リソース（ヘルプ、webページ、サンプルなど）へのリンク</li><li data-preserve-html="true">更新プログラムのチェックを無効にする</li><li data-preserve-html="true">使用統計の送信を無効にする</li><li data-preserve-html="true">substance shareへの書き出しを無効にする</li><li data-preserve-html="true">ようこそパネルと新機能パネルを無効にする</li></ul> | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_DEBUG\_FPS** | ビューポート内に、ビューポートによってレンダリングされる1秒あたりのフレーム数のカウンタを表示します。 | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_PAINTER\_VRAM\_BUDGET** | Painterで使用可能なGPUメモリの量を指定します。 これは、グローバル予算をMB単位で定義します。 例えば、4 GBの制限を定義するには、値4000を使用します。コマンドライン引数を使用して、同じアクションを実行することもできます。 [コマンドライン](command-lines.md)を参照してください。 | <ol data-preserve-html="true"><li data-preserve-html="true">2.1</li></ol> |
