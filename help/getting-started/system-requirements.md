---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/system-requirements.html"
breadcrumb-title: ''
description: Substance 3D Painterの必要システム構成を確認して、コンピューターがハードウェアとソフトウェアの仕様を満たしていることを確認します。
helpx_creative_field: ""
helpx_description: Painter > Getting Started > System requirements
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 必要システム構成
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---


# サポート対象システム

以下に、アプリケーションでサポートされているハードウェアとシステムのリストを示します。

## Windows

|  | 最小 | おすすめ | 最適 |
| --- | --- | --- | --- |
| <b>OS</b> | Windows 11 64ビット版23H2 | Windows 11 64ビット版24H1 | Windows 11 64ビット版24H2 |
| <b>CPU</b> | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| <b>GPU</b> | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| <b>VRAM</b> | 8 GB | 16 GB | 24 GB |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>ストレージ</b> | 30 GBの空き容量のあるSSD | 50 GBの空き容量のあるSSD | 70 GBの空き容量のあるSSD |

### macos

|  | 最小 | おすすめ | 最適 |
| --- | --- | --- | --- |
| <b>OS</b> | macOS 12 Monterey | macOS 13 Ventura | macOS14ソノマ |
| <b>CPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>GPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>ストレージ</b> | 30 GBの空き容量のあるSSD | 50 GBの空き容量のあるSSD | 70 GBの空き容量のあるSSD |

### Linux

| Enterprise | スチーム |
| --- | --- |
| RHEL 8</br>RHEL 9 | Ubuntu 22.04 |

## 一般的な推奨事項

UVタイルワークフローを使用する際に良好なパフォーマンスを得るには、次の使用をお勧めします。

* 32 GBのRAM
* 8 GBのVRAMを搭載したGPU
* プロジェクトとアプリケーションキャッシュの両方を保存するSSD。

その他 :

* 多くのSubstanceアプリは、RHEL8/9との互換性をOpenSSL 1.1.1に依存しています。 新しいバージョンのOpenSSLを使用するシステムの場合は、お客様が手動で提供する必要があります
* 快適な状態で作業するには、1000ピクセルを超え、1280ピクセルを超える縦長の解像度のモニターをお勧めします。
* <b>8K</b> （8192\*8192ピクセル）で書き出すには、<b>2 GBを超えるVRamを搭載したGPUが必要です。</b>
* macOS 10.15(Catalina)で実行するために公証されたのは、バージョン2019.x以降のみです。
* RDP （リモートデスクトップ）経由でソフトウェアを使用するには、専用の[ドキュメントページ](../pipeline-and-integration/configuration/remote-desktop.md)を参照してください。
* ベイク時にRyzen CPUでクラッシュする問題は、BIOSをアップデートすることで解決できます。

## サポートされていない設定

<b>ウィンドウ</b>

* 仮想マシンはサポートされていません。
* Windows Serverはサポートされていません。

<b>Mac</b>

* 公式のApple設定のみがサポートされています。
* eGPUは現在サポートされておらず、安定性の問題がある可能性があります。

<b>Linux</b>

* Linux上のMesaドライバはサポートされていません。

<b>任意のプラットフォーム</b>

* 内蔵GPUは、x86-64(Intel、AMD)CPUではサポートされていません。

## GPUドライバーの最小バージョン

アプリケーションを問題なく実行するために必要なGPUドライバーの最小バージョンを以下に示します。 このリストは、新しいバージョンのリリースに伴って変更される場合があります。

新しいドライバーをダウンロードするには、[GPUに古いドライバーがあります](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md)を参照してください。

| OS | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| <b>ウィンドウ</b> | GeForce 442.50 Quadro 442.50 | Radeon 19.7.1 Radeon Pro / FirePro 18.Q4 | 15.33 |
| <b>Linux</b> | 535.171.04以降 | Radeon 22.40.6 | 非対応 |

>[!NOTE]
>
> **Mac OS**&#x200B;では、GPUドライバーはオペレーティングシステム自体から提供されます。 最新のドライバーにアクセスするには、OSを最新バージョンにアップデートしてください。

### ドライバーの互換性の問題

コンストラクターごとのGPUドライバーの問題の詳細な一覧については、[専用のドキュメントページ](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md)を参照してください。

## 焼き用GPU レイトレーシング

OptixまたはDXR経由でGPU レイトレーシングを有効にするには、上記で推奨されている最小ドライバをインストールする必要があります。

<b>DXR</b>には、次の最小構成も必要です：

* <b>Windows 10</b>バージョン1809。詳細については、[このページ](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/features/gpu-raytracing)を参照してください
* <b> GPU、Pascalアーキテクチャ</b> (Nvidia GeForce 10XX)

>[!TIP]
>
> GPU レイトレーシングは、NVIDIA GeForce RTXまたはNVIDIA Quadro RTX GPUなどの専用レイトレーシングハードウェアで最適に実行されます。

## サポートされているグラフィックタブレット

以下は、Substance 3D Painterバージョン<b>7.4.2</b>でテストされた、互換性のあるグラフィックタブレットのリストです。

+++Wacom
<b>モデル:</b>Intuos Pro （Mサイズ）、Intuos （Sサイズ）


| OS | ドライバーバージョン |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |


+++

+++XPen
<b>モデル：</b>デコ01


| OS | ドライバーバージョン |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |
| Linux | XP-PEN-pentablet-3.2.1.211019-1 |


+++

+++フイオン
<b>モデル：</b> Q11K


| OS | ドライバーバージョン |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |


+++

+++Xencelabs
<b>モデル：</b>ペンタブレット（中）


| OS | ドライバーバージョン |
| --- | --- |
| Windows | XencelabsWin\_1.2.1-14 |
| macOS | XencelabsMac\_1.2.1-18 |
| Linux | XencelabsLinux\_1.1.0-2 |


+++

## サポートされている3Dconnexion SpaceMouseモデル

Substance 3D Painterバージョン<b>8.1.</b>でテストされた[3Dconnection Space Mouse](https://3dconnexion.com/us/spacemouse/)用の互換性のあるドライバーバージョンの一覧を次に示します

ドライバーのバージョンは、<b>コンパクト</b>、<b>Pro</b>および<b>エンタープライズ</b>モデルに適用されます。

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
