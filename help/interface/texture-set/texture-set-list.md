---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/interface/texture-set/texture-set-list.html"
breadcrumb-title: ''
description: Substance 3D Painterでテクスチャセットリストを使用して、プロジェクトの複数のテクスチャセットを管理および整理する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set list
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: テクスチャセット一覧
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---


# テクスチャセット一覧

![](../../assets/texture-set-list.png)

**テクスチャセットリスト**&#x200B;ウィンドウには、プロジェクト内の現在の3Dモデルのすべてのマテリアル IDが表示されます。 これにより、モデル上の各マテリアルに関連付けられたレイヤースタックとその専用の設定を切り替えて確認できます。

「テクスチャセットリスト」ウィンドウの主な目的は、マテリアル間を切り替えて、各マテリアルに関連付けられたレイヤースタックにアクセスできるようにすることです。\
[マテリアルレイヤー](../../features/dynamic-material-layering.md)のワークフローの場合、**サブスタック**&#x200B;はテクスチャセット名の&#x200B;**下**&#x200B;に表示されます。

>[!WARNING]
>
> 一度に編集/ペイントできるテクスチャセットは1つだけです。

## テクスチャセットステータス

テクスチャセットには複数のステートが可能です。

![](../../assets/txtset-status.png)

* **選択済み** ：現在のテクスチャセットは現在編集中です。 テクスチャセットを選択すると、[レイヤースタック](../layer-stack/layer-stack.md)と[シェーダー設定](../shader-settings/shader-settings.md)のウィンドウが更新されます。
* **表示/非表示** ：詳細については、以下の表示/非表示のセクションを参照してください。
* **無効** :テクスチャセットおよび関連するレイヤースタックをメッシュ上のマテリアルに添付できないことを示します。 詳細については、[テクスチャセットの再割り当て](texture-set-reassignment.md)を参照してください。

## 表示

![](../../assets/texturesetlist.png)

テクスチャセットの表示は、専用のアイコンで管理できます。

| *アイコン* | *アクション* | *説明* |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-menu.png"/></div> | メニューを開く | 次のアクションを使用して新しいメニューを開きます。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>すべて表示</strong>: ビューポート内のすべてのテクスチャセットを表示します。</li><li data-preserve-html="true"><strong>すべて非表示</strong> : ビューポート内のすべてのテクスチャセットを非表示にします。</li><li data-preserve-html="true"><strong>表示/非表示を反転</strong>：表示されているテクスチャセットは非表示になり、非表示のテクスチャセットは表示されます。</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-isolate.png"/></div> | フォーカスモード | 現在アクティブなテクスチャセットを分離し、このモードがアクティブである間は他のすべてのモードを非表示にします。 このボタンをもう一度クリックして、モードを終了します。 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-visible.png"/></div> | 表示 | テクスチャセットの横にあるこのボタンをクリックして、ビューポート内のテクスチャセットを非表示または表示します。 |

>[!NOTE]
>
> 既定では、**ペイント**&#x200B;の際に、選択されているテクスチャセットのみが表示されます。 「**ペイント時に選択したマテリアルのみを表示**」のチェックボックスをオフにすると、[環境設定](../settings/settings.md)でこの動作を変更できます。\
> 注意： **パフォーマンスの向上**&#x200B;のためにペイントしている間、他のテクスチャセットを非表示にしてください。

## コンテキストメニュー

![](../../assets/txtset-list-contextualmenu.png)

テクスチャセット名を右クリックするとコンテキストメニューが開き、次のアクションが表示されます。

* **テクスチャセットを表示/非表示** :テクスチャセットの表示/非表示を切り替えます（前のセクションを参照）
* **名前を編集** :テクスチャセットーの名前を変更できます。 この名前は、テクスチャの書き出しプロセスでも使用されます。 テクスチャセット名をダブルクリックして名前を変更することもできます。
* **名前を\*元の名前\***にリセット:メッシュ マテリアルが変更されている場合は、元のテクスチャセット名を復元します。
* **説明の編集** :テクスチャセットに関連付けられた説明を追加または変更できます。

## シェーダー管理

各テクスチャセット名の右側にあるボタンを使用して、シェーダー割り当てを管理できます。\
デフォルトでは、各テクスチャセットは同じシェーダーインスタンスを共有します。 ただし、メッシュの特定の部分に対してのみ異なるシェーダーを持つことが便利な場合があります。 この操作を実行するには、ボタンをクリックして「**新しいシェーダーインスタンス**」を選択します。 その後、[[シェーダーの設定](../shader-settings/shader-settings.md)]ウィンドウで、他のテクスチャセットに影響を与えることなく、シェーダーとそのパラメーターを変更できます。

![](../../assets/capture-d-e-cran-2018-07-12-a-15-45-32.png){width="500px"}

## 設定

「設定」ボタンをクリックすると、複数のアクションを表示する新しいメニューが開きます。

* **空の説明を非表示** （既定） ：空の場合は説明フィールドを非表示にします
* **説明をすべて非表示** ：空でない場合でも、説明フィールドを非表示にします
* **説明をすべて表示** ：空の場合でも、説明フィールドを表示します
* **シェーダーパラメーターのインポート** :JSONファイルをインポートして、テクスチャセットのシェーダーパラメーターを構成できるようにします
* **テクスチャセットの再割り当て** ：詳細については、[テクスチャセットの再割り当て](texture-set-reassignment.md)を参照してください。
