# CSS Selectors

## All HTML Elements are Selectors

我們可以把`<ul>`,`<table>`這些 elements 都當作 CSS selector

```css
body
{
background-color:#C6E2FF;
}
```

## Multiple Selectors

如果我們要改變像被包起來的 elements

```html
<div>
<div>
<p>I like tacos!</p>
```

CSS 就要寫成像這樣

```css
div div p
{ /*CSS stuff!*/
}
```

## One Selector to Rule Them All

要一次設定所有 elements 的樣式，可以用`*`

```
* {
border: 2px solid black;
}
```

## Keeping the HTML Elements Classy

如果你有一堆 HTML elements 要調整成同樣的樣式，請使用 class，而不是一項一項去加進 CSS 的 property。

在 HTML 加進 class

```html
<div class="square"></div>
<img class="square"/>
<td class="square"></td>
```

在 CSS 內使用`(.)`

```css
.square {
height: 100px;
width: 100px;
}
```

## 在Html加入CSS的語法，使用 &lt;link&gt; tag

```html
<link type:"text/css" href="css的檔名.css" rel="stylesheet">
```

基本語法

```css
selector {property: value;}
```

selector:在html裡的tag（可以是標題 段落）

property:要修改的變數像是字體（font-family），大小\(font-size\)，顏色

value:設定的值，e.g. 10px 和 red

## CSS 中 Back Value 的用法

You can tell CSS to try several value, going from one to the next if the one you want isn't available

* 第一個值不 work 就會啟動下一個 value。

```css
selector {property: bestValue, nextBestValue}
```

實例（字體的設定，設定 Garamond, serif 兩個值）

```css
p {
color:#4A4943;
font-size:18px;
font-family:Garamond, serif}
```

## CSS 中 img 的邊框顏色和圖片大小設定

```css
img{
height:100px;
width:300px;
border:1px, solid, #4282b4;
}
```

## Html 中設定 class

```html
<div class="square">
</div>
```

## CSS中 設定 class（加上dot）

```css
.square{color:red;}
```

## Html中設定id

```html
<div id="square"></div>
```

## CSS中設定id（加上\#）

```css
#square{color:red;}
```

## pseudo-class selector

* control the appearance of unvisited and visited links—even links the user is hovering over but hasn't clicked!
* 控制有點過跟沒點過的連結樣式、也可以設定 hover 時候的顏色。

pseudo-class selectors

* 在css中加上冒號，冒號後可加 link, visited, hover 分別表示連結未被點擊時的設定,被點擊過和滑鼠移動上方

```css
a:link An unvisited link.
a:visited: A visited link.
a:hover: A link you're hovering your mouse over.
```

CSS 範例

```css
a:link{text-decoration:none;color:#008B45;}
a:hover{color:#00FF00;}
a:visited{color:#EE9A00;}
```

## First child 的使用

* 當有一堆段落，挑選出第一個來設定

css實際案例

```css
p:first-child{font-family:cursive;}
```

## 當有一堆段落，挑選出第二段來設定

```css
p:nth-child(2) {
color: red;
}
```

## Serif 和 Sans-serif\(襯線\)

* [中文說明](http://tdesign.tw/serif/)
* serif: A font with little decorative bits on the ends of the strokes that make up letters. Do a search on "serif" to see what we mean.
* sans-serif: A plain-looking font, like this one. It doesn't have the little doohickies on the ends of letters like a serif font does.
* cursive: A scripty font! It looks like cursive writing.

## css中設定圓圈

```css
div {
display: inline-block;
margin-left: 5px;
height:100px;
width:100px;
border-radius:100%;
border:2px black solid;
}
```

## Display屬性的基本觀念

* [中文介紹](http://zh-tw.learnlayout.com/display.html)
* inline\(行內元素\)

* `span`是一個標準的行內元素。一個行內元素可以在段落中

* 不會打亂段落原本的版面配置。

* `a`tag 是最常見的行內元素，它可以被用作超連結之用。

* block\(區塊元素\)

* 一個區塊元素會讓其內容從新的一行開始顯示，並盡可能的撐滿容器。

* 常用的區塊元素包括`p`、`form`以及一些 HTML5 新出現的元素，例如：`header`、`footer`、`section`等等。

## 設定兩個div的相對位置

```css
position:absolute;
```

* abosolute可替換成relative, fixed

# CSSmargin-left Property

* 左邊間隔20px

```css
margin-left:20px;
```

## css屬性, z-index簡介

使用於多個元件的順序，數字越高越在上層

```css
#header{ position:fixed;
z-index:1;}

#footer{ position:fixed;
z-index:2;}
```

## 把區塊 float 在左側或右側

```css
.left{float:left;
}

.right{float:right;
}
```

# 設定顏色的三種寫法 - color property

1. RGB Values:0~255，255顏色最亮

```css
h1 {
color: rgb(102,153,0);
}
```

1. hexadecimal numbers: 00~ff，ff最亮

```css
h1 {
color:#9933CC;
}
```

1. Color names: [http://www.crockford.com/wrrrld/color.html](http://www.crockford.com/wrrrld/color.html)

```css
h1 {
color:aqua;
}
```

# 設定字體

[Google Fonts](https://www.google.com/fonts)\(over 600 more web fonts\)

```css
font-family: "Arial, Helvetica", sans-serif;
font-family: "Times New Roman", Times, serif;
font-family: "Courier New", Courier, monospace;
```

# 字體大小的單位

pixels, ems, or rems

* 一般就是px

The font-size unit em is a relative measure: one em is equal to the default font size on whatever screen the user is using. That makes it great for smartphone screens, since it doesn't try to tell the smartphone exactly how big to make a font: it just says, "Hey, 1em is the font size that you normally use, so 2em is twice as big and 0.5em is half that size!"

# 跟 background 相關的 property

* background-color
* background-image
* padding:調整border和content的距離
* margin:border以外的區域
* 使用margin-right: auto加上 margin-left: auto：可以把對象置中

# 講解margin,border,padding,text之間的關係

![](https://lh6.googleusercontent.com/YVlKknN73YoxijIlCxVdXQREbFvqENhuEsHe7H_HeaayLTs8yhClJ9ad2DuC3sCNo_8hhZoCp77VlC0De2J7QbNusW2iYyNx8_6tggaUjqLsHP8K115wpv1ubCr67JncN9gJS7Mr)

text-transform 屬性，可以控制文本的大小寫。

* 相關說明：[http://www.w3school.com.cn/cssref/pr\_text\_text-transform.asp](http://www.w3school.com.cn/cssref/pr_text_text-transform.asp)

## 設定background圖片

```css
.example{
background-image:url('https://goo.gl/04j7Nn');
}
```

## position, display, float - CSS Properties

The CSS properties display, position, and float can be used to control where an element sits on the page

* properties: [display](http://zh-tw.learnlayout.com/display.html)，[position](http://zh-tw.learnlayout.com/position.html) and [float](http://www.1keydata.com/css-tutorial/tw/float.php).

```css
position:fixed;
top:30px;
right:5px;
float:left;
```



