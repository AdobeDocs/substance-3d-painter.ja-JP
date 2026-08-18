---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-the-shelf-preferences-with-python.html"
breadcrumb-title: ''
description: Substance 3D PainterでPythonスクリプティングを使用してシェルフの環境設定を編集し、リソースパスの自動管理を行う方法について説明します。
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Edit Shelf Preferences with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pythonでシェルフの環境設定を編集する
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 2%

---


# Pythonでシェルフのプリファレンスを編集する

リソースパスを操作するためにWindowsレジストリを変更するPythonスクリプトの例を次に示します。

## レジストリキーパス

適切なレジストリキーパスを使用するには、次の表を参照してください。

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>システム</th> <th>バージョン</th> <th>パス</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>（登記簿）</p></td> <td><strong>7.2</strong>以降</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>レガシー</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>（図書館）</p></td> <td><strong>7.2</strong>以降</td> <td>/Users/[ユーザー名]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>レガシー</td> <td>/Users/[ユーザー名]/Library/Preferences/com.substance3d.user.plist</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td><strong>7.2</strong>以降</td> <td>/home/[ユーザー名]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>レガシー</td> <td>/home/[ユーザー名]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## 新しいパスの追加

リソースパスを追加するには、リストを新しいパスで増やすために、既存のパスを確認する必要があります。

次のコードでは、定義済みのパスの現在の数を確認した後、新しいシェルフパスをレジストリキーに追加します。

>[!NOTE]
>
> サブキー&#x200B;**Shelf** （**pathInfos**&#x200B;と一緒に）がレジストリに存在しない可能性があります。 アプリケーションの起動に表示されるようにするには、環境設定（編集/設定）を開き、「 OK 」をクリックしてアプリケーションを閉じます。

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

 

ShelfName = "myshelf" #Needs to be lowercase 

ShelfPath = "C:/Temp" 

ShelfStatus = "false" #false = not disabled 

 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

  

## Open parent registry key

Key = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ  ) 

 

## Iterate over each sub-key to retrieve the biggest Shelf number

SubKeyCount = winreg.QueryInfoKey( Key )[0] 

ShelfNumber = 0 

 

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 ShelfNumber = max( ShelfNumber, int(SubKeyName) ) 

 

ShelfNumber += 1 

 

## Create the new Key and add its values

NewKey = winreg.CreateKey( Key, str( ShelfNumber ) ) 

 

winreg.SetValueEx( NewKey, "disabled", 0, winreg.REG_SZ, ShelfStatus) 

winreg.SetValueEx( NewKey, "name", 0, winreg.REG_SZ, ShelfName) 

winreg.SetValueEx( NewKey, "path", 0, winreg.REG_SZ, ShelfPath) 

 

NewKey.Close() 

 

## Increment the Shelf path counter

Count = winreg.QueryValueEx( Key, "size" ) 

Key.Close() 

 

Key = winreg.OpenKeyEx( RegConnection, RegistryKeyName, 0, winreg.KEY_SET_VALUE  ) 

winreg.SetValueEx( Key, "size", 0, winreg.REG_DWORD, Count[0] + 1 ) 

Key.Close()
```


## リソースパスの無効化または有効化

作成されたパスは、不要になった時点で削除できますが、完全に削除できないデフォルトのパスに対しても無効にすることができます。

次のコードでは、Windowsレジストリを解析し、デフォルトのシェルフ（「starter\_assets」という名前）を無効にします。

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

 

## Open registry key

Key    = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ ) 

SubKeyCount  = winreg.QueryInfoKey( Key )[0] 

 

## Iterate over each sub-key

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 SubKey = winreg.OpenKey( 

  RegConnection, 

  RegistryKeyName + "\" + SubKeyName, 

  winreg.KEY_READ ) 

 SubKeyValueCount = winreg.QueryInfoKey( SubKey )[1] 

 

## Read subkey values

 Values = [] 

 for i in range( SubKeyValueCount ) : 

  Values.append( winreg.EnumValue( SubKey, i ) ) 

 

## Note : Values is a table of tuples

 FoundKey = False 

 for Value in Values : 

  if Value[0] == "name" : 

   if Value[1] == "starter_assets" : 

    FoundKey = True 

 

 SubKey.Close() 

 

## Found the path ? Then we edit the Key

 if FoundKey : 

  print( " - Editing Windows Registry" ) 

 

## Re-Open key in edition mode

  SubKey  = winreg.OpenKey(   

   winreg.HKEY_CURRENT_USER, 

   RegistryKeyName + "\" + SubKeyName, 

   0, 

   winreg.KEY_SET_VALUE ) 

 

## Assign new value

  winreg.SetValueEx(SubKey, "disabled", 0, 1, "true" ) #use "false" to Enable that shelf path 

 

  SubKey.Close() 

 

## Finish

Key.Close()
```
