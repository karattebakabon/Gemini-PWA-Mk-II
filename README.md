# Gemini PWA Client Mk-II

[本家PWA](https://github.com/ona-oni/geminipwa/)に新たな機能を追加した自分用の改造版です。

## 追加機能
* APIエラー時の自動リトライ機能  
設定画面でこの機能がオンになっている状態で、APIが「PROHIBITED_CONTENT」などのエラーを返した場合、規定回数に達するまで自動的にリトライします。

* 校正機能  
APIが生成した文章を別のモデルで校正出来ます。デフォルトでは「gemini-2.5-flash」で読点を抑制するシスプロが入力されています。  
flash以外も指定可能ですが、flash-liteは能力不足、proは料金が高く生成時間が長いためflashが適任かと。    
読点が多くなってからオンにすることを推奨。

* 画像のサムネイル表示機能  
大きな画像を表示する場合、サムネイルで表示してクリック時に拡大表示。

## 使い方

使用方法は本家と同様です。

[index.htmlへのリンク(Github Pages)](https://kinkan04.github.io/Gemini-PWA-Mk-II/)
※このリポジトリの内容が静的にアクセスできる

1. GeminiのAPIキーを準備。
2. 上のリンクにアクセス。
3. 設定画面にGemini APIキーを設定して設定を保存。
4. チャット画面からチャット。

## Special Thanks
本家作者 ona-oni様

## Dependencies
This project uses the following third-party libraries:

*   **Marked.js:** [MIT License](https://github.com/markedjs/marked/blob/master/LICENSE.md) - Used for rendering Markdown.
