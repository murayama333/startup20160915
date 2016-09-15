# Webサイト公開編

# 2 Linuxプログラミング

クラウドサーバに接続できたので、コマンドをいくつか実行してみましょう。

## 2.1 よく使うLinuxコマンド

Linuxはすべての操作をコマンドで処理します。ファイルやフォルダをつくるのもすべてコマンドで処理します。

### pwd カレントフォルダの表示

カレントフォルダとは現在、開いているフォルダのことです。

```
pwd
```

### cd カレントフォルダの移動

```
cd /home/ubuntu
```

### mkdir フォルダの作成


```
mkdir sample
```

### ls カレントフォルダの閲覧

```
ls
```

### echo メッセージの表示

```
echo Hello World
```

次のように入力するとメッセージをファイルに保存できます。

```
echo Hello World > hello.txt
```

### cat ファイルの表示

```
cat sample.txt
```

> Linuxにはviエディタというソフトが標準でインストールされています。viエディタはviコマンドで起動できます。（参考） http://net-newbie.com/linux/commands/vi.html


## 2.2 Webサーバのインストール

続いてWebページを配信するために、Webサーバをインストールしてみます。Webサーバ製品もいくつかありますが、ここでは世界中で最もよく利用されているApacheを利用します。

### クラウドサーバを最新化

クラウド上に作成してすぐのサーバは最新の状態になっていないので、以下のコマンドを使ってサーバの利用するソフトウェアを最新にしておきます。

```
sudo apt-get update -y
```


### Webサーバ（Apache）のインストール

サーバ上にApacheをインストールします。Apacheは世界で最も使われているWebサーバープロダクトです。

```
sudo apt-get install apache2
```

#### Apacheの起動と停止

Apacheは以下のコマンドで起動できます。

```
sudo service apache2 start
```

停止するときは以下のようにコマンドを実行します。

```
sudo service apache2 stop
```

### 2.3 HTMLファイルのアップロード

手元のパソコンから、クラウド上にあるサーバにHTMLファイルをアップロードします。

#### Macユーザの場合

Desktop上のsample.htmlをアップロードする場合

```
scp /Users/murayama/Desktop/sample.html ubuntu@52.79.97.23
```

#### Windowsユーザの場合

起動中のTeraTermにアップロードしたいファイルをドラッグアンドドロップします。


### 2.4 Apacheの公開フォルダにHTMLファイルをコピー

```
sudo cp /home/ubuntu/sample.html /var/www/html
```

以上でLinuxサーバのセットアップは完了です。

### 2.5 動作確認

ブラウザを開いて、以下のURLにアクセスしてみましょう。

```
http://52.79.97.23/sample.html
```

作成したHTMLファイルを閲覧できればプログラミングは終了です。

> 手元のスマートフォンからHTMLファイルを見ることもできます。
