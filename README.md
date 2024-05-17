

#### 環境構築  
以下のコマンドを実行  
```
docker compose up -d --build
docker exec -it backend_ocr bash
cd ../../../
go run main.go
```
  
#### 作ろうと思った経緯  
家計管理アプリにあるレシート読み込み機能を使ってみてうまく読み込める時とそうでない時があり、そもそもどうやって実装するのか気になったので作成。  
画像だけでなく動画も解析したい。→ 対応予定  
  
#### 使っている技術  
・go 1.22.3  
・echo  
・react  
・typescript  
・docker  
・tesseract  
・gosseract

https://github.com/Nyakira22/ocr/assets/162646793/b86caceb-a52f-407d-a877-75ff4153d9eb


https://github.com/Nyakira22/ocr/assets/162646793/91fa7952-8101-41b1-a321-ecd50af0f004

