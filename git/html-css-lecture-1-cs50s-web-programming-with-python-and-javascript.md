#Git - Keep Changes of Code
When we design projects, how to collaborate with people

Keep tracking about different version of project. 

Synchronizing code between different people. 

Test changes to code without losing the original.

Revert back to old versions of code.

## What Happens to The Remote Repository?
The answer is the changes I make to my computer, to my version of the repository on my computer. Never affect what's going on online unless I try to push those changes to Github.


## Git Clone
Download the repository on your own computer

## Touch
Create a new file
* touch `<filename>`

## atom .
編輯一個簡單的 html 頁面

#Git Add
Tell the git what files I want to track. Next time I want to copy to repository. Add the files we want to commit next time.
* `git add <filename>` (只加進我已經完成、要追蹤的檔案)
* `git add *` (加進所有檔案)

#Git Commit
* git commit -m "message"

#Git Status
What's going on inside of your repository.

#Git Push
How to send those changes back to Github. That's called the push! We've made changes to the repository adding hello.html on our computer locally, but that isn't yet reflected on Github.

#Git Pull
Pull down the latest change from GitHub. In the tutorial, we remove a line of "Hello World" and increase a line of "Hello World!Hello Again!" so there will be a 1 insertion(+), 1 deletion(-).

#Merge Conflict
先修改自己的檔案然後 git add 追蹤，然後 commit 了。git pull 的時候會發現 repository 有新版本，你的程式碼會標出不同顏色。

![](/assets/git_2.png)

#Git Log
Show you the commit history.

![](/assets/git_3.png)

#Git Reset
28:03

Use `git log` to see the git hash, you just need a part of commit hash, is usually sufficient to be able to identify it.

`git reset --hard 3ba710f26d1`

And the repository won't affect by your reset unless you git push.

#git commit -am
看來是等同於 git add 加上 git commit -m 
[參考資料](https://gogojimmy.net/2012/02/29/git-scenario/)
29:40

Before the git commit, you have to git add a file to the staging area and telling it these are files that I want to track.

#git reflog
Git tracks of all the different snapshots,the `git relog` command is just the log of different references.


#Error Statements

fatal: pathspec 'Fig' did not match any files

touch Fig 2.3_Printing a line of text with multiple statements.cpp
> 會出現一堆檔案![](/assets/git_1.png)

要使用 `rm` 把他們清光
```rm Fig 2.3_Printing a line of text with multiple statements.cpp```




#Github
A website repositories on the internet.

Commit means we work on a project and continue making changes. The term we use commit to our project.

Commit message


#Image tag
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


#HTML Color Picker

https://www.youtube.com/watch?v=1u2qu-EmIRc


Start a new feature in existing web application.

#Branching 
Multiple different directions

如果有 bug 的時候是在 master 開一個 branch 叫 fix bug，而不是 reset 回來到上一版本修。

![](/assets/lecture 1_1.png)

Head is where we currently are in the repository. Head points to master. Git is easy to change where the head is.

#git branch
輸入 `git branch`這個指令會把所有 branch 列出來。
如果要增加 branch 就在後面加上名稱，例如

`git branch feature`

在 iTerm2 裡會把 master branch 前面標示星號並且字體為綠色。

![](/assets/lecture 1_2.png)

#git checkout
Change we currently are in the repository. We can change one branch to another branch.

如果要 move to 其他 branch 的指令是

`git checkout feature`

這樣就會 master branch 轉到 feature 這個 branch

#git commit -am
It means add all of the files that I've changed that I've already been tracking and commit them at the same time. Just combines few steps in a one.

#git push --set-upstream

#git merge
Allows two separate branch and combine them together.

到 17:22
https://www.youtube.com/watch?v=XQs5KcUj-Do

