

#### 環境構築  
以下のコマンドを実行  
```
docker compose up -d --build
docker exec -it backend_ocr bash
cd ../../../
go run main.go
```
    
#### 使っている技術  
・go 1.22.3  
・echo  
・react  
・typescript  
・docker  
・tesseract  
・gosseract  

  
#### 作ろうと思った経緯  
家計管理アプリにあるレシート読み込み機能を使ってみてうまく読み込める時とそうでない時があり、そもそもどうやって実装するのか気になったので作成。  
画像だけでなく動画も解析したい。→ 対応予定  

  
#### 作った感想  
結論、実験程度であればかなり良いのではと思った。  
出力される結果を使いたいなら整形が必要でchatGPTなどのAIサービスで整形して使うのが一連の流れになりそう。  
他のocrエンジンとしては、Google　Cloud Vision APIやAzure Computer Visionなどがあり、調べたところGoogle Cloud Vision APIが一番精度が良さそう。  
(個人開発はできるだけ無料がいいなぁ)  

  
#### 実装動画
https://github.com/Nyakira22/ocr/assets/162646793/b86caceb-a52f-407d-a877-75ff4153d9eb
　　
  
出力されたテキストをchatGPTに食わせるといい感じにしてくれる。  
内部で解析結果をchatCGPのAPIで整形してから返却する方がより実用的  
https://github.com/Nyakira22/ocr/assets/162646793/91fa7952-8101-41b1-a321-ecd50af0f004

