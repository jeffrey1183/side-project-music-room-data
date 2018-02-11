#CS50 的課程
* [Lecture 0](https://www.youtube.com/watch?v=1u2qu-EmIRc)
* [Lecture 1 Youtube 連結](https://www.youtube.com/watch?v=qlq6DwRCJZU)

#Git - Keep Changes of Code
When we design projects, how to collaborate with people

Keep tracking about different version of project. 

Synchronizing code between different people. 

Test changes to code without losing the original.

Revert back to old versions of code.


## Git Clone
Download the repository on your own computer

## Touch
Create a new file
* touch `<filename>`

## atom .
編輯一個簡單的 html 頁面

#Git Add
Tell the git what files I want to track. Next time I want to copy to repository. Add the files we want to commit next time.
* git add `<filename>`

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
在 28:03 的地方

#git commit -am
看來是等同於 git add 加上 git commit -m 
[參考資料](https://gogojimmy.net/2012/02/29/git-scenario/)
29:40

Where the a stands for add to both files to the staging area and commit them all together in one command.

到 29:58

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
