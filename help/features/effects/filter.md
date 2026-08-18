---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/effects/filter.html"
breadcrumb-title: ''
description: Substance 3D Painterでフィルター効果を使用して、画像処理フィルターやテクスチャ補正を適用する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: フィルター
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# フィルター

フィルターエフェクトは、レイヤーまたはマスクの内容を変形する物質です。

## フィルターを適用するには？

フィルターの種類に応じて、レイヤーのコンテンツまたはマスクにフィルター効果を作成する必要があります。\
フィルターを適用するには2つの方法があります。どの方法を使用するかは、使用するフィルターの目的によって異なります。

## 手動でフィルタを適用する。

次の例ではぼかしフィルターがレイヤーのコンテンツに適用されていますが、一般的にはフィルターをマスクに適用するために使用されます。

### 1 – フィルター効果を追加する

まず、レイヤーのコンテンツを選択し（左のサムネール）、効果ボタンをクリックします（または右クリックでコンテキストメニューを開きます）。\
リストでオプション「 **フィルターを追加** 」を選択します。

![](../../assets/add-filter.gif)

### 2 – プロパティウィンドウでフィルターを選択します

プロパティウィンドウで、パラメーターまたはフィルターは現在空です。 選択ボタンのみが使用可能です。\
ボタンをクリックしてミニシェルフを開き、目的のフィルターを選択します。ここでは、ぼかしフィルターを選択します。

![](../../assets/filter-select-shelf.gif)

## シェルフからのフィルタのドラッグ&amp;ドロップ

このメソッドは、Layerstack全体に適用するフィルタのみを対象としています。 すべてのチャンネル[描画モード](../../interface/layer-stack/blending-modes.md)が自動的に設定されます。 マスクにフィルターを適用することはできません。

### 1 – シェルフのFilters領域を開きます。

シェルフで、左側にある「フィルタ」セクションをクリックします。

![](../../assets/shelf-filters.gif)

## 2 – フィルターをドラッグ&amp;ドロップ

シェルフで使用するフィルタを選択します。 レイヤースタックにドラッグ&amp;ドロップして、正しい場所に配置されていることを確認します（例えば、不要なグループにドロップすることは避けます）。

![](../../assets/filter-dragdrop.gif)

上記の例では、ドロップされたフィルターにパススルー描画モードが設定されていることに注意してください。 これは、ドキュメントのすべてのチャンネルに当てはまります。

## 新しいタイプのフィルターの追加

すべてのフィルターはSubstanceで、Substance 3D Designerを使用して作成できます。\
Substance 3D Designerを起動すると、Substance 3D Painterですぐに使用できるテンプレートが表示されます。

詳しくは、次のページを参照してください： [カスタムエフェクトの作成](../../content/creating-custom-effects/creating-custom-effects.md)
