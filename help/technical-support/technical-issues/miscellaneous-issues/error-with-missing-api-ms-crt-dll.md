---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/error-with-missing-api-ms-crt-dll.html"
breadcrumb-title: ''
description: Windowsランタイムライブラリを適切にサポートするために、Substance 3D Painterでapi-ms-crt DLLが見つからないエラーを修正する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Error with missing api-ms-crt dll
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: api-ms-crt dllが見つからないエラー
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# api-ms-crt dllが見つからないエラー

お使いのコンピューターに&#x200B;**api-ms-win-crt-runtime-l1-1-0.dll**&#x200B;がないため、Substance 3D Painterを開始できません。\
これは、Visual Studio 2015の&#x200B;**Visual C++再頒布可能パッケージ**&#x200B;の一部である更新プログラムKB2999226のインストールに失敗したことが原因である可能性があります。

## 問題の修正方法

### 1 - Windowsが最新であることを確認する

1. [スタート]メニューを開く
1. コントロールパネルを選択
1. **Windows Update**&#x200B;をクリックします
1. **[更新プログラムの確認]**&#x200B;をクリックします
1. 利用可能なすべての更新プログラムを&#x200B;**インストール**&#x200B;します。
1. 更新プログラムのインストールが完了したら、コンピューターを&#x200B;**再起動**&#x200B;します。

再起動後、利用可能なアップデートがなくなるまで上記の手順を繰り返します。

### 2 - Visual C++再頒布可能パッケージのインストール

1. Visual C++再頒布可能パッケージをダウンロードします。
   1. [Windows 64ビット](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x64.exe)の場合
   1. [Windows 32ビット](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x86.exe)の場合
1. **vcredist\_x64.exe** （64ビット）または&#x200B;**vcredist\_x86.exe** （32ビット）を実行します
1. 「アンインストール」を選択し、手順に従います
1. 実行可能ファイルを再実行する
1. 「インストール」を選択します
