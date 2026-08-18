---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/command-lines.html"
breadcrumb-title: ''
description: Substance 3D Painterでコマンドライン引数を使用して、自動化、スクリプト作成、パイプライン統合を行う方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Command lines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: コマンドライン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 3%

---


# コマンドライン

このページには、アプリケーションを起動してプロジェクトを作成したり開いたりするときに使用できるコマンドラインがいくつか表示されます。\
次のコマンドラインを使用できます。

```
"Adobe Substance 3D Painter.exe" --command [option] 
```


## コマンドのリスト

| コマンド | 説明 |
| --- | --- |
| **—help** **-?** **-h** | 使用できるコマンドラインとその使用方法に関する情報を表示します。 |
| **– バージョン** **-v** | Substance 3D Painterの現在のバージョンを表示します。 |
| **– メッシュ** | プロジェクトに読み込むメッシュ。例： `// Create a new project with a specific mesh   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj"       // Update a mesh inside an existing project   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj" "E:/MyMeshFolder/Project.spp"` |
| **—mesh-map** | メッシュに関連付けられたベイク済みマップ（AO、法線、曲率）。 複数回指定できます。 命名規則： TextureSetName\_AdditionalMapSlot<ul data-preserve-html="true"> <li data-preserve-html="true">環境オクルージョン= <strong> <em> ambient_オクルージョン </em> </strong></li> <li data-preserve-html="true">曲率= <strong> <em>曲率</em> </strong></li> <li data-preserve-html="true">標準= <strong> <em> normal_base </em> </strong></li> <li data-preserve-html="true">ワールド空間の標準= <strong> <em> world_space_normals </em> </strong></li> <li data-preserve-html="true">位置= <strong> <em>位置</em> </strong></li> <li data-preserve-html="true">Thickness = <strong> <em> Thickness </em> </strong></li> <li data-preserve-html="true">ID = <em> <strong> id </strong> </em></li> </ul>例： `"Adobe Substance 3D Painter.exe" --mesh "E:/MyMeshFolder/MyMesh.obj" --mesh-map " E:/MyMeshFolder/DefaultMaterial_ambient_occlusion.png"` |
| **—udimで分割** | UDIM タイルごとのテクスチャセットを作成します。 |
| **– 書き出しパス** | プロジェクトの出力が書き出されるデフォルトの書き出しパス。 |
| **—vram-budget** | Substance 3D Painterエンジンで定義されているビデオメモリ(VRAM)の割り当てを上書きします。 「量」はメガバイト単位です。    例： `// Set the VRam budget to 2GB   "Adobe Substance 3D Painter.exe" --vram-budget 2048` |
| **– バージョン確認を無効にする** | 起動時にアプリケーションの新しいバージョンが利用可能かどうかを確認しない |
| **– リモートスクリプトを有効にする** | アプリケーションの外部からスクリプトコマンドを実行できるようにします。 詳細については、[スクリプトによるリモートコントロール](../../scripting-and-development/scripts-and-plugins/remote-control-with-scripting.md)を参照してください。 |
