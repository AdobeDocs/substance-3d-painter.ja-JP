---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/technical-issues/rendering-issues/broken-viewport-ubuntu.html"
breadcrumb-title: ''
description: Substance 3D PainterのUbuntuでビューポートが壊れたり反応しなくなったりする問題を修正し、3Dレンダリングを適切に行う方法を説明します。
helpx_creative_field: ""
helpx_description: Viewport appears broken or unresponsive on Ubuntu
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ubuntuでビューポートが壊れているか、応答しない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# Ubuntuでビューポートが壊れているか、応答しない

バージョン11.1以降のUbuntuでSteamからPainterを実行すると、ビューポートが壊れているか、応答していないように見えることがあります。

これは、Painterが、適切なGPUが割り当てられて起動しない場合に発生します。 Ubuntuでは、控えめなGPUの代わりに統合GPUが選択されることがあります。 Painterは、この設定をSteamから引き継いでいるため、問題が発生する可能性があります。

いくつかの解決策があります。

1. ターミナルからSteamを実行します。 これにより、強制的に異なるコンテキストが生成され、SteamとPainterが適切なGPUで実行されます。
1. Steamショートカットを編集して、<b>専用のグラフィックスカードを使って実行</b>設定を無効にします。 その後、通常どおりSteamを実行します。

詳細については、[このgithub問題](https://github.com/ValveSoftware/steam-for-linux/issues/9940)を参照してください。
