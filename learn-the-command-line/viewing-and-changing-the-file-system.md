# Summary

* Options modify the behavior of commands:

* * `ls -a`
lists all contents of a directory, including hidden files and directories
* `ls -l`
lists all contents in long format
* `ls -t`
orders files and directories by the time they were last modified
* Multiple options can be used together, like
`ls -alt`
* From the command line, you can also copy, move, and remove files and directories:
* `cp`
copies files
* `mv`
moves and renames files
* `rm`
removes files
* `rm -r`
removes directories
* Wildcards are useful for selecting groups of files and directories

## Manipulation

Learn how to copy, move, and delete files and directories from the command line

```
$ ls -a

. .. .preferences action drama comedy genres.xt
```

* The `ls`command lists all files and directories in the working directory.

* `ls -a`to display the contents of the working directory in more detail , 其實就是列出所有內容，包含隱藏的檔案

* The`-a`modifies the behavior of the `ls`command to also list the files and directories starting with a dot \(`.`\). Files started with a dot are hidden, and don't appear when using `ls`alone.

* 把檔名開頭是 `.`的檔案列出來

* `-a`並不一定要加

### List Command and Options

* `ls -a` 的 -a 叫做 _**option**_

* Options modify the behavior of commands

* -a

* lists all contents, including hidden files and directories

* -l

* lists all contents of a directory in long format,**可以看到資料夾下有什麼檔案**
* long format 請見補充說明的文章 The Wide and Long Data Format
* 呈現像 table，下個這個例子有 4 rows, 7 column，每一個欄位代表

* Access rights. These are actions that are permitted on a file or directory.

* Number of hard links.This number counts the number of child directories and files. This number includes the parent directory link \(`..`\) and current directory link \(`.`\).

* The username of the file's owner. Here the username is `cc.`

* The name of the group that owns the file. Here the group name is `eng`

* The size of the file in bytes.

* The date & time that the file was last modified.

* The name of the file or directory.

* ```
$ ls -l
drwxr-xr-x 5 cc eng 4096 Jun 24 16:51 action
drwxr-xr-x 4 cc eng 4096 Jun 24 16:51 comedy
drwxr-xr-x 6 cc eng 4096 Jun 24 16:51 drama
-rw-r--r-- 1 cc eng 0 Jun 24 16:51 genres.txt
```
* `ls -alt`

* 是 ls-a 和 ls -l 和 ls-t 的綜合體

* lists all contents, including hidden files and directories, in long format, ordered by the date and time they were last modified.

* ```
$ ls -alt
drwxr-xr-x 4 cc eng 4096 Jun 29 12:22 .
-rw-r--r-- 1 cc eng 0 Jun 29 12:22 .gitignore
drwxr-xr-x 5 cc eng 4096 Jun 30 14:20 ..
drwxr-xr-x 2 cc eng 4096 Jun 29 12:22 satire
drwxr-xr-x 2 cc eng 4096 Jun 29 12:22 slapstick
-rw-r--r-- 1 cc eng 14 Jun 29 12:22 the-office.txt
```
* -t

* Order files and directories by the _**time**_ they were last modified.

## Cp Command

```
cp biopic/cleopatra.txt historical/
```

* 複製檔案某個資料夾的檔案，到某個資料夾

* 第一個 argument 是 biopic/cleopatra.txt，第二個 是 historical/

```
cp biopic/ray.txt biopic/notorious.txt historical/
```

* 也可以一次複製兩個檔案
* first arguments 是 biopic/ray.txt 和 biopic/notorious.txt，第二個是 **historical/**

### Wildcards

```
cp * satire/
```

* 除了用檔案名當 arguments 外，我們可以使用 special character 像 \*
* \*用來 select groups of files，這個特殊符號我們叫 Wildcards
* The`*`selects all files in the working directory, so here we use `cp`to copy all files into the **satire/ **directory.

```
cp m*.txt scifi/
```

* `m*.txt`selects all files in the working directory starting with "m" and ending with ".txt", and copies them to _**scifi/**_

## Mv Command

* 移動檔案，使用方式類似 cp

```
mv superman.txt superhero/
```

* 把 first argument 移到 second argument

```
mv wonderwoman.txt batman.txt superhero/
```

* 把 前二個 arguments 移到 second argument

```
mv batman.txt spiderman.txt
```

* **這一項很特別，這是改名!!!**
* By moving **batman.txt **into **spiderman.txt**, we rename the file as **spiderman.txt**


![](/assets/Viewing and Changing the File System_1.png)

## Rm Command

```
rm waterboy.txt
```

* 用來刪除檔案或資料夾

```
rm -r comedy
```

* The`-r`is an option that modifies the behavior of the`rm`command.
* The`-r`stands for "recursive," and it's used to delete a directory and all of its child directories.
* 把整個資料夾都刪除，要注意這是**永久刪除!!**

```
rm media/*
```

![](/assets/Viewing and Changing the File System_2.png)


## 練習題

![](/assets/Viewing and Changing the File System_3.png)
