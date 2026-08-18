---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/photoshop-brush-presets-abr/importing-photoshop-brush-presets.html"
breadcrumb-title: ''
description: Photoshopのブラシプリセット（ABRファイル）をSubstance 3D Painterに読み込んで、ブラシライブラリを拡張する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Photoshop Brush Presets (ABR) > Importing Photoshop Brush Presets
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Photoshopブラシプリセットの読み込み
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---


# Photoshopブラシプリセットの読み込み

ここでは、ABRファイルをSubstance 3D Painterに読み込む手順を説明します。

1. <b>リソースのインポートウィンドウを開きます。</b>

   「生産資源のインポート」ウィンドウは、次の3つの異なる方法でオープンできます。

   * ABRファイルをアセットパネルにドラッグ&amp;ドロップします。
   * メインメニューの<b>ファイル/リソースのインポート</b>を使用します。
   * アセットパネルの<b>+ </b>ボタンを使用します。
1. <b>ABRファイルを[リソースのインポート]ウィンドウに追加します。</b>

   ABRファイルを「アセット」ウィンドウにドラッグ&amp;ドロップして読み込みウィンドウを開かなかった場合、デフォルトでは空の状態になります。

   ABRファイルを追加するには、次のいずれかを実行します。

   * ABRファイルをウィンドウに&#x200B;**ドラッグアンドドロップ**&#x200B;します。
   * **[リソースの追加]**&#x200B;ボタンをクリックし、ABRファイルを選択して読み込みます。

   >[!NOTE]
   >
   > ![](../../../assets/shelf-import-error.png)
   > 
   > ABRファイルに問題がある場合は、その横に警告アイコンが表示されます。 例：
   > 
   > * 互換性のあるプリセットが見つかりません。 詳細については、[Photoshopブラシパラメーターの互換性](photoshop-brush-parameters-compatibility.md)の一覧を参照してください。
   > * ファイルを読み取れません（破損しているなど）。
1. <b>ABRファイルのインポート方法を選択してください。</b>

   「生産資源のインポート」ウィンドウの下部で、ABRファイルのロード先を選択します。

   * <b>プロジェクト</b>: ABRファイルは、現在開いているプロジェクトに読み込まれます。 ブラシは、現在のプロジェクトが開いており、プロジェクトファイルに添付されている場合にのみ使用できます。
   * <b>セッション</b>: ABRファイルがメモリに読み込まれます。 ブラシプリセットは、アプリケーションが閉じられるまで使用できます。
   * <b>ライブラリ</b>: ABRファイルがディスク上のシェルフにコピーされます。 ブラシプリセットは、Painterを開くと常に、すべてのプロジェクトで使用できます。

   ![](../../../assets/import-location.png)
1. <b>シェルフからブラシプリセットにアクセスします。</b>

   ![](../../../assets/shelf-demo.png)

   ブラシプリセットの読み込みに問題がなかった場合は、[アセット](../../../interface/assets/assets.md)ウィンドウに表示されます。

   >[!NOTE]
   >
   > ブラシプリセットがビットマップに基づいている場合は、そのプリセットが使用するイメージを、ブラシプリセットと同じ名前のシェルフのAlphaセクションでも使用できます。
