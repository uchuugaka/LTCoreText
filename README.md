![Screenshot 1](https://github.com/downloads/novi/LTCoreText/ss1-s.png)

![Screenshot 2](https://github.com/downloads/novi/LTCoreText/ss2.png)

## できる Can Do

* それなりに軽量 Light weight rendering
* ページング Pagination
* 段組み Column grouping
* 縦置き/縦書き (iOS 4.3以降) Vertical range and layout (iOS 4.3 and up)
* 均等揃え Uniform arrangement
* ハイフネーション(ハイフネーションライブラリが必要) Hyphenation (Hyphenation library required)
* カスタムビュー等の埋め込み Custom view padding
* レイアウトモード、ページ送り方向(横・逆方向・縦) Layout mode, Page (text) flow direction (horizontal, reverse, vertical) 
* 動的なページ挿入・削除 Dynamic page insertion, deletion
* 非同期レイアウト処理 Ansynchronous page laout processing
* iOS 4以降対応 iOS 4 and up.

## できない Cannot Do

* `NSAttributedString` の作成 (デモAppでは [DTCoreText](https://github.com/Cocoanetics/DTCoreText) を使用) `NSAttributedString` creation ( [DTCoreText](https://github.com/Cocoanetics/DTCoreText) is used in the demo app. )
* 動的なフレームサイズの変更 Dynamic frame resizing. 
* ルビ Ruby text
    * ただし、カスタムビューでルビ用のラベルを貼り付けることは可能 (MainViewController参照) But, labels for Ruby text can be placed in custom views (See MainViewController)
    * デモとして赤い文字で出ます Red characters appear with the demo.
* リンク等のイベント処理 Event processing such as hyperlinks.
    * カスタムビューを作成すれば可能 Available if creating custom views.
* テキスト選択 Text selection.
* GCD完全対応 (ViewのAPIにはメインキューでアクセスすること) Complete GCD support. (The main queue is accessible in the View API.)
* デモアプリのiPhone対応(このライブラリ自体は対応) Demo app supports iPhone (This library itself is supported.)

## 使いかた Usage

デモを実行するには [DTCoreText](https://github.com/Cocoanetics/DTCoreText) が必要です。Running the demo app requires  [DTCoreText](https://github.com/Cocoanetics/DTCoreText) 
submoduleとして入っています。The submodule is included.

デモプロジェクトのファイルをそのままターゲットプロジェクトに追加します。Just add the demp project files to the target project. Just add the demo project file to the target project. 
デモプロジェクトを開いたときのグループのそれぞれの役割は次の通りです。 When the demo project is opened, group are according to function.

* `Base`: ライブラリの基本 (必須) Base library. (Required)
* `Attachment/ImageView`: イメージビューの埋め込み (オプション) Image view padding (Optional)
* `Demo`: ライブラリの使いかたはここを参照してください。Please review this for library usage how-to.

オプションのファイル群は必要が無ければ追加しなくても動作します。 If optional file group is not required, it will still function without adding them.

## ライセンス License
MIT

Copyright © 2011-12 Yusuke Ito

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
