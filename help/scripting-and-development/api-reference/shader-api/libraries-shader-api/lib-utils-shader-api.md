---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-utils-shader-api.html"
breadcrumb-title: ''
description: Substance 3D PainterのLib Utils シェーダー APIリファレンスにアクセスして、カスタムシェーダ開発でユーティリティ機能を使用します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Utils - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ライブラリユーティリティ – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 1%

---


# ライブラリユーティリティ – シェーダー API

## アルゴリズムのユーティリティ関数

## トーンマッピング

シェーダで使用できるトーンマッピングの例を次に示します。 Painterでは、Yebisによって適用されたオプションのトーンマッピング以外、トーンマッピングは適用されません。 シェーダでトーンマッピングを行う場合は、Yebisトーンマッピングの前に適用されます。

sigmaおよびnパラメーターに基づいて、Sカーブのトーンマッピングを実行します。

```
vec3 tonemapSCurve(vec3 value, float sigma, float n) 

{ 

  vec3 pow_value = pow(value, vec3(n)); 

  return pow_value / (pow_value + pow(sigma, n)); 

}
```


## sRGB変換

Painterで使用される変換結果です。 次の行をカスタムシェーダに入れることで、ビューポートの自動リニア – > sRGB変換をオーバーライドできます。

*#define DISABLE\_FRAMEBUFFER\_SRGB\_CONVERSION*

独自のカスタム変換を実行できます。

sRGBからリニアカラーへの変換。 スカラーバージョン。

```
float sRGB2linear(float x) 

{ 

  return x <= 0.04045 ? 

    x * 0.0773993808 : // 1.0/12.92 

    pow((x + 0.055) / 1.055, 2.4); 

}
```


sRGBからリニアカラーへの変換。 RGBバージョン。

```
vec3 sRGB2linear(vec3 rgb) 

{ 

  return vec3( 

    sRGB2linear(rgb.r), 

    sRGB2linear(rgb.g), 

    sRGB2linear(rgb.b)); 

}
```


sRGBからリニアカラーへの変換。 RGB + Alpha版

```
vec4 sRGB2linear(vec4 rgba) 

{ 

  return vec4(sRGB2linear(rgba.rgb), rgba.a); 

}
```


リニアからsRGBカラーへの変換。 スカラーバージョン。

```
float linear2sRGB(float x) 

{ 

  return x <= 0.0031308 ? 

      12.92 * x : 

      1.055 * pow(x, 0.41666) - 0.055; 

}
```


リニアからsRGBカラーへの変換。 RGBバージョン。

```
vec3 linear2sRGB(vec3 rgb) 

{ 

  return vec3( 

      linear2sRGB(rgb.r), 

      linear2sRGB(rgb.g), 

      linear2sRGB(rgb.b)); 

}
```


リニアからsRGBカラーへの変換。 RGB + Alpha版

```
vec4 linear2sRGB(vec4 rgba) 

{ 

  return vec4(linear2sRGB(rgba.rgb), rgba.a); 

}
```


リニアからsRGBへのカラー変換はオプションです。 スカラーバージョン。

```
//: param auto conversion_linear_to_srgb 

uniform bool convert_to_srgb_opt; 

float linear2sRGBOpt(float x) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(x) : x; 

}
```


リニアからsRGBへのカラー変換はオプションです。 RGBバージョン。

```
vec3 linear2sRGBOpt(vec3 rgb) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgb) : rgb; 

}
```


リニアからsRGBへのカラー変換はオプションです。 RGB + Alpha版

```
vec4 linear2sRGBOpt(vec4 rgba) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgba) : rgba; 

}
```


カラー変換： スカラーバージョン。

```
uniform int output_conversion_method; 

float convertOutput(float x) 

{ 

 if (output_conversion_method == 0) return x; 

 else if (output_conversion_method == 1) return linear2sRGB(x); 

 else return sRGB2linear(x); 

}
```


カラー変換： RGBバージョン。

```
vec3 convertOutput(vec3 rgb) 

{ 

 if (output_conversion_method == 0) return rgb; 

 else if (output_conversion_method == 1) return linear2sRGB(rgb); 

 else return sRGB2linear(rgb); 

}
```


カラー変換： RGB + Alpha版

```
vec4 convertOutput(vec4 rgba) 

{ 

 if (output_conversion_method == 0) return rgba; 

 else if (output_conversion_method == 1) return linear2sRGB(rgba); 

 else return sRGB2linear(rgba); 

}
```


## ディザリング

シェーダにディザリングを追加するためのヘルパーです。

8 x 8ベイヤー行列を使用したディザリングモード

```
import lib-bayer.glsl 

 

float getDitherThreshold(uvec2 coords) 

{ 

  return bayerMatrix8(coords); 

} 

 

 

vec4 RGB2Gray(vec4 rgba) 

{ 

  float gray = 0.299 * rgba.r + 0.587 * rgba.g + 0.114 * rgba.b; 

  return vec4(vec3(gray), rgba.a); 

}
```


光沢のある金属表面（鏡に近い部分）のAOおよびシャドウを除去

```
float specularOcclusionCorrection(float diffuseOcclusion, float metallic, float roughness) 

{ 

  return mix(diffuseOcclusion, 1.0, metallic * (1.0 - roughness) * (1.0 - roughness)); 

} 

 
```
