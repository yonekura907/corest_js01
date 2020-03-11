

# JavaScript

* JavaScriptの役割
* JavaScriptの記述場所
* JavaScriptの文法
* コンソール
* コメント

&nbsp; &nbsp;


## JavaScriptの役割


&nbsp; &nbsp;

### 3つとも異なる言語でやりとりが必要

![](img/js01.png)


&nbsp; &nbsp;

## JavaScriptの記述場所

1. HTML内に記述
2. 外部jsファイルに記述

&nbsp; &nbsp;

### 1. HTML内に記述

xxx.html

```
	</footer>
	<script>

    	// ここにJavaScriptを記述する

	</script>
	</body>
</html>
```

&nbsp; &nbsp;


### 2. 外部jsファイルに記述

![](img/js01@2x.png)

&nbsp; &nbsp;


## JavaScriptの文法

&nbsp; &nbsp;



### 3つの記述パターン

1. 命令式 `()`
2. 代入式 `=`
3. グループ `{}`

&nbsp; &nbsp;

## 1. 命令文

`()`

命令を出す


```
命令の名前(引数);
```


&nbsp; &nbsp;




```
jump(100);
```


![](img/js02.png)

`jump`という命令名があって、`()`の中に値を入れるとその分だけ実行


&nbsp; &nbsp;


引数とは命令に渡す値(パラメーター)

```
alert('alertのテスト');
```
* 記述は半角英数
* セミコロンが文の区切りになる


&nbsp; &nbsp;


## 2. 代入式

`=`

何らかの値を保存させる

&nbsp; &nbsp;


```
要素.属性 = 値;
```

* `=` の前後に半角スペースを入れてもOK


> プログラミングの = (イコール) は 左辺に右辺の値を保存すること


&nbsp; &nbsp;




```
document.querySelector('h1').style.color = '#FF0000';
```

&nbsp;
&nbsp;

この文を日本語に訳すと、

HTML`document`からタグ `querySelector`を取り出して、CSS`style`の文字色`color`を`#FF0000`に変更する

&nbsp; &nbsp;


### ドットシンタックス
オブジェクトと命令を .(ドット)でつなげて記述する

```
document.querySelector('h1').style.color = '#FF0000';
```


&nbsp; &nbsp;


## 3. グループ

`{}`

処理をグループにする場合に使う


```
命令(){
    処理1
    処理2
    処理3
};
```

&nbsp; &nbsp;

### `{}`の中身はインデントする習慣をつけてください

```
function setColor(){
    document.querySelector('h1').style.color = '#FF0000';
    document.querySelector('h1').style.backgroundColor = '#DDDD';
}
```


&nbsp; &nbsp;

## その他

&nbsp; &nbsp;

## コンソール

JavaScriptで書いたソースの内容を確認する方法


&nbsp; &nbsp;

### コンソールの出し方

1.ブラウザ上で右クリックして`検証`
2.`Console`タブを選択

![](img/js03.png)

&nbsp; &nbsp;

### コンソールの実行

```
console.log('読み込んだよ');
```

![](img/js04.png)

&nbsp; &nbsp;

### コンソールでエラー確認


![](img/js05.png)


エラーの場合でも確認ができる。
どのファイルの何行目がエラーか教えてくれる。

&nbsp; &nbsp;



## コメント


&nbsp; &nbsp;

### コメントの書き方

コメントとはプログラミング内に記述する「メモ書き」のようなもの

```
// 1行のコメント
```

```

/*
複数行コメント
複数行コメント
*/

```

&nbsp; &nbsp;
