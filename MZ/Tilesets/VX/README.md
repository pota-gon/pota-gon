# MZ に VX と VXAce のタイルセットを追加する設定

## 手順
MZ に VX と VXAceのタイルセット設定を追加した Tilesets.json です。  
下記、手順を実施することで VXAce 用のタイルセットを追加できます。

1. 『Tilesets.json』 をダウンロード  
https://raw.githubusercontent.com/pota-gon/pota-gon/main/MZ/Tilesets/VX/Tilesets.json

2. ダウンロードした 『Tilesets.json』 を MZ のプロジェクト の 「data」 フォルダに配置  
※ タイルセットの設定を上書きするので、新規プロジェクトでの実施をおすすめします。

3. VXAce の RTPの 「C:/Program Files (x86)/Common Files/Enterbrain/RGSS3/RPGVXAce/Graphics/Tilesets」 を『tilesets』としてコピーし、MZプロジェクトの「img/tilesets」と差し替え

4. VX の RTPの 「C:/Program Files (x86)/Common Files/Enterbrain/RGSS2/RPGVX/Graphics/System」の 『TileA1.png ～ TileD.png』 までを MZプロジェクトの「img/tilesets」に配置

5. MZ プロジェクトを開き、データベース > システム2 を開き、タイルサイズを『32x32』に変更

※ 作成に使用した Tilesets.rvdata2  は [こちら](https://github.com/pota-gon/pota-gon/blob/main/MZ/Tilesets/VX/Tilesets.rvdata2?raw=true) からダウンロードできます。

## 素材集などの移行方法

素材集とかの設定を追加したい場合は、以下を使うとおすすめです。

・VX => VXAce(VX 用のマップタイルを VX Ace で使う | RPGツクールVX Ace 初心者向け講座)  
https://tkool.jp/products/rpgvxace/lecture/004_009c/

・VXAce => MZ(Ace to MV Converter - Ace to MV Converter.rb)  
https://plugin.fungamemake.com/archives/10014  
※ 備考：準公式プラグインは、私は以下にありました。見当たらない人は以下も探してみてください。  
C:/Program Files (x86)/Steam/steamapps/common/RPG Maker MV/dlc/RPGmakerWeb_plugins/Shaz
