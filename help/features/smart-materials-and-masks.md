---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/smart-materials-and-masks.html"
breadcrumb-title: ''
description: Substance 3D Painterでスマートマテリアルとマスクを使用して、ジオメトリに適応するプロシージャルテクスチャを作成する方法を説明します。
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

Substance 3D Painterでは、高度な&#x200B;**レイヤープリセット**&#x200B;の使用をサポートしています。 これらのプリセットを使用すると、異なる結果を維持しながら、**テクスチャセット間での**&#x200B;共有または&#x200B;**類似したテクスチャリングプロセス**&#x200B;をプロジェクトしたり、**メッシュトポロジに適合**&#x200B;したりできます。

>[!NOTE]
>
> レイヤースタックに追加されると、使用されたスマートマテリアルを取得する方法はありません。 スマートマテリアルを更新する必要がある場合は、手動で処理する必要があります。\
> ただし、[リソースアップデーター](plugins/resources-updater.md)を使用すると、個々のリソースを更新できます。

## スマートマテリアル/マスクの使用方法を教えてください。

スマートマテリアルはレイヤースタック内の任意の場所で使用できますが、スマートマスクはエフェクトスタックでのみ使用できます。\
違いについて詳しくは、[レイヤースタック](../interface/layer-stack/layer-stack.md)と[エフェクト](effects/effects.md)を参照してください

### スマートマテリアルの追加

スマートマテリアルは、次の2つの異なる方法で追加できます。

* シェルフからレイヤースタックにスマートマテリアルをドラッグ&amp;ドロップする方法：\
  ![](../assets/sm-drop.gif)
* スマートマテリアルボタンをクリックしてミニシェルフを開く：\
  ![](../assets/sm-button.gif)

### スマートマスクの追加

スマートマスクはエフェクトのプリセットなので、エフェクトスタック（特にマスクの場合）にのみ追加できます。

* スマートマスクを追加するには、**シェルフから1つを**&#x200B;ターゲット&#x200B;**レイヤーにドラッグ&amp;ドロップ**&#x200B;します。\
  ![](../assets/smm-drop.gif)
* **複数**&#x200B;のスマートマスクをドラッグ&amp;ドロップすると、累積されます。\
  ![](../assets/smm-drop-accum.gif)
* ただし、**CTRL**&#x200B;を押しながらドラッグ&amp;ドロップすると、効果スタック全体を&#x200B;**置き換え**&#x200B;できます。\
  ![](../assets/smm-drop-replace.gif)

### スマートマテリアル/マスクを作成するには？

スマートマテリアルを作成するには、**フォルダー**&#x200B;が必要です。\
スマートマテリアルのコンテンツはフォルダーに含まれます。 次に、フォルダーを右クリックして「 **スマートマテリアルを作成** 」を選択します。 スマートマテリアルは現在のシェルフに追加され、選択したフォルダに応じた名前が付けられます。

![](../assets/create-sm.png)

スマートマスクを作成するには、レイヤーの上で右クリックして、「**スマートマスクを作成**」を選択します。

![](../assets/create-smm.png)

## スマートマテリアル/マスクを共有/取得する方法を教えてください。

プリセットはディスクに&#x200B;**保存**&#x200B;されており、専用フォルダーから取得できます。\
**シェルフの場所**&#x200B;を見つけるには、「[ハードドライブへのコンテンツの追加](../content/importing-assets/adding-content-on-the-hard-drive.md)」を参照してください。

次に、誰でもSubstance 3D Painterシェルフにファイルを&#x200B;**読み込み**&#x200B;て、プリセットを使用することができます。
