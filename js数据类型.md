1.option(文本,赋值,ture,ture)

默认后面两个值为ture.

2.typeof

ECMAScript中有5种简单数据类型：Undefined、Null、Boolean、Number、String

```
undefined	--这个值未被定义;
boolean		--如果这个值是布尔值
string		--如果这个值是字符串
number		--如果这个值是数值
object		--如果这个值是对象或null
function	--如果这个值是函数
```

3.数值范围

由于内存的限制,ECMAScript不能保存世界上所有的数值.

```
Number.MAX_VALUE --最大值
Number.MIN_VALUE --最小值
```

如果计算结果超过数值范围，将自动转化为特殊的`Infinity`值,

负值转为`-Infinity`,正值转为`Infinity`

4.NaN

它是一个特殊的数值,.NaN与任何数值都不相等,也包括它本身.

```
console.log(NaN==NaN); --false
```

```javascript
console.log(isNaN(NaN));	--true
console.log(isNaN(10));		--false
console.log(isNaN("10"));	--false
console.log(isNaN("blue"));	--true
console.log(isNaN(true));	--false
```

true表示不能转化为数字，false表示可以转化：10,10,1

5.parseInt

用来转化为整形

```javascript
var num1=parseInt("1234blue");
var num2=parseInt(" ");
var num3=parseInt("0xA");
var num4=parseInt("22.5");
var num5=parseInt("070");
console.log(num1);	--1234
console.log(num2);	--NaN
console.log(num3);	--10
console.log(num4);	--22
console.log(num5);	--70 ES3中会当做八进制处理,ES5中当做十进制处理
```
