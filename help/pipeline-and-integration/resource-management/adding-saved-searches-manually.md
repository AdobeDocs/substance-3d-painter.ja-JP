---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/pipeline-and-integration/resource-management/adding-saved-searches-manually.html"
breadcrumb-title: ''
description: Substance 3D Painterで保存済みの検索を手動で追加し、頻繁に使用するリソースフィルターにすばやくアクセスする方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding saved searches manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 保存された検索を手動で追加する
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 2%

---


# 保存された検索を手動で追加する

アセット検索クエリ（または保存された検索）は、設定ファイルを編集することで定義できます。 このページではその方法について説明します。

## 構成ファイルの場所

カスタム保存クエリを追加するには、ユーザーのドキュメントフォルダーに移動し、**Shelf.ini**&#x200B;ファイルを開きます。

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Platform</th> <th>バージョン</th> <th>パス</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong>以降</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">レガシー</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong>以降</td> <td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">レガシー</td> <td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong>以降</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>レガシー</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

## 例

設定ファイルに入れられる内容の例を以下に示します。

```
[filters] 

size=4 

1name=Grunge 

1query="u:basematerial=,smartmaterial=,smartmask=,texture=,procedural=,brush=,alpha= grunge" 

2name=Procedural 

2query="u:procedural=" 

3name=Environment 

3query="u:environment=" 

4name=Default Filters 

4query="p:/allegorithmic/^ u:filters="
```


次に、このシンタックスの機能を示します。

* **サイズ**:アプリケーションで読み取りおよび読み込みが必要なカスタムプリセットの数を決定します。
* **数値**：行の先頭には、現在のプリセットが定義されています（例： **1/**）。
* **クエリ**: （数字の後）実際に使用される検索語を定義します。 この例では、用途には&#x200B;**u:**&#x200B;を使用し、パスには&#x200B;**p:**&#x200B;を使用し、検索語には文字列を使用しています。 クエリコンテンツは引用符で囲む必要があります。 使用できる用語については、[このページを参照](../../interface/assets/advanced-search-queries.md)してください。
* **名前**:プリセットの名前。
