&nbsp; &nbsp;
marp: true
&nbsp; &nbsp;


# jQuery セレクタ

JavaScriptからHTMLにアクセスする


&nbsp; &nbsp;-

## HTMLタグ / id / classの取得

&nbsp; &nbsp;

index.html

```
<h1>ドリンクメニュー</h1>
<h2 id="title">本日のコーヒー</h2>
<p class="type">ホット</p>
```
script.js

```
$('h1'); //h1タグを取得
$('#title'); //h2タグを取得
$('.type'); //pタグを取得
```
> '$' はjQueryの略

&nbsp; &nbsp;

## 親要素から子要素の取得

&nbsp; &nbsp;


#### index.html

```
<div class="container">
    <p>本日のコーヒー</p>
</div>
```
#### script.js

```
$('.container p');  //.containerの中の`p`タグ
```
> 半角スペースで子要素にアクセスする


&nbsp; &nbsp;

## find

#### script.js

```
$('.container).find('p');  //.containerの中の#title
```
> .find()で子要素を探す


&nbsp; &nbsp;


## CSSの操作


&nbsp; &nbsp;

`css()` の命令でCSSのプロパティを扱うことができる

index.html

```
<h1>ドリンクメニュー</h1>
<h2 id="title">本日のコーヒー</h2>
<p class="type">ホット</p>
```
script.js
```
$('h1').css('color','#FF0000'); //文字色の変更
$('#title').css('background-color','#EFEFEF'); //背景色の変更
$('.type').css({
    'fonnt-size':'15px',
    'color':'#00FF00',
    'background-color','#EFEFEF'
});
```

&nbsp; &nbsp;

### liの適用

index.html

```
<ul id="menu">
    <li>ブレンドコーヒー</li>
    <li>カプチーノ</li>
    <li>カフェラテ</li>
    <li>キャラメル マキアート</li>
</ul>
```
script.js

```
//（0から数えて）2番目の文字色を変更
$('#menu li').eq(2).css('color', '#00FF00');
```

&nbsp; &nbsp;
