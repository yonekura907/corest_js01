&nbsp; &nbsp;
marp: true
&nbsp; &nbsp;



# jQuery

&nbsp; &nbsp;

## jQueryとは


&nbsp; &nbsp;


[https://jquery.com/](https://jquery.com/)

JavaScriptの構文を簡略化して、CSS風に記述することができるライブラリ

![](img/jq01.png)


&nbsp; &nbsp;

## jQueryのダウンロード方法1

&nbsp; &nbsp;

[https://jquery.com/download/](https://jquery.com/download/)

![](img/jq_download.png)

&nbsp; &nbsp;

### 右クリックで「リンク先を別名で保存」

&nbsp;

![](img/jq_download2.png)

jsフォルダを作成してダウンロードしたファイルを保存する

&nbsp; &nbsp;

### HTMLにjQueryを読み込む

#### index.html

```
<footer/>

<script src="js/jquery-3.4.1.min.js"></script>
</body>
</html>

```

`body`の閉じタグの前に`script`タグを作成して読み込む

&nbsp; &nbsp;


## jQueryのダウンロード方法2

&nbsp; &nbsp;

### HTMLにjquery.comからサーバー経由でjQueryを読み込む

#### index.html


```
<footer/>

<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
</body>
</html>

```

`body`の閉じタグの前に`script`タグを作成して`https:~`から読み込む

> インターネットに接続していないと使用できない。

&nbsp; &nbsp;


## JavaScriptの記述場所

&nbsp; &nbsp;

### jsファイルを新規作成

![](img/jq_download3.png)


&nbsp; &nbsp;

### 新規jsファイルの読み込み方

```
<footer/>
<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
<script src="js/script.js"></script>
</body>
</html>

```
> ライブラリ（jQuery）の読み込みが先。自分のソースが後

&nbsp; &nbsp;



## jQueryの書き方


&nbsp; &nbsp;

### jQueryの記述パターンはこの3つ

1. HTMLの読み込み待ち　read
2. HTMLの操作 selector
3. イベントの扱い　on


&nbsp; &nbsp;

## 1 HTMLの読み込み待ち ready

&nbsp; &nbsp;

JavaScriptを実行する場合、ブラウザがHTMLタグを読み込み終えてから処理を始めないと、操作対象が見つからなくなる。

##### script.js

```
jQuery(document).ready(function(){
  //HTMLの読み込みが終わるとこの中が実行される
});

```

&nbsp; &nbsp;

### readyの短い書き方

##### script.js

```
$(function(){
  //HTMLの読み込みが終わるとこの中が実行される
});

```

> '$' は jQueryの略称

&nbsp; &nbsp;

