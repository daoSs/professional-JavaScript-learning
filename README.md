# professional-JavaScript-learning
js红宝书学习笔记

## 3.5 操作符
> 后置递减和递增与前置有一个非常重要的区别，即递增和递减操作是在包含它们的语句被求值之后才执行的

```javascript
var num1 = 2;
var num2 = 20;
var num3 = num1-- + num2; //等于22
var num4 = num1 + num2;   //等于21
```
> 我们可以利用逻辑或的这一行为来避免为变量赋null或undefined值

```javascript
var found = true;
var result = (fount || someUndefinedVariable); //无错
alert(result);
```
> 变量someUndefinedVariable没有定义 所以found为true时才不出错

```javascript
var found = false;
var result = (fount || someUndefinedVariable); //有错
alert(result);

var myObj = preferredObj || backupObject; // myObj将会被赋予等号后面两个值中的一个
```
> for in 语句 ：用于枚举对象的属性