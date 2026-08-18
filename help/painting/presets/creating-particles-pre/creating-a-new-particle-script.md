---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/creating-particles-presets/creating-a-new-particle-script.html"
breadcrumb-title: ''
description: Substance 3D Painterで新しいパーティクルスクリプトを作成し、カスタムパーティクルブラシのビヘイビアーとエフェクトを定義する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Creating A New Particle Script
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 新しいパーティクルスクリプトを作成する
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---


# 新しいパーティクルスクリプトを作成する

事前設定されたPopcornFXパッケージをダウンロードします： [Templates\_EmitterReceiver.pkkg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/67403778/68419585/1/1411557944000/templates-emitterreceiver.pkkg)

このパッケージは、Substance 3D Painterで編集して読み込むエミッタとレシーバを含む「スタートキット」です。

## Popcorn fxの設定

PopcornFX Editorを起動し、新しいプロジェクトを作成してから開きます。

プロジェクトで、空の領域を右クリックして、「ポップコーンパッケージを読み込み」を選択します。 次に、「Templates\_EmitterReceiver.pkkg」を選択します。

これで、次のことが可能になりました。

* エミッタのベーステンプレートであるパーティクルシステム「\_Emitter」。
* パーティクルシステム「\_Receiver」は、レシーバのベーステンプレートです。
* シーンのデフォルトの背景として使用される球体メッシュ

「\_Emitter」と「\_Receiver」はすでに「Painter対応」になっています。 これらは既に必要な進化形、フィールド、バックドロップ等で構成されています。

## メッシュをインポートする

PopcornFXは&#x200B;**FBX**&#x200B;のみをサポートしています。メッシュをこの形式で書き出してください。 エクスポートのステップで、メッシュのサイズをチェックして、「実際の世界」で正しい単位に合うようにします。

プロジェクトの「メッシュ」フォルダーにコピー&amp;ペーストします（PopcornFXでは、「メッシュ」フォルダーを右クリックして「ファイルの場所を開く」を選択できます）。

エディターに戻ってメッシュを開き（ダブルクリック）、「**ビルド**」をクリックします。 ウィンドウを閉じ、変更を保存します。

## エミッタ/レシーバの編集

既存のパーティクルシステムを複製し、新しいメッシュを正しく考慮して適応させます。

パーティクルシステム「\_Emitter」（「パーティクル」フォルダ内）を右クリックし、「クローン」（または「複製」）を選択して独自のエミッタを作成します。

これを開き、「Particle Treeview」ウィンドウ（左下）で、「Editor Properties => Backdrop => 3D Layers」にある「**Layer\_Model**」を選択します。

次に、「Node Properties」ウィンドウで「dummymesh.fbx」をモデルに置き換えます。 修正を保存し（ファイル=>保存）、エミッタウィンドウを閉じます。

次に、「\_Receiver ****」**を（「パーティクル」フォルダー内で）クローンし、このフォルダーから独自のReceiverを作成します。**

これを開き、エミッタの場合、ダミーメッシュを「レイヤー\_モデル」のモデルで置き換えます。 **画面に表示されている** **メッシュを修正**&#x200B;しましたが、パーティクルで使用されている&#x200B;**メッシュ** **も修正する必要があります** 。

これを行うには、「Particle Treeview」ウィンドウで、「**Shape** 」をクリックします。これは、「 Particle Effect => Spawner => Layer\_1 => Samplers => Mesh 」にあります。

次に、「MeshResource」をモデルに置き換えます。

完了したら、最後に行う作業があります。エミッタとレシーバを、先ほど作成したレシーバと「リンク」する必要があります。

レシーバーのツリービューで、「エディタープロパティ」を選択し、「OverSpawnEffect」でエミッタを選択します。 受信機を保存します。

エミッタ（先ほど複製したエミッタ）を開き、「パーティクルツリービュー」ウィンドウで、「パーティクルエフェクト=>スポウナー」にある「イベント」をクリックします。 次に、「Extern」をクリックして、受信機を置き換えます。\
完了です。 これで、（エミッタまたはレシーバの）3Dビューを選択した場合、「スペース」ボタンを押してパーティクルを作成できます。

## オプション：受信機の動作を変更します

レシーバを開き、「Particles Treeview」ウィンドウで、「Particle Effect => Layer\_1 => State\_0」にある「 CParticleEvolver\_Script 」（専用見出し：）を選択します。

[Specialized Node Editor]ウィンドウの関数で、「Life = 0.5;」を追加してパーティクルのライフタイムを変更します。 次に、「Ctrl+s」ショートカットを使用してスクリプトを保存します。 3Dビューで違いが見えるはずです。

この機能について詳しくは、以下のリンクを参照してください。

<http://wiki.popcornfx.com/index.php/Main_Page>

## Substance 3D Painterでのエミッタ/レシーバの読み込み

Substance 3D Painterで、「ファイル」/「パーティクルを読み込み」を実行するか、Ctrl-Alt-Rを押して、Pack内のエミッタとレシーバ（.pkfx形式の両方）を選択します。

Substance 3D Painterは自動的に要件（パーティクルフィールド、OnCollideイベント）を検出し、pkfxがエミッタ、レシーバ、または互換性がないかどうかを判断します。

これで、エミッタ/レシーバがシェルフ（「エミッタ」タブと「レシーバ」タブ）に表示されます。

これらを使用するには、最初に「パーティクルの表示/非表示」ボタンをクリックする必要があります。

「Tool」ウィンドウの「Physics」で、エミッタを選択し（「default\_emitter」を置き換えます）、レシーバを選択します（「default\_receiver」を置き換えます）。

「ツール」ウィンドウを右クリックしてツールを保存できます。
