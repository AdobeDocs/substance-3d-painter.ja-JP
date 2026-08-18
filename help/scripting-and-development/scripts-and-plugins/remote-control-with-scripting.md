---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-painter/scripting-and-development/scripts-and-plugins/remote-control-with-scripting.html"
breadcrumb-title: ''
description: Substance 3D Painterのリモートコントロールスクリプティングを使用して、ワークフローを自動化し、プログラムによりアプリケーションを制御する方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Remote control with scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: スクリプトによるリモートコントロール
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# スクリプトによるリモートコントロール

このページでは、JavascriptまたはPythonコマンドを実行するために、アプリケーションをリモートで制御する方法について説明します。\
これには特別なコマンドライン引数が必要で、単純なPythonスクリプトで既存のJavascriptやPython APIから使用できるコマンドを実行できます。

## アプリケーションの起動

アプリケーションをリモートで制御するには、Substance 3D Painterを次のコマンドラインで起動する必要があります。

```
"Adobe Substance 3D painter.exe" --enable-remote-scripting
```


>[!NOTE]
>
> スクリプトを実行する前に、このコマンドを使用してアプリケーションが起動および実行されていることを確認してください。 アプリケーションがまだ起動中であるか、まだ準備ができていない場合は、スクリプトが失敗することがあります。

## リモート制御スクリプト

次のPythonスクリプトは、アプリケーションと通信するためのライブラリとして使用できます。

以下のスクリプトを&#x200B;**lib\_remote.py**&#x200B;という名前のファイルに保存して、以下の例が正しく動作するようにします。

```
import sys 

import json 

import base64 

import subprocess 

 

if sys.version_info >= (3, 0): 

 import http.client as http 

else: 

 import httplib as http 

 

class RemotePainter() : 

 def __init__(self, port=60041, host='localhost'): 

  self._host = host 

  self._port = port 

 

## Json server connection

  self._PAINTER_ROUTE = '/run.json' 

  self._HEADERS = {'Content-type': 'application/json', 'Accept': 'application/json'} 

 

## Execute a HTTP POST request to the Substance Painter server and send/receive JSON data

 def _jsonPostRequest( self, route, body, type ) : 

  connection = http.HTTPConnection(self._host, self._port, timeout=3600) 

  connection.request('POST', route, body, self._HEADERS) 

  response = connection.getresponse() 

 

  data = response.read() 

  connection.close() 

 

  if type == "js" : 

   data = json.loads( data.decode('utf-8') ) 

 

   if 'error' in data: 

    OutJson = json.loads( body.decode() ) 

    print( base64.b64decode( OutJson["js"] ) ) 

    raise ExecuteScriptError(data['error']) 

  else : 

## Python can return nothing, so decoding can fail

   try: 

    data = data.decode('utf-8').rstrip() 

   except: 

    pass 

 

  return data 

 

 def checkConnection(self): 

  connection = http.HTTPConnection(self._host, self._port) 

  connection.connect() 

 

## Execute a command

 def execScript( self, script, type ) : 

  Command = base64.b64encode( script.encode('utf-8') ) 

 

  if type == "js" : 

   Command = '{{"js":"{0}"}}'.format( Command.decode('utf-8') ) 

  else : 

   Command = '{{"python":"{0}"}}'.format( Command.decode('utf-8') ) 

 

  Command = Command.encode( "utf-8" ) 

 

  return self._jsonPostRequest( self._PAINTER_ROUTE, Command, type ) 

 

class PainterError(Exception): 

 def __init__(self, message): 

  super(PainterError, self).__init__(message) 

 

class ExecuteScriptError(PainterError): 

 def __init__(self, data): 

  super(PainterError, self).__init__('An error occured when executing script: {0}'.format(data)) 

 
```


## 例

以下に、アプリケーションでサポートされている両方のAPIでコマンドを実行する方法を示す2つの簡単な例を示します。

### Javascriptコマンドの実行

APIのほとんどのJavascript関数は、Pythonスクリプト内での操作を容易にする文字列またはJsonデータを返します。 データの送受信に大きな問題はないはずです。

**example\_js.py**&#x200B;という名前のpythonスクリプトファイルを作成し、次のコードを追加します。

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## Print the API version

Version = Remote.execScript( "alg.version.painter", "js" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library:

Files = Remote.execScript( 'alg.resources.findResources("starter_assets", "*")', "js" ) 

 

for File in Files : 

 print( File )
```


アプリケーションがコマンドラインで実行されている場合、このスクリプトを実行すると、コマンドが実行され、その結果が取得されます。

### Pythonコマンドの実行

ほとんどのPython関数は、リモートスクリプトに渡すことのできないオブジェクトを返します。つまり、データを受け取るためには、文字列やJson辞書に明示的に変換する必要があります。

より簡単に行うには、アプリケーションの起動時にロードされるカスタムPythonスクリプトを作成し、インライン変換に依存しなくてもこのような変換を処理する関数を呼び出すことができます。

**example\_py.py**&#x200B;という名前のpythonスクリプトファイルを作成し、次のコードを追加します。

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## import the substance_painter module to make

## its API available to us

Remote.execScript( "import substance_painter", "python" ) 

 

## Print the API version

Version = Remote.execScript( "substance_painter.__version__", "python" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library

## Because the search function return objects, we have to convert

## the information into a string within the same command (inline)

Command = 'substance_painter.resource.search( "p:starter_assets/" )' 

Command = '"|||".join( [ x.identifier().url() for x in {0}] )'.format( Command ) 

 

Files = Remote.execScript( Command, "python" ) 

Files = Files.split( "|||" ) 

 

for File in Files : 

 print( File )
```


アプリケーションがコマンドラインで実行されている場合、このスクリプトを実行すると、コマンドが実行され、その結果が取得されます。
