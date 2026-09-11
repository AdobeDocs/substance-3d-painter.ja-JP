---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/post-processing/glare.html"
breadcrumb-title: ''
description: Substance 3D Painterでグレアの後処理エフェクトを使用して、明るい領域に逆光やブルーム効果を加える方法を説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Glare
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: グレア
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---


# グレア

![](../../assets/glare-example.jpg)![](../../assets/glare.png)

パラメーターの説明：

| 設定 | 説明 |
| --- | --- |
| **輝度** | グレアエフェクトの全体的な輝度です。 この値を0.0に設定すると、効果が完全に無効になります。  現実的な値の範囲は約0.5 ～ 4.0で、最大値は約16.0です。 |
| **しきい値** | しきい値より明るいピクセルのみが抽出され、グレアが生成されます。  自然な結果を得るには、0.0 ～ 1.0の値を指定することをお勧めします。 |
| **マップの変更** **係数** | 1.0以外の値を指定すると、抽出された高輝度コンポーネントはさらに非線形に拡大（圧縮）されます。 1.0より大きい値を渡すと、明るいピクセルに対してグレアが強くなります。  他のエフェクトに影響を与えずに、グレアの輝度マッピングを個別に調整する場合に使用します。 明るいパスの後の輝度は、滑らかな曲線で増加し、輝度値1.0が&#x200B;**リマップ係数**&#x200B;に近づき、1.0を超える値が（**リマップ** **係数** ^2）に近づきます。 |
| **図形** | シェイプはグレアの外観を定義し、様々なモデルが使用可能です。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ブルーム</strong> ：ブルーム効果のみ。</li><li data-preserve-html="true"><strong>レンズフレア:</strong>開花/ゴースト(レンズフレア)/残像</li><li data-preserve-html="true"><strong>標準：</strong>すべての基本要素をバランスよく含んだ型です。</li><li data-preserve-html="true"><strong>安いレンズ:</strong>安いレンズのシャープなゴーストやその他の表現。 </li><li data-preserve-html="true"><strong>画像の後：</strong>非常に強い残像を持つタイプ。 </li><li data-preserve-html="true"><strong>クロススクリーンフィルター:</strong>十字型スターフィルターのジェネレーターが取り付けられたレンズ。</li><li data-preserve-html="true"><strong>クロススクリーンフィルタースペクトル</strong> ：強力なスペクトラムを付加した十字型スターフィルターのジェネレーターを備えたレンズです。</li><li data-preserve-html="true"><strong>スノークロスフィルター</strong> :6方向のスターフィルターのジェネレーターが取り付けられたレンズ。</li><li data-preserve-html="true"><strong>スノークロスフィルタースペクトル</strong> :6方向のスペクトルが強いスターフィルターのジェネレーターが取り付けられたレンズ。</li><li data-preserve-html="true"><strong>サニークロスフィルター</strong> :8方向のスターフィルターのジェネレーターが取り付けられたレンズ。</li><li data-preserve-html="true"><strong>サニークロスフィルタースペクトル</strong> :8方向のスペクトルが強いスターフィルターのジェネレーターが取り付けられたレンズ。</li><li data-preserve-html="true"><strong>水平ストリーク</strong> ：このレンズフレアの種類は、星に強い水平の筋が入ります。</li><li data-preserve-html="true"><strong>垂直ストリーク</strong> ：垂直方向に星の光が強い書体です。 CCDデジタルカメラ用スミア等</li></ul> |

## シェイプの例

![](../../assets/bloom-examples-bloom.jpg)![](../../assets/bloom-examples-standard.jpg)![](../../assets/bloom-examples-cross.jpg)![](../../assets/bloom-examples-snow.jpg)![](../../assets/bloom-examples-sunny.jpg)![](../../assets/bloom-examples-streak.jpg)
