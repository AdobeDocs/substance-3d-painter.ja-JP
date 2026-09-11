---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/channel-specific-filter.html"
breadcrumb-title: ''
description: Substance 3D Painterで個々のテクスチャチャンネルを処理するための、チャンネル固有のフィルターエフェクトを作成する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Channel specific filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: チャンネル固有のフィルター
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# チャンネル固有のフィルター

エフェクトは、特定のチャンネルに固有の場合があります。 この場合、特定のチャンネルに影響を与えるには、そのチャンネルを識別する入力と出力を作成する必要があります。 原則として、入力/出力構造は常に1:1の規則に従う必要があります。 特定のチャンネルを入力する場合は、同じチャンネルを出力する必要があります。

**ベースカラー**&#x200B;チャンネルのみに影響するフィルターの例：

![](../../assets/specific-filter-basecolor.png)

>[!NOTE]
>
> 一般的な設定（入出力ノード）と特定のチャンネル（ベースカラー/ベースカラー）を組み合わせることはできません。

## Alphaコンポーネントの管理

RGBAとして保存されたチャンネルは、アルファ（ベースカラーなど）をサポートします。 これらのチャンネルについては、アルファ入出力をSubstanceカラー出力に直接保存できます。 ただし、Substanceエンジンはグレースケール画像のAlphaをサポートしていないため、セカンダリマップを使用して管理する必要があります。 Substance グラフのチャンネルのアルファコンポーネントを取得するには、&#39;**channelname\_grayscale**&#39;という名前のAlphaの入力を作成します（例： **ベースカラー\_Alpha**、**ラフネス\_Alpha**）。\
このアルファコンポーネントを出力するには、同じ命名規則を使用して出力ノードを作成します。

>[!NOTE]
>
> チャンネルごとの特定の「**\_Alpha**」出力は、通常の&#x200B;**マテリアル**&#x200B;では機能しません。 マスク付きチャンネルを非表示にするには、次の命名規則に従って特定の出力を作成する必要があります。
> 
> * 識別子 : **チャンネル\_Alpha**
> * 使用方法： **チャンネル\_Alpha**

## 入出力の用途と識別子のリスト

>[!NOTE]
>
> 入力ノードで&#x200B;**使用**&#x200B;または&#x200B;**識別子**&#x200B;のいずれかを使用できます（使用が優先されます）。

| チャンネル名 | 使用状況 | 識別子/識別子Alpha |
| --- | --- | --- |
| *環境オクルージョン* | **アンビエントオクルージョン** | **アンビエントオクルージョン/アンビエントオクルージョン\_Alpha** |
| *異方性角度* | **異方性ピアングル** | **異方性角度/異方性角度\_Alpha** |
| *異方性レベル* | **異方性反射** | **異方性反射レベル/異方性反射レベル\_Alpha** |
| *基本色* | **ベースカラー** | **ベースカラー/ベースカラー\_Alpha** |
| *Blending mask* | **blendingmask** | **blendingmask / blendingmask\_Alpha** |
| *拡散* | **拡散** | **拡散/拡散\_Alpha** |
| *ディスプレイスメント* | **ディスプレイスメント** | **ディスプレイスメント/ディスプレイスメント\_Alpha** |
| *放射体* | **emissive** | **放射/放射\_Alpha** |
| *光沢* | **光沢** | **光沢度/光沢度\_Alpha** |
| *Height* | **Height** | **Height/Height\_Alpha** |
| *IOR* | **ior** | **ior / ior\_Alpha** |
| *メタリック* | **メタリック** | **メタリック/メタリック\_Alpha** |
| *標準* | **通常** | **通常/通常\_Alpha** |
| *不透明度* | **不透明度** | **不透明度/不透明度\_Alpha** |
| *リフレクション* | **リフレクション** | **リフレクション/リフレクション\_Alpha** |
| *粗さ* | **ラフネス** | **ラフネス/ラフネス\_Alpha** |
| *散布* | **散布** | **散布/散布\_Alpha** |
| *Specular* | **Specular** | **Specular / Specular\_Alpha** |
| *Specular level* | **specularlevel** | **specularLevel / specularLevel\_Alpha** |
| *Transmissive* | **transmissive** | **transmissive / transmissive\_Alpha** |
| *ユーザー0* | **ユーザー0** | **ユーザー0 /ユーザー0\_Alpha** |
| *ユーザー1* | **ユーザー1** | **user1 / user1\_Alpha** |
| *ユーザー2* | **ユーザー2** | **ユーザー2 /ユーザー2\_Alpha** |
| *ユーザー3* | **ユーザー3** | **ユーザー3 /ユーザー3\_Alpha** |
| *ユーザー4* | **ユーザー4** | **ユーザー4 /ユーザー4\_Alpha** |
| *ユーザー5* | **ユーザー5** | **ユーザー5/ユーザー5\_Alpha** |
| *ユーザー6* | **ユーザー6** | **ユーザー6 /ユーザー6\_Alpha** |
| *ユーザー7* | **ユーザー7** | **ユーザー7 /ユーザー7\_Alpha** |

## 例

![](../../assets/single-channel.png){width="650px"}

この例では、**ラフネス**&#x200B;チャンネルを上書きするために、グレースケールノードを介してBase colorアルファチャンネルが抽出されます。

![](../../assets/mix-channel.png){width="650px"}

この例では、**ラフネス**&#x200B;チャンネルが&#x200B;**Base color**&#x200B;に掛けられます。
