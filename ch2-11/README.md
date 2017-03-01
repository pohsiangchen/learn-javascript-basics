# Conceptual Aside: Javascript and 'undefined'


### undefined
 - 為 Javascript 中一個特別的 Value，一個 special keyword，表示變數存在於 memory space 中，但尚未設定初值
 - Javascript engine 在執行 execution context 中，所有變數的初值皆為 undefined，因此如果 programmer 未賦予變數任何其他值，其變數的 Value 將為 undefined
 - undefined 表示該變數尚未被賦予初值，是 Javascript engine 自己給予變數的值。
   因此千萬別自己刻意將變數設為 undefined，應保持 undefined 這個訊息表示為「未給值」，以利 debug
 
#### 範例

```javascript
****** Example - undefined ******
var a;
console.log(a);

if (a === undefined) {     // undefined 不是 String, 是一個 special keyword 
    console.log('a is undefined');
}
else {
    console.log('a is defined');
}

// ===== Output =====
// undefined
// a is undefined
// ==================
*********************************


******* Example - defined *******
var a = 'Hello Word';       // 若我們給予 a 一個初值，則 a 即為 defined 
console.log(a);

if (a === undefined) { 
    console.log('a is undefined');
}
else {
    console.log('a is defined');
}

// ===== Output =====
// Hello Word
// a is defined
// ==================
*********************************
```

### not defined
 - 變數從未變宣告過

#### 範例

```javascript
console.log(a);     // 變數 a 從未被宣告過

if (a === undefined) { 
    console.log('a is undefined');
}
else {
    console.log('a is defined');
}

// ===== Output =====
// Uncaught ReferenceError: a is not defined
// ==================
```
