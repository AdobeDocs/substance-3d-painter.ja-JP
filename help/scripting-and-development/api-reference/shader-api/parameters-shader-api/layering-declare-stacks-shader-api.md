---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-declare-stacks-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painterのレイヤーのスタックを宣言シェーダー APIリファレンスにアクセスして、マテリアルのレイヤリングスタックをカスタマイズします。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Declare Stacks - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: レイヤーのスタックの宣言 – シェーダー API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---


# レイヤーのスタックの宣言 – シェーダー API

## マテリアルレイヤー：編集可能なスタックを宣言

編集可能なスタックは、一意の識別子と文書チャネルのリストによって定義されます。 考えられるチャンネルID: *ambientocclusion* *anisotropyangle* *anisotropylevel* *basecolor* *blendingmask* *diffuse* *ディスプレイスメント* *放射性* *光沢性* *Height* *ior* *メタリック* *normal* *不透明度* *リフレクション* *粗さ* *散布* *Specular* *specularlevel* *透過型* *user0* *user1* *user2* *user3* *user4*&#x200B;ユーザー5 **&#x200B;ユーザー6 **&#x200B;ユーザー7 **

例：

```
//:  stacks [ 

//:    { 

//:      "id": "Mask1", 

//:      "channels": [ 

//:        {"id": "opacity"} 

//:      ] 

//:    }, { 

//:      "id": "Mask2", 

//:      "channels": [ 

//:        {"id": "opacity"}, 

//:        {"id": "user0"} 

//:      ] 

//:    } 

//:  ]
```


スタックのチャンネルをサンプラーパラメーターにバインドするには、チャンネルタグにスタック識別子の接頭辞を付けます。

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
