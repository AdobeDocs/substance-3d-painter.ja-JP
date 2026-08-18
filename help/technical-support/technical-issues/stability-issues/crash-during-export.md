---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-during-export.html"
breadcrumb-title: ''
description: 信頼性の高いテクスチャ書き出しワークフローのために、書き出し処理中にSubstance 3D Painterがクラッシュする問題を解決する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash during export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 書き出し中にクラッシュする
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---


# 書き出し中にクラッシュする

特定のケースでは、特に非常に高解像度（4Kや8Kなど）で、書き出し中にSubstance 3D Painterがクラッシュすることがあります。 以下に、この問題の最も一般的な原因のリストを示します。

## TDR（タイムアウトの検出とリカバリ）

TDR(Timeout Detection and Recovery)は、GPUが計算を終わらせることなくシステムをロックするのを防ぐための、Microsoft Windowsの安全メカニズムです。 残念ながら、このメカニズムはデフォルトではSubstance 3D Painterに対して制限が厳しすぎます。

詳しくは、[長時間の計算でGPUドライバーがクラッシュする（TDRクラッシュ）](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)を参照してください。

## 仮想メモリ不足

書き出しは大量のRAM（コンピューターメモリ）を消費する可能性があります。その場合、システムがRAMを使い果たすと、システムは仮想メモリにフォールバックしようとします。 仮想メモリは通常、ハードディスクに保存される追加メモリです。 仮想メモリサイズが小さすぎると、総メモリが不足しているため、Substance 3D Painterがクラッシュします。

詳細については、[仮想メモリ不足によるクラッシュ](crash-with-low-virtual-memory.md)を参照してください。

## ディスク容量の不足

Sparse Virtual Textures (SVT)の登場により、Substance 3D Painterはパフォーマンスのバランスをとるためにキャッシュをディスクにストリーミングできます。 ディスクに十分な空き容量がない場合、アプリケーションがキャッシュを転送および書き込めなかったため、クラッシュする可能性があります。

キャッシュの場所は、既定のシステム一時ファイルフォルダーから移動できます。 詳細については、[スパース仮想テクスチャ](../../../features/sparse-virtual-textures.md)を参照してください。

## オーバークロックGPU周波数

オーバークロックされたGPUは、多くの場合、GPUコンストラクターによって最初に設計されなかった周波数で実行されるため、不安定になります。 オーバークロックをしばらく無効にすると役立つ場合があります。

詳しくは、「[オーバークロックされたGPUで作業中にクラッシュする](../gpu-issues/crash-when-working-with-overclocked-gpu.md)」を参照してください。
