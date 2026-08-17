---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management/color-management-with-adobe-ace-icc.html"
breadcrumb-title: ''
description: Substance 3D PainterでAdobe ACEとICCカラーマネジメントを使用して、一貫したカラーワークフローを実現する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with Adobe ACE - ICC
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Adobe ACEを使用したカラーマネジメント – ICC
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Adobe ACEを使用したカラーマネジメント – ICC

ICCプロファイルで画像を使用するAdobe Color Engine(ACE)に関連するカラーマネジメント設定について説明します。

## プロジェクト設定

![](../../assets/cm-ace.png)

プロジェクト設定は、[新規プロジェクト](../../getting-started/project-creation.md)ウィンドウを使用して、または[プロジェクト構成](../../interface/project-configuration.md)ウィンドウを使用して、新規プロジェクトを作成するときに設定できます。

>[!NOTE]
>
> 環境変数（以下を参照）またはプリセットファイルが読み込まれた場合、UIの設定は無効になります。

使用可能な設定は次のとおりです。

| セクション | 設定 | 説明 |
| --- | --- | --- |
| **構成** | **カラーマネジメント** | カラーの管理に使用するエンジンを定義します。有効な値：<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>従来</strong> （既定）：定義済みのsRGB/リニアsRGBガンマ色補正を使用します。</li> <li data-preserve-html="true"><strong>OpenColorIO</strong>: OCIO統合を使用します。</li> <li data-preserve-html="true"><strong>Adobe ACE</strong>: Adobe Color Engine、ICCプロファイルをサポートします。</li> </ul> |
|  | **プリセットファイルを使用する** | 有効な場合は、json構成ファイルを介してカラーマネジメント設定をアップロードすることを許可します。 |
|  | **プリセットファイル** | プリセットファイルへのJSON形式のパス。 詳しくは、以下を参照してください。 |
|  |  |  |
| **色の設定** | **作業用カラースペース** | アプリケーション内で作業するためにエンジンによって使用されるカラースペース。 テクスチャを変換（読み込み）または変換（書き出し）するカラースペースです。指定できる値は次のとおりです。<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>リニアsRGB IEC61966-2.1</strong> （既定）</li> <li data-preserve-html="true"><strong>ACEScg ACESワーキングスペースAMPAS S-2014-004</strong></li> <li data-preserve-html="true"><strong>リニアAdobe RGB (1998)</strong></li> </ul> |
|  | **マッチング方法** | カラースペース間の色の変換方法を指定します。有効な値：<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>知覚的</strong></li> <li data-preserve-html="true"><strong>彩度</strong> （既定）</li> <li data-preserve-html="true"><strong>相対色</strong></li> <li data-preserve-html="true"><strong>絶対色</strong></li> </ul> |
|  |  |  |
| **ビットマップの読み込みカラースペースの既定値** | **8ビット画像** | 8ビット画像ファイルを読み込むときにデフォルトで使用されるカラースペース。 |
|  | **16ビット画像** | 16ビットイメージファイルを読み込むときにデフォルトで使用するカラースペース。 |
|  | **浮動小数点の画像** | HDR/EXR画像ファイルを読み込むときにデフォルトで使用するカラースペース。 |
|  | **埋め込みICCプロファイルを使用（推奨）** | 有効になっている場合は、画像ファイルの設定に従ってICCプロファイルを使用してカラーを調整します。 |
|  |  |  |
| **Substanceの素材** | **マテリアルカラースペースの既定** | Substanceマテリアルのカラーマネジメント入出力に使用するカラースペースを定義します。 |
|  |  |  |
| **カラースペースの書き出し** | **8ビット画像** | 8 bit画像ファイルを書き出すときにデフォルトで使用されるカラースペース。 |
|  | **16ビット画像** | 16ビットイメージファイルの書き出し時にデフォルトで使用されるカラースペース。 |
|  | **浮動小数点の画像** | HDR/EXR画像ファイルを書き出すときにデフォルトで使用するカラースペース。 |

## プリセットファイルの使用

![](../../assets/cm-ace-env-var.png)

新規プロジェクトの作成時に、プリセットファイル（json形式）を使用してACE設定を制御できます。

### 環境変数

環境変数&#x200B;**PAINTER\_ACE\_CONFIG**&#x200B;を使用して、プリセットファイルのパスを指定できます。 存在する場合、アプリケーションは常にプリセットファイルを使用してカラーマネジメント設定を行います。 この設定はインターフェイスで無効になります。

詳細については、[環境変数](../../pipeline-and-integration/configuration/environment-variables.md)ページを参照してください。

### プリセットの例

プリセットファイルとして使用できるjsonファイルの例を次に示します。

```
{ 

  "color settings": { 

    "working color space": "Linear Adobe RGB (1998)", 

    "rendering intent": "Saturation" 

  }, 

  "bitmap import color space defaults" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw", 

    "use embedded ICC profiles when available": false 

  }, 

  "substance material": { 

    "material color space default": "image P3" 

  }, 

  "export colors spaces" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw" 

  } 

} 
```
