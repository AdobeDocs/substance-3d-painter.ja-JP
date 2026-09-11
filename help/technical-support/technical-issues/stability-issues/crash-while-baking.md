---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: ベイク作業中にSubstance 3D Painterのクラッシュを修正し、信頼性の高いテクスチャベイクワークフローを実現する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ベイク処理中のクラッシュ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# ベイク処理中のクラッシュ

一部の構成では、ベイクプロセス中にSubstance 3D Painterがクラッシュする場合があります。 このページでは、既知の問題とその軽減方法のリストを再編成します。

## ベイクプレビューでクラッシュする

デフォルトでは、Substance 3D Painterはテクスチャのベイクの進行中ステータスをビューポートに表示します。 コンピューターによっては、この機能が不安定になる可能性があります。

無効にするには：

1. **編集/設定**&#x200B;を使用して、メイン設定を開きます
1. **一般**&#x200B;から、**ベイク処理オプション**&#x200B;という名前のセクションにスクロールダウンします。
1. オプション「**ライブプレビューのベイクプロセスを有効にする**」をオフまたは無効にします。

## GPU レイトレーシングとのクラッシュ

ドライバーが不安定な一部のGPUでは、ベイクプロセスがGPU レイトレーシング機能によるクラッシュの原因になる場合があります。

無効にするには：

1. **編集/設定**&#x200B;を使用して、メイン設定を開きます
1. **一般**&#x200B;から、**ベイク処理オプション**&#x200B;という名前のセクションにスクロールダウンします。
1. オプション&#x200B;**GPU レイトレーシングを有効にする**&#x200B;をオフまたは無効にします。

## Ryzen CPUとのクラッシュ

Ryzen CPUで実行されているコンピューター構成でベイク処理中にアプリケーションがクラッシュする場合があります。 通常、BIOSをアップデートすると問題が解決します。

これは、マルチスレッド計算に関連しています。 この問題を解決するために、多くのマザーボードのコンストラクタが新しいBIOSアップデートを発行しています。そのため、このアップデートの適用をお勧めします。 詳細については、マザーボードのマニュアルとコンストラクタのWebサイトを参照してください。

## 互換性のないAssbinファイル

既定では、ベイク時に、ハイポリメッシュが&#x200B;**\*.assbin**&#x200B;ファイルに前処理され、後で再ベイク処理が高速化されます。 まれに、これらのファイルが別のバージョンで生成されていると、アプリケーションがクラッシュになることがあります。 それらを単に削除すると、それらが再生成されるので、問題を解決する必要があります。
