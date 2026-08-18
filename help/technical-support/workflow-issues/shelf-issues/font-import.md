---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/workflow-issues/shelf-issues/font-import.html"
breadcrumb-title: ''
description: Substance 3D Painterでフォントファイルの読み込みに関する問題を解決し、フォントリソースを正常に読み込んで使用する方法について説明します。
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: フォントファイルを読み込めません
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# フォントファイルを読み込めません

[テキストリソース](../../../painting/text-resource.md)の導入により、フォントファイルは起動時に自動的に収集されます。 フォントファイルは手動で読み込むこともできます。

この場合、いくつかのエラーメッセージが表示されます。

* Painterインターフェイスにファイルをドラッグ&amp;ドロップする場合。
* Painterがディスク上のフォントを検出したとき（ライブラリのクロール）。

## 問題の修正方法

<b>破損したファイル</b>に関するエラーメッセージが表示された場合は、代替バージョンを探すと、Painterで読み込むことができる場合があります。 <b>.ttf</b>および<b>.otf</b>形式のみがサポートされていることに注意してください。

<b>ライセンスの問題</b>に関するエラーメッセージが表示された場合、そのフォントはPainterと互換性がなく、インポートできません。

### メッセージの概要

|  |  |
| --- | --- |
| <b>エラーメッセージ</b> | <b>説明</b> |
| 「LIBRARYNAME」ライブラリに、4つのフォントファイル(FONTNAME、FONTNAME、FONTNAME)に影響する問題があります。 | このメッセージは、Painter内で読み込めないフォントファイルを特定し、その短いリストを収集します。 これらのファイルは無視され、アセットウィンドウに表示されません。 |
| フォントの問題が見つかりました。 詳細については、 https://を参照してください。 | フォントに関する問題が見つかったことを示す一般的なメッセージ。 |
| ライセンス制限のため、FONTNAMEを読み込めません。 詳細については、 https://を参照してください。 | フォントを使用するには、Painterがプロジェクトファイルにフォントを埋め込める必要があります。 そのため、（メタデータに指定されている）これを許可しないフォントは読み込むことができません。 |
| ファイルが破損しているか、サポートされていない種類のため、FONTNAMEをインポートできません。 詳細については、 https://を参照してください。 | Painterは指定されたフォントファイルを読み取れません。 |
