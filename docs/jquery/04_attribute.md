&nbsp; &nbsp;
marp: true
&nbsp; &nbsp;


# 属性 attribute


&nbsp; &nbsp;

## 属性とは


```
<img src="main.jpg" alt="メイン画像">
```
* `src`属性
* `alt`属性

> `src`属性の値が`main.jpg`、`alt `属性の値が`メイン画像`

&nbsp; &nbsp;


## attr 属性値の変更


&nbsp; &nbsp;

```
attr('属性名','値');
```
attrの中に属性名と値を入れると属性値を変更できる

&nbsp; &nbsp;-



index.html

```
<div class="main">
   <img src="main.jpg" alt="メイン画像">
</div>
```

script.js
```
$('.main').find('img').attr('src','sub.jpg');
// src属性のmain.jpgをsub.jpgに変更できる
```
&nbsp; &nbsp;


## HTMLタグのクラス変更


&nbsp; &nbsp;


### addClass

HTMLタグにクラスを付与する

```
addClass('クラス名');
```

&nbsp; &nbsp;

html
```
<ul class="tab-menu">
   <li>Get Started</li>
   <li>Tutorial</li>
   <li>Guidelines</li>
</ul>
```

js
```
$('.tab-menu li').on('click', function () {
   $(this).addClass('active');
});
```


&nbsp; &nbsp;

### liタグをクリックすると


html
```
<ul class="tab-menu">
   <li class="active">Get Started</li>
   <li>Tutorial</li>
   <li>Guidelines</li>
</ul>
```
**class="active"** が追加される


&nbsp; &nbsp;

### removeClass

HTMLタグからクラスを削除する

```
removeClass('クラス名');
```


&nbsp; &nbsp;

### toggleClass

HTMLタグからクラスを付与と削除を交互に行う

```
toggleClass('クラス名');
```

&nbsp; &nbsp;


