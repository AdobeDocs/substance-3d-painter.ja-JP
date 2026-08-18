---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/pipeline-and-integration/resource-management/excluding-resources-in-a-resource-path.html"
breadcrumb-title: ''
description: Substance 3D Painterのリソースパスから特定のリソースを除外して、シェルフの整理を改善する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Excluding resources in a resource path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: リソースパス内のリソースの除外
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---


# リソースパス内のリソースの除外

このページでは、[アセット](../../interface/assets/assets.md)ウィンドウのクロール処理中に無視されるリソースとフォルダーを指定するために、無視ファイルを設定する方法について説明します。 これにより、不要なリソースが表示されるのを防ぐことができます。

>[!NOTE]
>
> この機能はバージョン7.2.3以降で利用可能です。

## 無視するファイルの作成

リソースを非表示にするリソースフォルダーの場所に移動します。 次に、followという名前のファイルを作成します。

```
.ignore_assets_pt
```


>[!NOTE]
>
> ファイル名はドットで始まる必要があります。

作成後は、次のようになります。

![](../../assets/ignore-file-location.png)

## 例

次のファイルの内容は、デフォルトのライブラリフォルダー以外のリソースとフォルダーを破棄します。

```
## exclude all

* 

 

## re-include library directories

!alphas 

!colorluts 

!effects 

!emitters 

!environments 

!export-presets 

!generators 

!materials 

!presets 

!procedurals 

!receivers 

!shaders 

!smart-masks 

!smart-materials 

!templates 

!textures
```


## ルールとガイドライン

次の表に、ignoreファイルに適用される一般的なルールを示します。

>[!NOTE]
>
> ignoreファイルのパターンマッチングでは、オペレーティングシステムの動作とは別に、大文字と小文字が区別されます。

| ルール | 説明 | 例 |
| --- | --- | --- |
| **空白行** | 何にも一致しない空の行。 読みやすくするための区切りとして使用できます。 |  |
| **ディレクトリ区切り記号** | スラッシュはディレクトリの区切り文字として使用されます。 区切り文字は、検索パターンの先頭、中央、末尾に置くことができます。パターンの先頭または途中（あるいはその両方）に区切り文字がある場合、パターンは無視ファイル自体のディレクトリレベルに対する相対パスになります。 それ以外の場合、パターンは無視ファイルレベルより下の任意のレベルでも一致する可能性があります。 パターンの末尾に区切り文字がある場合は無視され、パターンはファイルとディレクトリの両方に一致します。 | `folder/filename.extension   folder/sub-folder` |
| **コメント行** | シャープ記号（またはハッシュ）で始まる行はコメントとして機能します。 | `# This is a comment` |
| **アスタリスク** | アスタリスクはスラッシュ以外の文字と一致します。 | `# Match anything starting with Alpha   alpha*   # Match any file with given extension   *.jpg` |
| **文字範囲** | 角かっこで括った文字の範囲を指定して、フォルダー名やファイル名と一致させることができます。<ul data-preserve-html="true"> <li data-preserve-html="true"><b>[abc]</b>：指定されたリストの1文字と一致します</li> <li data-preserve-html="true"><b>[a-c]</b>：指定された範囲内の1文字と一致します</li> <li data-preserve-html="true"><b>[ !abc]</b>：指定されたリストにない1文字と一致します</li> <li data-preserve-html="true"><b>[ !a-c]</b>：指定された範囲内にない1文字と一致します</li> </ul>範囲と一覧には、<b>[0-9]</b>の形式で数値を指定できます。 | `# Exclude any UDIM image in PNG   *_[0-9][0-9][0-9][0-9].png` |
| **エスケープ中の文字** | それ以外の場合は無視されるか、または規則として使用されるリテラル文字を示します。 | `# This is a comment   [#]This/Is/A/Path` |
| **末尾のスペース** | 末尾のスペースは、エスケープされない限り無視されます。 | `# Match a subfolder with trailing space   folder/subfolder[ ]` |
| **感嘆符のプレフィックス** | パターンの前に感嘆符(!)を付けると、パターンを否定できます。以前のパターンで除外されたファイルは、再び含まれるようになります。 ファイルの親ディレクトリが除外されている場合、そのファイルを再度含めることはできません。 クロールでは、パフォーマンス上の理由から除外されたディレクトリは一覧表示されないため、含まれているファイルのパターンは、定義されている場所に関係なく影響を受けません。 | `# Re-include specific file   !my_file_name.png` |
