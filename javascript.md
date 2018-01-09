#If...Else Statements

if 跟 else 後面的判斷不用加分號，分號在後面。

```js
if (12 >= 10)
{console.log("You got a true!");
} else {
console.log("You got a false!");
}
```

詢問年齡，判別後做回應

```js
var age = prompt("What's your age");

if(age < 13)
{console.log("they're allowed to play but you take no responsibility.");
}
else
{console.log("Don't give up");
}
```

# Using console.log\(\)

Prints into the console whatever we put in the parentheses.

For debugging purposes, you can use the **console.log\(\) **method to display data.

```js
console.log()
prompt("when can i sleep?")

//會跳出對話框
```

# 計算餘數

* console.log\(14%3\)

# Substrings

指定字串中其中幾個字

```
"hello". substring(0, 2);
```

* 以上面的程式碼為例，把hello拆成0~4

* 要記得第一個字排序是0

0 1 2 3 4

\| \| \| \| \|

h e l l o

使用 console.log 顯示結果

```
console.log("January".substring(0,3))
```

# 設置變數

---

```js
var myAge = 26;
console.log(myAge);
```

* So the variable stores the value of the variable, whether that is a number or a string

* We store data values in variables. We can bring back the values of these variables by typing the variable name.

* 變數的第一個字必須是小寫\(lowercase letter\)

## Variable Scope

* Scope can be global or local

* 差別在一個變數在 function 外定義，一個在 function 內

### Global Variable

Variables defined outside a function are accessible anywhere once they have been declared. They are called global variables and their scope is global.

For Example

```js
var globalVar = "hello";

var foo = function() {
console.log(globalVar);
prints "hello"
}
```

### Local Variable

* 變數定義在 function 內

```js
var bar = function() {
var localVar = "howdy";
}

console.log(localVar);
error
```

### Global variable 和 Local variable

在第四行中加入 var 造成 function 內的 my\_number 變成local variable，第一行變成global variable

```js
var my_number = 7; //this has global scope

var timesTwo = function(number) {
var my_number = number * 2;
console.log("Inside the function my_number is: ");
console.log(my_number);
};

timesTwo(7);
console.log("Outside the function my_number is: ")
console.log(my_number);
```

# Manipulating numbers & strings

* comparisons \(e.g. &gt;, &lt;=\)
* modulo \(e.g. %\)

# Function syntax

```js
var greeting = function (name) {
console.log("Great to see you," + "" + name);
};

greeting("Jeffrey");
```

1.Declaring a function using var

2.The name of function should begin with lowercase letter

3.The code in the parentheses is called a parameter

* function後設定此function的參數\(parameter\)

4.The entire function ends with a semi-colon.

5.呼叫function時，we call the function by just typing the function's name and putting a parameter value inside parentheses after it

## 多於一個 parameter 的 function

```js
var perimeterBox =function(length,width){
return length + length + width + width;
}

perimeterBox(5,5)
```

# String Concatenation

把字串連起來\(concatenation\)，如果你要字與字之間有空格，要記得加進空格，如下：

```
console.log("Hey" + " " + "you");
```

# Return

* When we call a function, its return value is just the result from running the function.

```js
var quarter = function(number){
return number/4;
}
```

# HTML的註解

* 使用&lt;!--與 --&gt;將要註解的文字包起來。

```html
<!--我是註解 -->
```

# CSS的註解

* 使用/\* 與 \*/ 將要註解的文字包起來。

```css
<STYLE>

/*這裡是註解*/

.樣式名a{
CSS屬性名A:屬性值;
CSS屬性名B:屬性值;
}

.樣式名b{
CSS屬性名B:屬性值;
CSS屬性名C:屬性值;
/*CSS屬性名D:屬性值; 這個屬性暫時不用*/
}

</STYLE>
```

# JavaScript 的註解

JavaScript 的註解符號和 Java 一樣，

註解的方式有兩種：

（1）/\* \*/ 多行的註解

（2）// 單行註解

單行註解是從到該行結尾

```
/*
多行註解可以橫跨多行
但是在註解中不可以再打一次註解
*/
```

# Java 的註解

* [說明](http://journals.ecs.soton.ac.uk/java/tutorial/getStarted/application/comments.html)
* [說明2](https://stackoverflow.com/questions/29815636/and-in-java-comments)

# 陣列的介紹 Arrays

* Any time you see data surrounded by \[ \], it is an array.

* Store lists of data

* Can store different data types at the same time

* Are ordered so the position of each piece of data is fixed

Examples:

```js
var names = ["Mao","Gandhi","Mandela"];
var sizes = [4, 6, 3, 2, 1, 9];
var mixed = [34, "candy", "blue", 11];
```

## Array positions

* 陣列中第一個值的 indexing number 是 0
* Arrays have 0-based indexing, so we start counting the positions from 0.
* 假設現在有一個 array

```
var arrayName = ["Mao","Gandhi","Mandela"];
```

* arrayName\[0\] 代表陣列中的第一個值 Mao，arrayName\[1\] 代表陣列中的第二個值 Gandhi，以此類推

應用案例

```
var cities = ["Melbourne", "Amman", "Helsinki", "NYC","Taipei"];

for (var i = 0; i < cities.length; i++) {

console.log("I would like to visit " + cities[i]);

}

console.log(cities.length)
```

避免text過長，可以使用backslash

```
var text = "Hey, how are you \
doing? My name is Emily.";
```

字串也可以用陣列呼叫

```
var myName = 'Eric';

myName[0]; equals 'E'
```

# 簡潔的 code, less is more

```
var bool = true;

while(bool){
Do something
}
```

等同於

```
var bool = true;

while(bool === true){
Do something
}
```


