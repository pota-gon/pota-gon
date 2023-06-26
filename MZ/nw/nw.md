# RPGツクールMZで NW.js が残り続ける問題の解決方法
RPGツクールMZ でゲーム開発していると、時々重くなることがあります。  
タスクマネージャーを開いてみると大量の NW.js が起動したままとなっています。

NW.js のバージョンが原因と推測されるため、  
NW.js の差し替え方法について説明します。

|RPGツクールMZバージョン|NW.jsバージョン|報告されている問題|
|---|---|---|
|1.0.0 ～ 1.1.1|0.44.5|(1) M1チップ搭載のMac機種にて強制終了する<br>(2) Big Surにて画面が表示されなくなる|
|1.2.0|0.51.0|NW.js が残り続ける|
|1.2.1 ～ 1.5.0|0.48.4|NW.js が残り続ける|
|1.6.0|0.69.1|一部の環境で「テストプレイ」「バトルテスト」「デプロイメントしたアプリ」が起動しない<br>・macOS10.15以前(node.js v18.10.0 になったことが原因)|
|1.6.1 ～ 1.7.0|0.48.4|NW.js が残り続ける|

以下、目次から確認したい項目を選択してください

|目次|備考|
|---|---|
|[NW.jsを最新版へ差し替え](#nwjsを最新版へ差し替え)|最新版に差し替えたい場合、こちらを確認してください。|
|[NW.jsを旧バージョンに差し替え](#nwjsを旧バージョンに差し替え)|NW.js が残り続ける問題が発生する前のバージョンに差し替える方法を説明します。|
|[プロフィールエラーの解消について](#プロフィールエラーの解消について)|差し替え後、エラーが出る場合確認してください。|

---

## NW.jsを最新版へ差し替え
NW.jsを最新版へ差し替える方法を説明します。

### 1. NW.js のダウンロードサイトへアクセス
下記URLにアクセスします。  
https://nwjs.io/downloads/

### 2.『SDK』を選択
『SDK』を選択してください。  
※ Mac の場合は、「Mac OS X 64-bit」 の横にある『SDK』を選択してください。

<img src="nw.png" width="75%">

### 3. 差し替えるフォルダをバックアップ
以下のフォルダをバックアップしておいてください。  
もし、忘れた場合でも再度、RPGツクールMZ を再インストールすれば、元に戻せます。

* ストア版: C:\Program Files\KADOKAWA\RPGMZ\nwjs-win
* Steam版: C:\Program Files (x86)\Steam\steamapps\common\RPG Maker MZ\nwjs-win  
※ Mac は、同じ階層にある nwjs-mac を差し替えてください。

### 4. ダウンロードしたZIPファイルを解凍
ダウンロードしたZIPファイルを解凍します。

### 5. 解凍したフォルダ名称を変更します
解凍したフォルダ名称を以下のように変更してください。

* Windows: 『nwjs-sdk-v0.59.0-win-x64』 => nwjs-win
* Mac: 『nwjs-sdk-v0.59.0-osx-x64』 => nwjs-mac

### 6. フォルダを差し替え
以下のフォルダを差し替えてください。これで完了です。

* ストア版: C:\Program Files\KADOKAWA\RPGMZ\nwjs-win
* Steam版: C:\Program Files (x86)\Steam\steamapps\common\RPG Maker MZ\nwjs-win  
※ Mac は、同じ階層にある nwjs-mac を差し替えてください。

---

## NW.jsを旧バージョンに差し替え
ここでは、NW.js が残り続ける問題のなかった 『0.44.5』への差し替え方法を説明します。

### 1. NW.js のダウンロードサイトへアクセス
下記URLにアクセスします。  
https://nwjs.io/downloads/

### 2.『Previous releases』を選択
『Previous releases』を選択してください。  
<img src="nw_old.png" width="75%">

### 3. 『v0.44.5』を選択
『v0.44.5』を選択してください。

![](before.png)

### 4. 以下ファイルをダウンロード
* Windows:『nwjs-sdk-v0.44.5-win-x64.zip』
* Mac:『nwjs-sdk-v0.44.5-osx-x64.zip』

### 5. 差し替えるフォルダをバックアップ
以下のフォルダをバックアップしておいてください。  
もし、忘れた場合でも再度、RPGツクールMZ を再インストールすれば、元に戻せます。

* ストア版: C:\Program Files\KADOKAWA\RPGMZ\nwjs-win
* Steam版: C:\Program Files (x86)\Steam\steamapps\common\RPG Maker MZ\nwjs-win  
※ Mac は、同じ階層にある nwjs-mac を差し替えてください。

### 6. ダウンロードしたZIPファイルを解凍
ダウンロードしたZIPファイルを解凍します。

### 7. 解凍したフォルダ名称を変更します
解凍したフォルダ名称を以下のように変更してください。

* Windows: 『nwjs-sdk-v0.44.5-win-x64』 => nwjs-win
* Mac: 『nwjs-sdk-v0.44.5-osx-x64』 => nwjs-mac

### 8. フォルダを差し替え
以下のフォルダを差し替えてください。これで完了です。

* ストア版: C:\Program Files\KADOKAWA\RPGMZ\nwjs-win
* Steam版: C:\Program Files (x86)\Steam\steamapps\common\RPG Maker MZ\nwjs-win  
※ Mac は、同じ階層にある nwjs-mac を差し替えてください。

---

## プロフィールエラーの解消について
テストプレイ時に 『プロフィールエラーが発生しました。』 が出る場合は、以下フォルダを削除してください。  
※ ユーザ名は、パソコンの設定内容によって異なるので、適宜変更してください。

C:\Users\ユーザ名\AppData\Local\rmmz-game
