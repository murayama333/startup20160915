# Webページ開発

## 3種の神器

+ テキストエディタ
+ Webブラウザ
+ ターミナル

## 開発の準備

デスクトップ上にst0915というフォルダを作ってください。

> 後のファイルはst0915フォルダ上に保存します。


## PART1 HTML編

### Wikipedia

> HyperText Markup Language（ハイパーテキスト マークアップ ランゲージ）、略記・略称HTML（エイチティーエムエル）とは、ウェブ上の文書を記述するためのマークアップ言語である。 文章の中に記述することでさまざまな機能を記述設定することができる。- Wikipedia


### hello.html

はじめてのHTML。

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Hello</title>
  </head>
  <body>
    <h1>Hello World</h1>
  </body>
</html>
```

> エディタは ctrl + s で保存するようにします。

コードを保存したらブラウザで表示してみましょう。


### image.html

imgタグを使って画像を表示します。

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Image</title>
  </head>
  <body>
    <img src="http://kronos.jp/img/logo.png">
  </body>
</html>
```

コードを保存したらブラウザで表示してみましょう。


### link.html

リンクを表示します。

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>link</title>
  </head>
  <body>
    <a href="http://itcaret.com/">IT CARET</a>
  </body>
</html>
```

コードを保存したらブラウザで表示してみましょう。

### list.html

リスト（箇条書き）を表示してみましょう。

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>List</title>
  </head>
  <body>
    <ul>
      <li>PHP</li>
      <li>Java</li>
      <li>JavaScript</li>
    </ul>
  </body>
</html>
```

コードを保存したらブラウザで表示してみましょう。

他にもいろんなタグがあります。HTMLクイックリファレンス など参考になります。

http://www.htmq.com/html/
