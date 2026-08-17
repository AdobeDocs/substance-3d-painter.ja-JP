---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/technical-support/project-resources.html"
breadcrumb-title: ''
description: Substance 3D Painterのプロジェクトリソースと技術文書にアクセスして、ワークフローとトラブルシューティングを強化します。
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: プロジェクトリソース
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# プロジェクトのリソースと設定

プロジェクトリソースを管理することで、Painterでのプロジェクトのパフォーマンスに適した基盤を構築できます。

+++ベイク済みマップを縮小
すべてのベイク済みマップが2Kまたは4K解像度である必要がない場合もあります。 2Kでバッチをベイクしてから、視覚的に違いがあるかどうかを確認するために、低い解像度で再ベイクしてください。

+++

+++読み込まれたビットマップの管理
読み込まれた画像はパフォーマンスに大きな影響を与える可能性があるため、読み込まれる画像に注意することが重要です。 テクスチャセットが2Kに設定されていて、これより高い解像度では書き出されない場合、8K画像を使用しても良い影響はありません。テクスチャセットの解像度であるため、画質は2Kに制限されます。

フォーマットも重要です。EXR、HDR、そしてPNGでさえ、JPGよりもはるかに重く、すべての画像がEXRの画質のレベルを必要とするわけではありません（例えば、ベースカラーとHeightのディテールなど）。

+++

+++シェーダ設定の調整
UltraでのSpecular品質により、より正確な結果が得られますが、この設定にはコストがかかります。 シェーダで一度に有効にするエフェクトの数が多いほど、計算が重くなります。 可能な限り、複雑なマテリアルを別のシェーダで別のテクスチャセットに分割してください。 ディスプレイスメントが有効になっている場合は、テッセレーションパラメータに注意してください。

+++

+++ファイルオプションを調整
<b>ファイル/保存/保存してファイルを減らす</b>を使用 <b>不要なデータをフラッシュし、<b>未使用のリソースを削除</b>して、プロジェクト内で使用されていないファイルをプロジェクトにインポートして削除します。</b>

+++
