---
breadcrumb-title: ""
description: Substance 3D Painterの必要システム構成を確認して、コンピューターがハードウェアとソフトウェアの仕様を満たしていることを確認します。
title: 必要システム構成
user-guide-description: ""
user-guide-title: ""
source-git-commit: fbfe7e52b226b5a92f5b46ebbf82728f0ff9e3c5
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%
---

# サポート対象システム

以下に、アプリケーションでサポートされているハードウェアとシステムのリストを示します。

## Windows

|  | 最小 | おすすめ | 最適 |
| --- | --- | --- | --- |
| **OS** | Windows 11 64ビット版23H2 | Windows 11 64ビット版24H1 | Windows 11 64ビット版24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **ストレージ** | 30 GBの空き容量のあるSSD | 50 GBの空き容量のあるSSD | 70 GBの空き容量のあるSSD |

### macOS

|  | 最小 | おすすめ | 最適 |
| --- | --- | --- | --- |
| **OS** | macOS 15セコイア | macOS 27ゴールデンゲート | macOS 27ゴールデンゲート |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **ストレージ** | 30 GBの空き容量のあるSSD | 50 GBの空き容量のあるSSD | 70 GBの空き容量のあるSSD |

>[!WARNING]
>
> [VFX Reference Platform](https://vfxplatform.com/)を念頭に置いて構築されたパイプラインでは、macOS 14 SonomaにSubstance 3D Painterをインストールできます。 ただし、Painterは、最小必要システム構成を下回るOSバージョンではテストされていないため、安定性は保証されていません。

### Linux

| Enterprise | スチーム |
| --- | --- |
| RHEL 8<br>RHEL 9 | Ubuntu 22.04 |

## 一般的な推奨事項

UV タイルワークフローを使用する際に適切なパフォーマンスを得るには、次の使用をお勧めします。

* 32 GBのRAM
* 8 GBのVRAMを搭載したGPU
* プロジェクトとアプリケーションキャッシュの両方を保存するSSD。

その他 :

* 多くのSubstanceアプリは、RHEL8/9との互換性をOpenSSL 1.1.1に依存しています。 新しいバージョンのOpenSSLを使用するシステムの場合は、お客様が手動で提供する必要があります
* 快適な状態で作業するには、1000ピクセルを超え、1280ピクセルを超える縦長の解像度のモニターをお勧めします。
* **8K** （8192\*8192ピクセル）で書き出すには、**2 GBを超えるVRamを搭載したGPUが必要です。**
* macOS 10.15(Catalina)で実行するために公証されたのは、バージョン2019.x以降のみです。
* RDP （リモートデスクトップ）経由でソフトウェアを使用するには、専用の[ドキュメントページ](../pipeline-and-integration/configuration/remote-desktop.md)を参照してください。
* ベイク時のRyzen CPUのクラッシュは、BIOSをアップデートすることで修正できます。

## サポートされていない設定

**ウィンドウ**

* 仮想マシンはサポートされていません。
* Windows Serverはサポートされていません。

**Mac**

* 公式のApple設定のみがサポートされています。
* eGPUは現在サポートされておらず、安定性の問題がある可能性があります。

**Linux**

* Linux上のMesaドライバはサポートされていません。

**任意のプラットフォーム**

* 内蔵GPUは、x86-64(Intel、AMD)CPUではサポートされていません。

## GPUドライバーの最小バージョン

アプリケーションを問題なく実行するために必要なGPUドライバーの最小バージョンを以下に示します。 このリストは、新しいバージョンのリリースに伴って変更される場合があります。

新しいドライバーをダウンロードするには、[GPUに古いドライバーがあります](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md)を参照してください。

| OS | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **ウィンドウ** | GeForce 442.50 Quadro 442.50 | Radeon 19.7.1 Radeon Pro / FirePro 18.Q4 | 15.33 |
| **Linux** | 535.171.04以降 | Radeon 22.40.6 | 非対応 |

>[!NOTE]
>
> **Mac OS**&#x200B;では、GPUドライバーはオペレーティングシステム自体から提供されます。 最新のドライバーにアクセスするには、OSを最新バージョンにアップデートしてください。

### ドライバーの互換性の問題

コンストラクターごとのGPUドライバーの問題の詳細な一覧については、[専用のドキュメントページ](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md)を参照してください。

## ベイク用GPU レイトレーシング

OptixまたはDXR経由でGPU レイトレーシングを有効にするには、上記の最小推奨ドライバーをインストールする必要があります。

**DXR**&#x200B;には、次の最小構成も必要です：

* **Windows 10**&#x200B;バージョン1809。詳細については、[このページ](https://experienceleague.adobe.com/ja/docs/substance-3d/bakers/features/gpu-raytracing)を参照してください
* **Pascalアーキテクチャ搭載GPU** (Nvidia GeForce 10XX)

>[!TIP]
>
> GPU レイトレーシングは、NVIDIA GeForce RTXまたはNVIDIA Quadro RTX GPUなどの専用レイトレーシングハードウェア上で最適に実行されます。

## サポートされているグラフィックタブレット

以下は、Substance 3D Painterバージョン&#x200B;**7.4.2**&#x200B;でテストされた、互換性のあるグラフィックタブレットのリストです。

+++Wacom

**モデル:** Intuos Pro （Mサイズ）、Intuos （Sサイズ）

| OS | ドライバーバージョン |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |

+++

+++XPen

**モデル：**&#x200B;デコ01

| OS | ドライバーバージョン |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |
| Linux | XP-ペン – ペンタブレット–3.2.1.211019-1 |

+++

+++フイオン

**モデル：** Q11K

| OS | ドライバーバージョン |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |

+++

+++Xencelabs

**モデル：** ペンタブレット（中）

| OS | ドライバーバージョン |
| --- | --- |
| Windows | XencelabsWin_1.2.1-14 |
| macOS | XencelabsMac_1.2.1-18 |
| Linux | XencelabsLinux_1.1.0-2 |

+++

## サポートされている3Dconnexion SpaceMouseモデル

Substance 3D Painterバージョン&#x200B;**8.1.**&#x200B;でテストされた[3Dconnection Space Mouse](https://3dconnexion.com/us/spacemouse/)用の互換性のあるドライバーバージョンの一覧を次に示します

ドライバーのバージョンは、**コンパクト**、**Pro**&#x200B;および&#x200B;**エンタープライズ**&#x200B;モデルに適用されます。

| OS | ドライバーバージョン |
| --- | --- |
| Windows | 10.8.6.3431 |
| macOS | 10.7.2.3454 |

## 言語

ソフトウェアインターフェイスは次の言語で使用できます。

* 英語（米国）
* Deutsch
* スペイン語
* Français
* イタリア語
* 日本語
* 韓国語
* ポルトガル語（ブラジル）
* 中国語（簡体）
