&nbsp; &nbsp;
marp: true
&nbsp; &nbsp;



# 変数


&nbsp; &nbsp;

### 変数の宣言
変数とはデータの保存
固有の名前を与えて、一定期間記憶し必要なときに利用できるようにする

```
var colorValue; // 変数colorValueを宣言
```

> JavaScriptの新しいバージョン(ES6)では、値を変更できない `const`　と　参照範囲を有効にできる `let` が加わった

<!-- > JavaScriptでは型を記述しなくても良い -->

&nbsp; &nbsp;

### 変数を宣言し値を代入

変数を命名して宣言する。変数に値を保存する。



```
var colorValue; // 変数colorValueを宣言

colorValue = '#FF0000'; // 変数colorValueに値 '#FF000' を代入
```

> 変数の保存はパソコンのメモリにデータを保存するイメージ

&nbsp; &nbsp;

### 変数宣言と代入を同時に

```
var color = '#FF0000'; // 変数colorを宣言し、値 '#FF0000' を代入
```

&nbsp; &nbsp;


## 変数に保存できる値の種類

* 数値
* 文字列
* 真偽値
* Null

&nbsp; &nbsp;


## 数値　の保存

値に数字をそのまま記述して保存すると、数値として計算処理できる

```
var numA = 3; // 変数numAに数値3を代入
var numB = 6; // 変数numBに数値6を代入
var result = numA + numB; //変数numAと変数numBを足す
console.log(result);
// 結果は9
```

&nbsp; &nbsp;


## 文字列

値を `"`ダブルクォーテーションまたは `'`シングルクォーテーション で囲んで代入すると、文字列として処理される

```

var message = 'Hello';
var numA = '3'; // 変数numAに文字列3を代入
var numB = '6'; // 変数numBに文字列6を代入
var result = message + numA + numB;
console.log(result);
// 結果はHello36　すべて文字として連結される

```


`"`ダブル、`'`シングルどちらでも使えるが、必ず開始と閉じを同じにする。JavaScriptは、HTMLと同時に記述することがあるので、`'`シングルを推奨される。（HTMLのタグ内は必ず `"`ダブルで書くため）

&nbsp; &nbsp;-

## 真偽値

真(true)と偽(false)の2種類の値だけを扱う

```
var isFlag = true; // 変数myFlagに真(true)を代入
```

&nbsp; &nbsp;



## Null

データがない、返す値がないことを表す

```
var myTest = null; // 変数myTestは空っぽ
```


&nbsp; &nbsp;
