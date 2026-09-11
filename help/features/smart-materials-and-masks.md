---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/smart-materials-and-masks.html"
breadcrumb-title: ''
description: Substance 3D Painterでスマートマテリアルとマスクを使用して、ジオメトリに適応するプロシージャルのテクスチャを作成する方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Smart Materials and Masks
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: スマートマテリアルとマスク
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# スマートマテリアルとマスク

Substance 3D Painterでは、高度な&#x200B;**レイヤープリセット**&#x200B;の使用をサポートしています。 これらのプリセットを使用すると、結果の違いを維持しながら、**テクスチャセット間での共有**&#x200B;やプロジェクト間での共有&#x200B;**類似のテクスチャリングプロセス**、メッシュトポロジへの適合&#x200B;**を迅速に行うことができます。**

>[!NOTE]
>
> レイヤースタックに追加されると、使用されたスマートマテリアルを取得する手段がないことに注意してください。 スマートマテリアルを更新する必要がある場合は、プロセスを手動で実行する必要があります。\
> ただし、[リソースアップデーター](plugins/resources-updater.md)を使用すると、個々のリソースを更新できます。

## スマートマテリアル/マスクの使用方法を教えてください。

スマートマテリアルはレイヤースタック内の任意の場所で使用できますが、スマートマスクはエフェクトスタックでのみ使用できます。\
違いについて詳しくは、[レイヤースタック](../interface/layer-stack/layer-stack.md)と[効果](effects/effects.md)を参照してください

### スマートマテリアルの追加

スマートマテリアルを追加するには2つの方法があります。

* シェルフからレイヤースタックにスマートマテリアルをドラッグ&amp;ドロップする方法：\
  ![](../assets/sm-drop.gif)
* スマートマテリアルボタンをクリックしてミニシェルフを開く：\
  ![](../assets/sm-button.gif)

### スマートマスクの追加

スマートマスクはエフェクトのプリセットなので、（マスク専用の）エフェクトスタックにのみ追加できます。

* スマートマスクを追加するには、シェルフから&#x200B;**ターゲット**&#x200B;レイヤーに&#x200B;**ドラッグ&amp;ドロップ**&#x200B;します。\
  ![](../assets/smm-drop.gif)
* **複数**&#x200B;個のスマートマスクをドラッグアンドドロップすると、累積されます：\
  ![](../assets/smm-drop-accum.gif)
* ただし、**CTRL**&#x200B;を押しながらドラッグ&amp;ドロップすると、効果スタック全体を&#x200B;**置き換え**&#x200B;できます。\
  ![](../assets/smm-drop-replace.gif)

### スマートマテリアルやマスクを作成するにはどうすればよいですか？

スマートマテリアルーを作成するには、**フォルダー**&#x200B;が必要です。\
スマートマテリアルの内容はフォルダーに格納されます。 次に、スマートマテリアルーを右クリックして「 **フォルダーを作成** 」を選択します。 スマートマテリアルは現在のフォルダーに追加され、選択したシェルフーに応じた名前が付けられます。

![](../assets/create-sm.png)

スマートマスクを作成するには、レイヤーの上で右クリックして、「**スマートマスクを作成**」を選択します。

![](../assets/create-smm.png)

## スマートマテリアル/マスクを共有/取得する方法を教えてください。

プリセットはディスクに&#x200B;**保存**&#x200B;されており、専用フォルダーから取得できます。\
**シェルフーの場所**&#x200B;を見つけるには、「[ハードドライブにコンテンツを追加する](../content/importing-assets/adding-content-on-the-hard-drive.md)」を参照してください。

次に、誰でも簡単にファイルをSubstance 3D Painter シェルフに&#x200B;**読み込み**&#x200B;して、プリセットを使用できます。
