---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/features/post-processing/tone-mapping.html"
breadcrumb-title: ''
description: Substance 3D Painterのトーンマッピング後処理を使用して、ビューポートの露光量とカラーグレーディングを調整する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Tone Mapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: トーンマッピング
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# トーンマッピング

![](../../assets/tone-mapping.png)

「トーンマッピング」パラメーターを使用すると、画面上に表示されるカラーのスケール方法を制御できます。 これらの設定は、カラーの値の範囲が広い（現在の画面で表示できる範囲を超える可能性がある）ため、カラーを再分配するのに便利です。

>[!NOTE]
>
> Substance 3D Painterは、**HDR** (ハイダイナミックレンジ)カラー（リニアガンマ空間）を出力しますが、ほとんどの画面では、**LDR** （低ダイナミックレンジ）のカラーのみが表示されます。 HDR範囲をLDR範囲にマッピングするには、変換を実行する必要があります。 これがトーンマッピングの原則です。

| *設定* | *説明* |
| --- | --- |
| **露光量** | グレア効果が適用されたり、トーンマッピングが行われる前に、HDR空間のレンダリング結果のスケールを調整します。 |
| **ガンマ** | ガンマ補正のガンマ値です。 |
| **関数** | HDR範囲をLDR範囲にマッピングするために使用する機能。  次の関数を使用できます。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>自動</strong> ：トーンマップ機能が自動的に選択されます。 既定値は<strong>センシトメトリック</strong>です。 </li><li data-preserve-html="true"><strong>線形</strong> ：出力カラーは、このタイプに対してのみ0から1にクランプされません。 これは、エフェクトの適用後にアプリケーション側のHDR領域でエフェクトを実装する場合に最適です。 <br/>使用する特別な理由がない限り、この方法はお勧めしません。線形マッピングを最終的な画面の出力としてそのまま使用すると、高輝度のコンポーネントが完全に失われ、ハイライトが白とびします。</li><li data-preserve-html="true"><strong> LinearSat </strong> ：これは、<strong> Linear </strong>とほとんど同じですが、出力カラーが固定される点が異なります。 また、グレア合成は、<strong>線形</strong>よりも少し滑らかです。</li><li data-preserve-html="true"><strong>センシトメトリック</strong> : HDRスペースでシーンレンダリングを実行する場合の既定の関数です。</li><li data-preserve-html="true"><strong>強く調整</strong> ：これにより、<strong>知覚測定</strong>よりも緩やかなマッピングになり、コントラストがわずかに低くなります。 これにより、高輝度成分の分解能が高くなり、明部における輝度のバラツキの再現性が高くなる。</li><li data-preserve-html="true"><strong> ReinhardLum </strong> ：輝度を基準とし、元の彩度（鮮やかさ：RGB比）を維持して<strong> Reinhard </strong>トーンマップを実装するための種類です。 輝度情報のみをLDR空間にマッピングして、元の彩度を再現します。 HDR空間の彩度は、トーンマッピング後も保持されます。</li><li data-preserve-html="true"><strong>のログ</strong> ：これにより、<strong>のラインハード</strong>よりも段階的なマッピングが行われ、コントラストが低くなります。 これにより、高輝度成分の分解能が高くなり、明部の輝度のばらつきが最も強く再現される。</li><li data-preserve-html="true"><strong> LogLum </strong> ：輝度を基準として対数空間のトーンマップを実装し、元の彩度を維持するための型です（鮮やかさ：RGB比）。 これにより、輝度情報のみが対数空間にマッピングされ、元の彩度が再現されます。 HDR空間の彩度は、トーンマッピング後も保持されます。</li></ul> |
| **マッピング係数** | これにより、トーンマッピングプロセスの最終的なLDRスペースにマッピングされる、HDRスペースの輝度（明るさ）の最大レベルを制御します。 指定されたHDRスペースの輝度よりも明るいカラーは、LDRスペースで表現できないため、ハイライトが白とびします。 具体的には、この値はHDRスペースの輝度（露出スケール後）で、LDRスペースの最大輝度値(1.0)にマッピングされます。 HDRレンダリングモードでは、この値が低いほどコントラストが高くなり、ハイライトが白とびする可能性が高くなります。 逆に、値を大きくすると、コントラストが低くなり、白とびしたハイライトが生じる可能性が低くなります。 LDRレンダリングモードで、エフェクトを適用するためにHDRスペースにリマップする場合、輝度範囲は&#x200B;**マッピング係数**&#x200B;で指定された値まで拡張されます。 逆に、トーンマッピング中に、**マッピング係数**&#x200B;の輝度が最大LDR輝度にマップされます。つまり、エフェクトを適用するLDRレンダリング結果に適用されるダイナミックレンジのスケール係数を指定します。 この値を大きくすると、効果の明るい部分が強調されます。  **注意：** **関数**&#x200B;がHDRレンダリングモードで次のいずれかに設定されている場合、この設定は無効になります（無視されます）: **線形** 、 **線形サット**&#x200B;または&#x200B;**センシトメトリック** 。 |
