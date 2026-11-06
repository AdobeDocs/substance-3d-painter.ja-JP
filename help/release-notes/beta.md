---
description: 新機能と完全なチェンジログを含む、現在のSubstance 3D Painterベータ版について説明します。
title: ベータリリース
source-git-commit: 3f87068a5a29fd50d7b1e3857691e9a396775175
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%
---

# ベータ版リリースノート

## V12.2.1

Substance 3D Painterのこのベータ版は、ARM(ARM64)システム上のWindowsのネイティブサポートを追加します。 チームが安定性の向上に取り組んでいるため、今後数週間でさらにリリースされる予定です。

### ビルド3

**固定**:

* &lbrack;Mac&rbrack;&lbrack;OpenPBR&amp;rbrack；特定のサブサーフェス半径スケール値を持つビューポートのテクスチャアーティファクト
* &lbrack;Mac&rbrack;ディスプレイ設定のテクスチャミップマップからのフィルタリングバイアスは何の影響も与えません
* &lbrack;Windows&rbrack;&lbrack;Nvidia&rbrack;ブラシおよびマテリアルプレビューの生成により、TDRが発生する可能性がある

### ビルド2

リリース日： **2026年11月2日**

**追加済み**:

* &lbrack;ベイク処理&rbrack; Highpoly Matching Error Visualization uses Match-by-Name

**固定**:

* &lbrack;Python&amp;rbrack；一部の非推奨の関数は警告を表示しますが、その関数が誰であるかは表示しません
* &lbrack;ベイク&rbrack;ケージジオメトリは、1つのUV アイランドにペイントするときに穴を開けることができます
* &lbrack;Mac&rbrack;&lbrack;ベイク処理&rbrack;ベイク処理モードでのケージペイントのビューポートのパフォーマンスの問題

### ビルド1

リリース日： **2026年10月21日**

**追加済み**:

* Substance 3D PainterはWinARMマシンをネイティブにサポートするようになりました。

**固定**:

* ケージペイントを使用したMacで、ベイク処理モードビューポートのパフォーマンスの問題(&lbrack;ベイク処理&rbrack;)。
