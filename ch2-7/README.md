# Conceptual Aside: Name/Value Pairs and Objects

### Name/Value Pair: A name which maps to unique value.
- 一個 name 對應一個值. 
- 在任何 excution context 的 name(變數) 只可以有一個 value(值).
```javascript
var name = 'Jack';
```

### Object: A collection of name/value pairs
- Javascript Object 是由一或多個 name/value pairs 組成的 collection
- 
```javascript
// address 由 collection of name/value pairs 組成
// street 與 number 個別為 name/value pairs
// apartment 又是另一個 collection, 裡面包含了其他的 name/value pairs
var address = {
  street: 'Main',
  number: 100,
  apartment: {
    floor: 3,
    number: 301
  }
};
```