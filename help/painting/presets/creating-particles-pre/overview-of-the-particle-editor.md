---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/creating-particles-presets/overview-of-the-particle-editor.html"
breadcrumb-title: ''
description: Substance 3D Painterのパーティクルエディターについて学習し、テクスチャペイント用のカスタムパーティクルブラシプリセットを作成します。
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Overview of the particle editor
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: パーティクルエディタの概要
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---


# パーティクルエディタの概要

このページでは、PopcornFXパーティクルエディタの複数の側面について説明します。 ウィンドウのタイトルとパラメーターの一部は、使用されているエディターのバージョンによって変更される場合があります。

## ビューポート設定

### 独自のメッシュをインポートする方法

Packの「Meshes」フォルダーにメッシュをコピー&amp;ペーストします。 次に、エディタでメッシュを開き、「構築」をクリックします。

次に、パーティクルシステムで、ツリービューの[Backdrop]に移動し、[3Dレイヤ]、[New Backdrop]、[CNEdEditorBackdrop\_Model3D]を右クリックして、[リソースモデル]でメッシュを選択します。

Substance 3D Painterでは、メッシュは各軸のサイズ[-1;1]のボックス内に収まるように拡大/縮小されます。 エディタでSubstance 3D Painterを使用して適切なスケールを得るには、ボックスに収まるように既にスケールされているメッシュをインポートするか（簡単な方法）、エディタでスケールを操作する必要があります。

注： FBXメッシュ形式のみがサポートされています。

#### グリッドの表示方法

Ctrl+Gを押します。「エディターのプロパティ」「GridColor」でグリッドの色をカスタマイズできます。

## エミッター

### 「OnCollide」イベントの作成方法

Physics Evolverは、シーン内の背景メッシュとの衝突を処理します。 Substance 3D Painterでは、シーンはメッシュになります。

Physics Evolverでは、まず「WorldInteractionMode」を「OneWay」に設定して、パーティクルの衝突を有効にします。 次に、「OnCollide」というイベントを作成します。Physics Evolverは、シーンとの衝突時にイベントをトリガーします。

Substance 3D Painterでは、シーンは作業中のモデルであり、「OnCollide」と呼ばれるすべてのイベントは、現在のブラシのエミッタパーティクルシステムによってオーバーライドされます。

#### カメラからパーティクルを発射する方法

ビューポートの上部で、4番目の[カメラ平面にスポーンを拘束]ボタンを有効にします。

Substance 3D Painterは、初期設定でカメラからエミッタを発射します。

#### 雨のようにパーティクルを上部に放出する方法

有効になっている場合は、「カメラ平面にスポーンを制限」を無効にします。

「グローバル」というパーティクルアトリビュートを作成します。これで、Substance 3D Painterは原点でパーティクルをスポーンします。

メッシュの上部にスポーンするには、シェイプSampler BOXまたはCYLINDERを追加し、その上に配置して、スポーナースクリプトでサンプリングします。

たとえば、「Spawn」というシェイプSampler BOXを使用して、これをSpawner Scriptに追加します。

*Position = Spawn.samplePosition();*

## レシーバー

### レシーバの作成/編集中にエミッタを生成する方法

レシーバの編集中にSubstance 3D Painterのワークフローにより近づけるために、生成されたパーティクルシステムをオーバーライドするようにエディタを設定できます。

レシーバーのツリーで、「エディタープロパティ」を選択し、「UserOverSpawn」を有効にして、「OverSpawnEffect」でエミッタを選択します。

この場合も、エミッタを開いて「OnCollide」イベントを設定し、現在編集中のレシーバを起動する必要があります。

#### パーティクルフィールドの設定方法

レシーバに必要なパーティクルフィールドの説明を次に示します。

*&quot;Size&quot;浮動小数点*

Substance 3D Painterのブラシサイズの乗数。

*&quot;不透明度&quot;浮動小数点*

Substance 3D Painterのブラシの不透明度の乗数です。

*「UV」float3*

パーティクルのメッシュ上のテクスチャ座標。

Evolver Scriptでは、プロジェクションエボリュバーによって指定されたパラメトリック座標を使用して、シェイプSamplerの「メッシュ」をサンプリングします。

UV = Mesh.sampleTextcoord(pCoords);

*&quot;Normal&quot;浮動小数点3*

パーティクルの下のメッシュサーフェスの法線。

Evolver Scriptでは、プロジェクションエボリュバーによって指定されたパラメトリック座標を使用して、シェイプSampler「メッシュ」をサンプリングします。

Normal = normalize(Mesh.sampleNormal(pCoords));

*&quot;シード&quot; int*

Substance 3D Painterにランダムに生成された値：

Evolver Scriptでは、次のように追加します。

シード= int(rand(0,20000000));

*&quot;pCoords&quot; int3*

Substance 3D Painterでは使用されていませんが、メッシュ上のパーティクルプロジェクションを実行し、他のフィールドをサンプリングするために不可欠です。

#### メッシュ上にパーティクルを投影する方法

レシーバーの「State\_0」にプロジェクションエボバーを追加します。

各フレームで、プロジェクションエボリュバーはシェイプSamplerの最も近いサーフェスにパーティクルを投影します。

投影エボリュバーは、「OutputParametricCoordsField」で指定されたパーティクルフィールド（「pCoords」パーティクルフィールドを参照）で、投影のパラメトリック座標を入力できます。

また、「ReprojectedField」を使用して、メッシュのサーフェス上にベクトルを再投影することもできます。

ここでは、Samplerシェイプの「メッシュ」にパーティクルを投影し、int3パーティクルフィールド「pCoords」でパラメトリック座標を入力し、サーフェス上にも「速度」を投影します。

#### メッシュをサンプリングする方法

Substance 3D Painterでは、「Mesh」および「ShapeType」の「MESH」と呼ばれるすべてのシェイプサンプラーが、Substance 3D Painterで使用されているメッシュで上書きされます。<b>\
</b>

エディタで、背景と同じメッシュに設定します。

スクリプトでオブジェクトをサンプリングするには、スクリプトに&quot;Mesh.sample~Something~(pCoords)&quot;と記述します。以下にドキュメントを示します。

<https://wiki.popcornfx.com/index.php/CParticleSamplerShape#Script_bindings>

必要となる便利なコードスニペットは次のとおりです。

```
// UV is the texture coordinate of the particle on the mesh

// Must be after CParticleEvolver_Projection

UV = Mesh.sampleTexcoord(pCoords);

// Normal is the Normal of the surface on the mesh just below the particle

// Must be after CParticleEvolver_Projection

Normal = normalize(Mesh.sampleNormal(pCoords));
```


## 一般的なヒント

### Substance 3D Painterでエミッタ/レシーバをインポートする方法

Substance 3D Painterで、「ファイル」/「パーティクルを読み込み」を実行するか、Ctrl-Alt-Rを押しながらPackのEmitter.pkfxまたはReceiver.pkfxを選択します。

Substance 3D Painterは自動的に要件（パーティクルフィールド、OnCollideイベント）を検出し、pkfxがエミッタ、レシーバ、または互換性がないかどうかを判断します。

これで、エミッタ/レシーバがシェルフに表示されます。

#### 実行可能なパーティクルサイズでパーティクルをデバッグする方法

「サイズ」パーティクルフィールドは、Substance 3D Painterのブラシサイズの乗数として0 ～ 1の範囲で設定する必要があるため、パーティクルはエディタ内で大きすぎます。 したがって、パーティクルを見やすくするために、Billboardパーティクルレンダラーで「SizeField」として使用する、スポーナースクリプトでカスタムフィールド浮動小数点の「BBSize」を0.01に設定します。

#### 進化の秩序を台無しにする方法

進化者の序列は非常に重要な場合がある。

たとえば、最後の2つのエボルバを必ず投影エボルバにし、次に投影エボルバで生成されたpCoordsを使用してUVと法線をサンプリングするスクリプトエボルバを設定することができます。

進化形の順序は文字通りフレーム内の実行順序であり、Substance 3D Painterはパーティクルフィールドの値と各フレームの終わりを収集することに注意してください。

#### メッシュの法線マップをサンプリングする方法

Substance 3D Painterは、「NormalMap」と呼ばれるすべてのテクスチャサンプラーをメッシュの法線マップ（インポートした場合）に置き換えます。

現時点で唯一のテクスチャですが、他のすべてのテクスチャにはSubstance 3D Painterではアクセスできません。

「NormalMap」というテクスチャSamplerを追加すると、スクリプトでサンプリングできます。

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerTexture>

便利なコードスニペット：

```
// In Evolver Script convert the NormalMap texture in tangent space to world space normal

// /!\ the "Normal" particle field must always be the normal of the mesh not influenced by the normal map

// /!\ dont forget to initialize your particle fields in your Spawn Script

// otherwise pCoords and Normal will be invalid at the first update

float normalFactor = 1.0; // change the intensity of the normal map

float3 meshnormal = Normal;

float4 rawtangent = Mesh.sampleTangent(pCoords);

float3 binormal = normalize(cross(meshnormal, rawtangent.xyz) * rawtangent.w);

float3 tangent = normalize(cross(meshnormal, binormal));

float3 tsNormal = normalize(((NormalMap.sample(UV).xyz * 2.0 - 1.0).xyz) * float3(-normalFactor, normalFactor, 1));

float3 normal = normalize(tsNormal.x * tangent + tsNormal.y * binormal + tsNormal.z * meshnormal);
```


#### 乱気流の作成方法

エディタで、乱気流Samplerを作成します。

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerProceduralTurbulence>

次に、タービュランスをサンプリングしてパーティクルに影響を与える2つの方法があります。

##### 簡単な方法

レイヤーのPhysics Evolverで、「VelocityFieldSampler」をタービュランスSampler名に設定し、「Drag」を値>0に設定します。

##### パラメーター化された方法

アトリビュートを使用して乱気流を調整するには、Evolverスクリプトで乱気流Samplerによって生成されたベロシティフィールドをサンプリングします。

2つのパーティクルアトリビュートを作成する：

* float &quot;TurbulencePower&quot; minmax: [0;5]
* float &quot;TurbulenceScale&quot; minmax: [0.001; 5] （0以上である必要があります）

次に、3つのパーティクルフィールドを作成します。

float &quot;TurbPower&quot;およびfloat &quot;TurbScale&quot;

Spawnerスクリプトにアトリビュートを格納するには：

* TurbScale = 1.0 / TurbulenceScale;
* TurbPower = TurbulencePower;

float3 「VelocityField」を回転モードで使用します。

これはPhysics Evolverの「VelocityField」として使用されます（デフォルトでは「VelocityField」フィールドに設定されています）。

それで、Physics Evolverの前に、Script Evolverで「Turb」と呼ばれる乱気流Samplerをサンプリングします。

VelocityField = Turb.sample(Position \* TurbScale) \* TurbPower;

#### dtの正しい使用方法（デルタタイム）

デルタタイムは、各フレームの更新間のシミュレーション時間（秒単位）です。 エディタでは、デルタ時間は実際の経過時間で更新されます。 Substance 3D Painterでは、デルタ時間が修正され、最後のアップデートが終了するとすぐに、各アップデートが起動されます。

60 FPSでプレイするゲームのデルタタイムは1/60= 0.016秒なので、0.016秒のデルタタイムでプレイしてみてください。

* ビッグデルタタイム> 0.016s
* PROの高速アップデート

更新間隔が大きいほどパーティクルの動きが大きくなるので、Substance 3D Painterでのブラシの実行速度が速くなります。

* コン近似

PopcornFXは一種の大きな離散化システムなので、dtが大きいほど、精度は高くなります。 乱気流に大きなデルタ時間の影響を参照： <http://www.popcornfx.com/wiki/index.php/CParticleEvolver_Physics#Dealing_with_turbulences_at_low_framerates>

* コンスプラット

デルタ時間が大きい場合は、フレーム間のパーティクルの動きも大きくなります。 そのため、Substance 3D Painterでは、直線の代わりに小さな斑点が表示される場合があります。

これは、Substance 3D Painterでは、各フレームの最後にパーティクルごとに1つのストロークポイントが描画されるためです。また、最後のフレームと現在のフレームの間にはパーティクルごとに線が描画されません。

* Little delta time &lt; 0.016s
* PRO precision

この値を小さくすると、ブラシストローク間の距離が短くなり、描画がよりシャープになります。 シミュレーションの分離も良くなります。

* コンスロー

デルタ時間が短いほど、同じ距離を描くために必要な更新回数が多くなります。

デルタ時間の最後のヒント：適切なdtを得るための良い方法は、大きなdt(0.1s)から始めて、ステップごとに減らして、必要な結果を得ることです。

#### パーティクルシステムのパラメータを表示する方法

Substance 3D Painterはパーティクルシステムのパーティクルアトリビュートを収集し、物理ブラシのパラメータに表示します。

<http://www.popcornfx.com/wiki/index.php/Particle_effect_attributes>

PopcornFXには、「Attributes in Evolve」という機能があります。この機能を使用すると、Evolveスクリプトの属性にアクセスできます。この機能を使用しないでください。 代わりに、パーティクルフィールドを作成し、その中にアトリビュートを格納します。次に、これらのパーティクルフィールドをエボラスクリプトで使用します。 （これは将来修正される可能性があります）

#### 問題のあるパーティクルを検出する方法

パーティクルフィールドの値が奇妙なパーティクルは決して存在すべきではありません。そのため、問題が発生する可能性のあるパーティクルを何度も分割するようにしてください。

<http://www.popcornfx.com/wiki/index.php/Particle_tips_BreakOnProblematicParticle>

#### Substance 3D Painterでパーティクルシステムの問題を解決する方法

Substance 3D Painterのインストールディレクトリに、「popcorn.htm」というファイルがあります。 このファイルにはPopcornFXのすべてのログが含まれています。内部を見て、何が間違って起こったのかを確認してください。

#### パーティクルフィールドを正しく初期化する方法

最初のフレームから有効なpCoords UVとNormalを取得するには、これをSpowner Scriptに追加します。

<b>  
</b>

```
// PostEval() will be called after particles have been translated to their respective spawn locations

// so, PostEval() is executed in world space

function void PostEval()

{

// we need to initialize correctly the values needed by Substance 3D Painter:

pCoords = Mesh.projectParametricCoords(Position);

UV = Mesh.sampleTexcoord(pCoords);

Normal = normalize(Mesh.sampleNormal(pCoords));

}
```
