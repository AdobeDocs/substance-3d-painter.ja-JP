---
breadcrumb-title: ""
description: テキストファイルとして処理された、破損したSubstance 3D Painterプロジェクトファイルを復元する方法について説明します。
title: 破損したプロジェクトファイル
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%
---

# プロジェクトがテキストファイルとして処理されたため、破損しています

プロジェクトの読み込み時に、次のエラーが表示されることがあります。

```
[Hdf5Archive] Archive 'project.spp' appears to have been processed as a text file and is irremediably corrupted. 

[Project management] The selected project 'project.spp' isn't valid!
```


このエラーは、プロジェクトがSubstance 3D Painter以外で変更されているため、**正しく読み取ることができません** 。\
これは通常、バージョン管理ソフトウェア（**Perforce**&#x200B;など）がSubstance 3D Painterプロジェクト&#x200B;**をバイナリファイル**&#x200B;ではなくテキストファイルとして処理した場合に発生します。 唯一の解決策は、**sppファイルをバイナリ**&#x200B;として処理するように、バージョン管理ソフトウェアに新しいルール/例外を追加することです。 **Perforce**&#x200B;について詳しくは、専用ドキュメントを参照してください： <https://www.perforce.com/perforce/r16.1/manuals/cmdref/p4_typemap.html>
