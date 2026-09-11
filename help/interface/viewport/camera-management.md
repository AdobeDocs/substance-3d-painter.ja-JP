---
helpx_url: 'https://helpx.adobe.com/jp/substance-3d-painter/interface/viewport/camera-management.html'
breadcrumb-title: ''
description: Substance 3D Painter ビューポートでカメラビューを管理し、3Dモデルを効率的に移動およびフレームする方法について説明します。
helpx_creative_field: ''
helpx_description: Painter > Interface > Viewport > Camera management
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: カメラ管理
user-guide-description: ''
user-guide-title: ''
source-git-commit: e370ba212d3e90f71e09b75ff41be6123d37c5eb
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---


# カメラ管理

Maya、Max、Blender、Modo、DAEで作成されたカメラは、Substance 3D Painterに読み込むことができます。

>[!NOTE]
>
> ABC(Alembic)フォーマットでは、カメラと表示比率が正しくサポートされていません。

## Substance 3D Painterでのカメラの読み込み

カメラは、FBXまたはABC(Alembic)フォーマットのいずれかでメッシュファイルに含める必要があります。

名前、変形パラメーター、視野、縦横比（存在する場合）が読み込まれます。

新規プロジェクトウィンドウで、カメラを含むメッシュファイルを選択し、「**カメラを読み込み**」チェックボックスがオンになっていることを確認します。 **編集/プロジェクトメッシュウィンドウ**&#x200B;で&#x200B;**設定の再読み込み**&#x200B;をオンにすると、最初のプロジェクト作成時にカメラが見つからなかった場合に&#x200B;**設定の読み込み**&#x200B;をオンにすることもできます。

次に、[**OK**]をクリックします：

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/New-project-window-full.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/project-configuration-full.png" alt=""/></td>
  </tr>
</table>

## カメラを選択

現在のプロジェクトにカメラが読み込まれたら、**3D ビューポート**&#x200B;の&#x200B;**ドロップダウン**&#x200B;から、アクティブなカメラを選択できます。

デフォルトでは、「デフォルトカメラ」という名前のPainter カメラが選択され、遠近法モードになっています。

![](../../assets/camera-select.png)

上記の例では、3つのカメラが読み込まれ、デフォルトカメラが含まれている場合、ドロップダウンに合計4つのカメラが表示されます。

## カメラを制御する

読み込んだカメラが選択されている場合、ビューポート内でパン、ズーム、回転してカメラを動かすと、デフォルトカメラに切り替わります。 これにより、読み込まれたカメラがシーン内で移動するのを防ぐことができます。

>[!NOTE]
>
> 読み込んだカメラの順番を変更する必要がある場合は、選択したシーン編集アプリケーションで順番を更新し、**編集/プロジェクトシーン**&#x200B;で構成を再度読み込みます。

**ディスプレイ設定ウィンドウ**&#x200B;で、インポートされたカメラのパラメーターを制御できます。

![](../../assets/display-settings-cameras.png)

「**プリセット**」ドロップダウンを使用して、編集するカメラを選択します。

いずれかの属性が変更された場合、**[復元]ボタン**&#x200B;を使用して元の値に戻すことができます。

![](../../assets/camera-restore.png)

インポートされたカメラのパラメータが変更されている場合、カメラ名は斜体で表示され、カメラ名に&#39;\*&#39;が追加されます。

### カメラ属性

視野または視野は度で表されます。

焦点距離はmmで表されます。

ビューポートモード(OpenGL)では、焦点距離とアパーチャは非アクティブになります。 アクティブ化するには、ポストエフェクトと自由度をアクティブ化する必要があります。

### 表示比率

メッシュファイルに表示比率がある場合は、カメラセクションに表示されます。 カメラの表示比率が定義されていない場合は、**指定なし** （既定のカメラなど）として表示されます。

### ロック

ロックアイコンをクリックすると、カメラをロックできます。 カメラをロックすると、カメラのパラメーターが変更されるのを防ぐことができます。

![](../../assets/image2018-7-26-15-47-6.png)

## カメラフレーム

カメラのフレームは、**画面の設定/ビューポートの設定**&#x200B;で切り替えることができます。

![](../../assets/image2018-7-26-15-54-58.png)

**ゲートマスクの不透明度**&#x200B;で、フレームの外側の領域の不透明度を調整することもできます。

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-45.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-53.png" alt=""/></td>
  </tr>
</table>
