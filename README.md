![Screenshot 1](https://github.com/downloads/novi/LTCoreText/ss1-s.png)

![Screenshot 2](https://github.com/downloads/novi/LTCoreText/ss2.png)

## できる Can Do

* それなりに軽量
* ページング Pagination
* 段組み
* 縦置き/縦書き (iOS 4.3以降)
* 均等揃え
* ハイフネーション(ハイフネーションライブラリが必要)
* カスタムビュー等の埋め込み
* レイアウトモード、ページ送り方向(横・逆方向・縦)
* 動的なページ挿入・削除
* 非同期レイアウト処理
* iOS 4以降対応 iOS 4 and up.

## できない Cannot Do

* `NSAttributedString` の作成 (デモAppでは [DTCoreText](https://github.com/Cocoanetics/DTCoreText) を使用) 
* 動的なフレームサイズの変更
* ルビ
    * ただし、カスタムビューでルビ用のラベルを貼り付けることは可能 (MainViewController参照)
    * デモとして赤い文字で出ます
* リンク等のイベント処理
    * カスタムビューを作成すれば可能
* テキスト選択
* GCD完全対応 (ViewのAPIにはメインキューでアクセスすること)
* デモアプリのiPhone対応(このライブラリ自体は対応)

## 使いかた Usage

デモを実行するには [DTCoreText](https://github.com/Cocoanetics/DTCoreText) が必要です。
submoduleとして入っています。

デモプロジェクトのファイルをそのままターゲットプロジェクトに追加します。
デモプロジェクトを開いたときのグループのそれぞれの役割は次の通りです。

* `Base`: ライブラリの基本 (必須)
* `Attachment/ImageView`: イメージビューの埋め込み (オプション)
* `Demo`: ライブラリの使いかたはここを参照してください。

オプションのファイル群は必要が無ければ追加しなくても動作します。

## ライセンス License
MIT

Copyright © 2011-12 Yusuke Ito

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
