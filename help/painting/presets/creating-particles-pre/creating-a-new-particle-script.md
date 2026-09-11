---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/painting/presets/creating-particles-presets/creating-a-new-particle-script.html"
breadcrumb-title: ''
description: Substance 3D Painterで新しいパーティクルスクリプトを作成し、パーティクルブラシのビヘイビアーとエフェクトをカスタマイズする方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Creating A New Particle Script
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 新しいパーティクルスクリプトの作成
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---


# 新しいパーティクルスクリプトの作成

事前設定されたPopcornFXパッケージをダウンロードします： [Templates\_EmitterReceiver.pkkg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/67403778/68419585/1/1411557944000/templates-emitterreceiver.pkkg)

このパッケージは、Substance 3D Painterで編集して読み込むエミッタとレシーバを含む「スタートキット」です。

## Popcorn fxの設定

PopcornFX Editorを起動し、新しいプロジェクトを作成してから開きます。

プロジェクトで、空の領域を右クリックして、「ポップコーンパッケージを読み込み」を選択します。 次に、「Templates\_EmitterReceiver.pkkg」を選択します。

これで、次のことが可能になりました。

* パーティクルの基本エミッターであるエミッターシステム「\_template」。
* 受信者の基本テンプレートであるパーティクルシステム「\_Receiver」。
* シーンのデフォルトの背景として使用される球体メッシュ

「\_Emitter」と「\_Receiver」はすでに「Painter対応」になっています。 これらは既に必要な進化形、フィールド、バックドロップ等で構成されています。

## メッシュを読み込む

PopcornFXは&#x200B;**FBX**&#x200B;のみをサポートしています。メッシュをこの形式で書き出してください。 エクスポートのステップで、メッシュのサイズをチェックして、「実際の世界」で正しい単位に合うようにします。

プロジェクトの「メッシュ」フォルダーにコピー&amp;ペーストします（PopcornFXでは、「メッシュ」フォルダーを右クリックして「ファイルの場所を開く」を選択できます）。

エディターに戻り、メッシュを開き（ダブルクリック）、「**ビルド**」をクリックします。 ウィンドウを閉じ、変更を保存します。

## エミッター/受信者の編集

既存のパーティクルシステムを複製し、新しいメッシュを正しく考慮して適応させます。

パーティクルーシステム「\_エミッター」（「パーティクル」フォルダー内）を右クリックし、「クローン」（または「複製」）を選択して独自のエミッターを作成します。

これを開き、「パーティクルツリービュー」ウィンドウ（左下）で、「**レイヤー\_モデル** 」を選択します。これは、「エディタープロパティ=>背景=> 3Dレイヤー」にあります。

次に、「Node Properties」ウィンドウで「dummymesh.fbx」をモデルに置き換えます。 修正を保存し（ファイル=>保存）、エミッタウィンドウを閉じます。

次に、「\_Receiver **&#x200B;**」**を（「パーティクル」フォルダー内に）コピーして、このフォルダーから独自のReceiverを作成します。**

これを開き、エミッタの場合、ダミーメッシュをLayer\_Modelのモデルで置き換えます。 **画面に表示されているメッシュ** **を変更しましたが、パーティクルが使用している**&#x200B;メッシュ&#x200B;**&#x200B;**&#x200B;も変更する必要があります&#x200B;**。**

これを行うには、「パーティクルツリービュー」ウィンドウで、「**シェイプ** 」をクリックします。これは、「 パーティクルエフェクト=>スポーター=>レイヤー\_1 =>サンプラー=> メッシュ」にあります。

次に、「MeshResource」をモデルに置き換えます。

完了したら、最後に行う作業があります。エミッタとレシーバを、先ほど作成したレシーバと「リンク」する必要があります。

レシーバーのツリービューで、「エディタープロパティ」を選択し、「OverSpawnEffect」でエミッタを選択します。 受信機を保存します。

エミッタ（先ほど複製したエミッタ）を開き、「パーティクルツリー表示」ウィンドウで、「イベントエフェクト=>スポウナー」にある「パーティクル」をクリックします。 次に、「Extern」をクリックして、受信機を置き換えます。\
完了です。 これで、（エミッタまたはレシーバの）3Dビューを選択すると、「スペース」ボタンを押してパーティクルを作成できます。

## オプション：受信機の動作を変更します

レシーバーを開き、「パーティクルツリー表示」ウィンドウで、「パーティクルエフェクト=>レイヤー\_1 =>ステート\_0」にある「 CParticleEvolver\_Script 」（専用の上部：）を選択します。

「Specialized Node Editor」ウィンドウの関数で、「Life = 0.5;」を追加してパーティクルのライフタイムを変更します。 次に、「Ctrl+s」ショートカットを使用してスクリプトを保存します。 3Dビューで違いが見えるはずです。

この機能について詳しくは、以下のリンクを参照してください。

<http://wiki.popcornfx.com/index.php/Main_Page>

## Substance 3D Painterでのエミッター/レシーバの読み込み

Substance 3D Painterで、「ファイル」/「パーティクルを読み込み」を実行するか、Ctrl-Alt-Rを押しながらPack内のエミッターとレシーバー（.pkfx形式の両方）を選択します。

Substance 3D Painterは自動的に要件（パーティクルフィールド、OnCollideイベント）を検出し、pkfxがエミッター、レシーバ、または互換性がないかどうかを判断します。

これで、エミッター/レシーバがシェルフ（「エミッター」タブと「レシーバ」タブ）に表示されます。

これらを使用するには、まず「パーティクルの切り替え」ボタンをクリックする必要があります。

「Tool」ウィンドウの「Physics」で、エミッタを選択し（「default\_emitter」を置き換えます）、レシーバを選択します（「default\_receiver」を置き換えます）。

「ツール」ウィンドウを右クリックしてツールを保存できます。
