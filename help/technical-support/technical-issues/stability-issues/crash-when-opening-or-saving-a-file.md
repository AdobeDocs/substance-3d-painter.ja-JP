---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-when-opening-or-saving-a-file.html"
breadcrumb-title: ''
description: プロジェクト管理を確実に行うために、ファイルを開いたり保存したりするときにSubstance 3D Painterがクラッシュする問題の解決方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash when opening or saving a file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ファイルを開くまたは保存するときにクラッシュする
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# ファイルを開くまたは保存するときにクラッシュする

ファイルダイアログを開くと、WindowsでSubstance 3D Painterがクラッシュする理由がいくつかあります。 このページでは、この問題の理由と解決策について説明します。

## ソフトウェアの競合

プログラムによっては、インストールやクラッシュの原因となる可能性のあるカスタムシェル拡張機能を追加できます。 詳細については、[ソフトウェアの競合](../startup-issues/software-conflicts.md)の一覧を参照してください。

## シェル拡張機能/カスタムテーマ

カスタムテーマはGUIフレームワークではサポートされていないため、Substance 3D Painterを使用する前に現在のテーマをアンインストールすることを強くお勧めします。

**Alienware** / **Dell**&#x200B;コンピュータは、Substance 3D Painterとの互換性がないことが知られている一部のシェル拡張機能をデフォルトで統合しています。 それらをアンインストールすることをお勧めします。 互換性がないすべての拡張機能が正確にはわかっていませんが、ほとんどの場合は次の機能に対応しています。

* DBROverlayIconBackuped.DBROverlayIconBackupedクラス
* DBROverlayIconNotBackuped.DBROverlayIconNotBackupedクラス

コンピューターにインストールされている拡張機能を確認するには、次のツールを使用します。 次に、処理の大まかな手順を示します。

1. NirSoftからShellExViewをダウンロードしてインストールします： <http://www.nirsoft.net/utils/shexview.html>
1. プログラムの実行
1. **オプション**&#x200B;をクリックして、**拡張機能の種類でフィルター**&#x200B;を選択します
1. **アイコンオーバーレイハンドラー**&#x200B;を選択
1. **エイリアンリスポーン**&#x200B;の2つのエントリが表示されます。
1. **両方**&#x200B;を選択し、赤いボタンをクリックして無効にします。
