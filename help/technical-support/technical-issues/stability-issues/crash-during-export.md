---
breadcrumb-title: ""
description: テクスチャの書き出し作業で信頼性を高めるために、書き出し操作中にSubstance 3D Painterのクラッシュを修正する方法について説明します。
title: 書き出し中のクラッシュ
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%
---

# 書き出し中のクラッシュ

特定のケースでは、特に非常に高解像度（4Kや8Kなど）で、書き出し中にSubstance 3D Painterがクラッシュすることがあります。 以下に、この問題の最も一般的な原因のリストを示します。

## TDR（タイムアウトの検出とリカバリ）

TDR(Timeout Detection and Recovery)は、GPUが計算を終わらせることなくシステムをロックするのを防ぐための、Microsoft Windowsの安全なメカニズムです。 残念ながら、このメカニズムはデフォルトではSubstance 3D Painterに対して制限が厳しすぎます。

詳細については、[長い計算でのGPUドライバーのクラッシュ(TDRクラッシュ)](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)を参照してください。

## 仮想メモリ不足

書き出しは大量のRAM（コンピューターメモリ）を消費する可能性があります。その場合、システムがRAMを使い果たすと、システムは仮想メモリにフォールバックしようとします。 仮想メモリは通常、ハードディスクに保存される追加メモリです。 仮想メモリサイズが小さすぎると、Substance 3D Painterのメモリ不足によりクラッシュします。

詳細については、[仮想メモリの不足したクラッシュ](crash-with-low-virtual-memory.md)を参照してください。

## ディスク容量の不足

スパース仮想テクスチャ(SVT)の登場により、Substance 3D Painterはディスク上にキャッシュをストリーミングしてパフォーマンスのバランスを取ることができます。 ディスクに十分な空き領域がない場合、アプリケーションがキャッシュを転送および書き込めなかったため、クラッシュが発生する可能性があります。

キャッシュの場所は、既定のシステム一時ファイルフォルダーから移動できます。 詳細については、[スパース仮想テクスチャ](../../../features/sparse-virtual-textures.md)を参照してください。

## オーバークロックGPU周波数

オーバークロックされたGPUは、多くの場合、GPUコンストラクターによって最初に設計されなかった周波数で実行されるため、不安定になります。 オーバークロックをしばらく無効にすると役立つ場合があります。

詳細については、[オーバークロックされたGPUを操作しているときのクラッシュ](../gpu-issues/crash-when-working-with-overclocked-gpu.md)を参照してください。
