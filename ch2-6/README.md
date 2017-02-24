# Conceptual Aside: Syntax Parsers, Execution Contexts, and Lexical Environments



### Syntax Parser
  - A program that reads your code and determines what it does and if its grammer is valid.
  - Javescript 與 電腦之間溝通的轉譯媒介，將 Javescript 語法逐字解析並轉為電腦可識別之內容


### Lexical Environment
  - where something sits physically in the code you write
```javascript
var name = 'Jack';

function last() {
  console.log(name);
}

function test() {
  var name = 'Jason';
  console.log(name);
  
  last();
}

test();
```
![Alt text](ec.jpg)


### Execution Context
  - 目前執行之 scope，如果要呼叫一個在該exection context中沒有的變項時，它會往它的 outer environment去找。
  - refer. - http://chocochocoduck.tumblr.com/post/144812296253/js-%E8%AB%87%E8%AB%87execution-context
  - 
![Alt text](ec.jpg)