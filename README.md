## アドオン概要
  
コマンドでチャット検知をしたい、、    
   
統合版コマンダーはそう願っていた(?)    
  
そんな夢を叶えてくれるのがChatTagAddon！  
  
これを使えばtag指定でチャット検知が可能になります。  
  
## 導入
  
「ベータ API」をオンにしてワールドにアドオンを入れるだけで使えます。  
  
## 仕様
  
チャットを送信するとchat_メッセージというtagが付きます。  
  
例:こんにちは と送信するとchat_こんにちは というtagが付きます  
  
このtagはチャットをする度に外され新たなtagが付きます。  
  
## 使用例
  
### ?lobbyと打つとtpするコマンド  

tp @a[tag="chat_?lobby"] 座標  

tag @a[tag="chat_?lobby"] remove "chat_?lobby"  
  
?messageと打つとメッセージが表示されるコマンド  
  
tellraw @a[tag="chat_?message"] {"rawtext":[{"text":"メッセージ"}]}  
  
tag @a[tag="chat_?message"] remove "chat_?message"  
  
## 注意点
  
・「ベータ API」をオンにしてください  
  
・特定の条件でアドオンが動かない場合があるそうです(現在条件を調査中)  
  
改造・二次配布について  
  
改造は自由です。二次配布は改造したものならokですが、そのまま二次配布するのはおやめください。  
動画などで紹介してもらえると飛んで喜びます。  

## 追記
  
windows版で動作しない場合があるそうです(原因不明)  
