---
breadcrumb-title: ""
description: Substance 3D PainterのLib Bayer シェーダー APIリファレンスにアクセスして、カスタムシェーダにベイヤディザリングパターンを作成します。
title: Lib Bayer - シェーダー API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '32'
ht-degree: 0%
---

# Lib Bayer - シェーダー API

## lib-bayer.glsl

**パブリック関数：** *bayerMatrix8*

```
float bayerMatrix8(uvec2 coords) { 

  return (float(bayer(coords.x, coords.y)) + 0.5) / 64.0; 

} 

 
```
