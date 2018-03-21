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