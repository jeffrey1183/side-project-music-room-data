##Image tag
* source attribute
* weight and height attribute
* width attribute

##Table
需要實作練習，其實就寫一列一列寫

```
<table>
    <tr> //table row
        <th>First Name</th> //table header
        <th>Last Name</th>
        <th>Years in Office</th>
    </tr> 
    <tr> //table row
        <th>First Name</th> //table header
        <th>Last Name</th>
        <th>Years in Office</th>
    </tr>

</table>
```

##Table border
<style>
    table {
        border: 2px solid black;
    }
    th, td{
        border: 1px solid black;
    }
    
</style>
```



#Form
Collecting information from users.


```
<form>
    <input type="text" placehodler="Full Name" name="name">
    <button>submit</button>
</form>

```

#Document Object Model
59:40


#CSS

## Three Ways of Linking CSS

1. Start from adding a style attribute.

```
<h1 style="color:blue;text-align:center">Welcome to My Web Page</h1>
```
color attribute 可以用 hex code


2. 除了這種包在裡面的之外，還可以用
```
<style>
    h1 {
    color:blue;
    text-align:center;
    
    }
</style>
```

這種寫法會套用在所有 h1 header

![](/assets/html_1.png)

3. link tag
separate out into a different file such that have many different HTML files. They can all reference the same CSS file.

```
<link rel="stylesheet" href="style.css">

```

#div
A section of my code

```
<style>
    div {
        background-color: teal;
        width: 100px;
        height: 400px;
        margin: 30px;
        padding: 20px;
    }
</style>
```

#margin & padding 
Margin is the space around the outside of the border element.

Padding is between the content of the element.


#font

```
<style>
    div{
        font-family: Arial, sans-serif;
        font-size: 28px;
        font-weight: bold;
        
    }
</style>
```

#border

案例1
```
<style>
    div{
        border: 3px solid blue;
        
    }
</style>
```
案例2
```
<style>
    div{
        border: 3px dotted red;
        
    }
</style>
```


到 1:24:27


#HTML Color Picker

https://www.youtube.com/watch?v=1u2qu-EmIRc



到 1:02:50
