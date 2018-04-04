#Branching 
Multiple different directions

如果有 bug 的時候是在 master 開一個 branch 叫 fix bug，而不是 reset 回來到上一版本修。

![](/assets/lecture 1_1.png)

Head is where we currently are in the repository. Head points to master. Git is easy to change where the head is.

#git branch
Listing all of branches
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


#實作上遇到的問題
看來是 master 跟 original 都有一個 commit

![](/assets/git_4.png)

[stack overflow](https://stackoverflow.com/questions/2452226/master-branch-and-origin-master-have-diverged-how-to-undiverge-branches) 解法
最後我是用 `git reset --hard origin/master`


# Remotes
A version of repository left somewhere, like Github.

## git fetch
Go to the remote repository online repository and download locally.

 
#Forks 

到 28:53
https://www.youtube.com/watch?v=XQs5KcUj-Do








