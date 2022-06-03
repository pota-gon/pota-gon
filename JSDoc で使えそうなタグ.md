# JSDoc で使えそうなタグ
JavaScript の勉強中なので、JSDoc で使えそうなタグをまとめてみました。  
主に自分のコピペ用です。

## <span>@</span>file
ファイルの説明に使います。

```js
/** 
  * @file ファイルの説明
  * @version Ver1.0.0
  * @author 作成者名
  * @license {@link 作成者URL}
  * @copyright Copyright (c) 2020 作成者名
  */
```

## <span>@</span>class
クラスの説明に使います。

```js
/**
  * コンストラクタの説明
  *
  * @class
  * @extends 継承元
  * @classdesc クラスの説明
  */
function Sample() {
    this.initialize.apply(this, arguments);
}
```

## <span>@</span>namespace
```js
/**
  * 名前空間の説明
  *
  * @namespace
  */
function NameSpace() {
    throw new Error("This is a static class");
}
```

## <span>@</span>memberof
return は非推奨なので、returnsを使うこと。

```js
/**
  * メソッドの説明
  *
  * @memberof NameSpace
  * @param {number} num - 引数の説明
  * @returns {number} 返り値の説明
  * @throws {Exception} 例外の説明
  * @see 他の定数等を参照
  * @deprecated 非推奨
  */
function Sample.prototype.param = function(num) {
    return num;
}
```

## <span>@</span>type
```js
Sample.initialize = function() {
    /**
     * 説明
     *
     * @readonly
     * @type string
     * @name Sample.sampleVal
     * @default "sample"
     */
     this.sampleVal = "sample";
}
```

## <span>@</span>constant
定数の説明に使います。

```js
/**
  * 定数の説明
  *
  * @type string
  * @constant
  */
const SAMPLE_CONST = "sample";
```

## <span>@</span>member
```js
/**
 * @member {number} メンバ変数の説明
 */
this._index = 0;
```

## <span>@</span>example
```js
/**
 * @todo example について使い方を記載する
 * @example
 */
```

## <span>@</span>enum
```js
/**
 * @enum {number}
 */
HOGE = {
    FIZ: 3,
    BUZZ: 5,
    FIZBUZZ: 8
};
```

