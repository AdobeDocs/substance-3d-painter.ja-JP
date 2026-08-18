---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/pipeline-and-integration/configuration/querying-current-software-version.html"
breadcrumb-title: ''
description: 現在のSubstance 3D Painterソフトウェアバージョンをプログラムで照会し、パイプラインの統合と自動化を行う方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Querying Current Software Version
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 現在のソフトウェアバージョンを照会しています
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# 現在のソフトウェアバージョンを照会しています

アプリケーションの現在のバージョンの確認は、ニーズに応じて複数の方法で行うことができます（例えば、ソフトウェアを起動することなく）。

## 実行可能ファイルによるバージョンの確認

Windows上で実行可能なSubstance Painterには、外部ツール（Pythonなど）で照会できる情報がわずかしか含まれていません。

**Python 3**&#x200B;の例（[ここから取得](https://stackoverflow.com/questions/580924/python-windows-file-version-attribute)） :

```
import os 

import imp 

import pip 

import win32api #pypiwin32 

 

 


## Reader


def getFileProperties(fname): 

 """ 

 Read all properties of the given file return them as a dictionary. 

 """ 

 propNames = ('Comments', 'InternalName', 'ProductName', 

  'CompanyName', 'LegalCopyright', 'ProductVersion', 

  'FileDescription', 'LegalTrademarks', 'PrivateBuild', 

  'FileVersion', 'OriginalFilename', 'SpecialBuild') 

 

 props = {'FixedFileInfo': None, 'StringFileInfo': None, 'FileVersion': None} 

 

 try: 

## backslash as parm returns dictionary of numeric info corresponding to VS_FIXEDFILEINFO struc

  fixedInfo = win32api.GetFileVersionInfo(fname, '\') 

  props['FixedFileInfo'] = fixedInfo 

  props['FileVersion'] = "%d.%d.%d.%d" % (fixedInfo['FileVersionMS'] / 65536, 

   fixedInfo['FileVersionMS'] % 65536, fixedInfo['FileVersionLS'] / 65536, 

   fixedInfo['FileVersionLS'] % 65536) 

 

## VarFileInfoTranslation returns list of available (language, codepage)

## pairs that can be used to retreive string info. We are using only the first pair.

  lang, codepage = win32api.GetFileVersionInfo(fname, '\VarFileInfo\Translation')[0] 

 

## any other must be of the form StringfileInfo%04X%04Xparm_name, middle

## two are language/codepage pair returned from above

 

  strInfo = {} 

  for propName in propNames: 

   strInfoPath = u'\StringFileInfo\%04X%04X\%s' % (lang, codepage, propName) 

   ## print str_info 

   strInfo[propName] = win32api.GetFileVersionInfo(fname, strInfoPath) 

    

  props['StringFileInfo'] = strInfo 

 except: 

  pass 

 

 return props 

 

 


## Check exe


Path = "E:/Software/Painter/Substance Painter.exe" 

 

FileInfo = getFileProperties(Path) 

 

print( FileInfo )
```


出力されます：

```
E:SoftwarePainter>query.py 

{'FixedFileInfo': {'Signature': -17890115, 'StrucVersion': 65536, 'FileVersionMS': 132251649, 'FileVersionLS': 65536, 'ProductVersionMS': 132251649, 'ProductVersionLS': 65536, 'FileFlagsMask': 0, 'FileFlags': 0, 'FileOS': 0, 'FileType': 1, 'FileSubtype': 0, 'FileDate': None}, 'StringFileInfo': {'Comments': None, 'InternalName': 'Substance Painter', 'ProductName': 'Substance Painter', 'CompanyName': 'Allegorithmic', 'LegalCopyright': 'Copyright (C) 2017 Allegorithmic', 'ProductVersion': '2018.1.1', 'FileDescription': 'Substance Painter 2018.1.1', 'LegalTrademarks': None, 'PrivateBuild': None, 'FileVersion': '2018.1.1', 'OriginalFilename': 'Substance Painter.exe', 'SpecialBuild': None}, 'FileVersion': '2018.1.1.0'}
```


コマンドラインによるバージョンの確認

コマンドラインは次のように使用できます。 **substance painter.exe** command\_name *[オプション]*

バージョンを確認するには、**—version**、**-v**&#x200B;を使用してください。

>[!NOTE]
>
> Substance Painterのコマンドライン操作はウィンドウを出力することに注意してください。

## スクリプトによるバージョンの確認

スクリプトAPI（ヘルプメニューから利用可能）を使用すると、アプリケーションの現在のバージョンを照会できます。

詳細については、名前空間&#39;&#39;**alg**&#39;&#39;を参照してください。

例：

```
//Print current version in the log window (string) 

alg.log.info( alg.version.painter );
```
