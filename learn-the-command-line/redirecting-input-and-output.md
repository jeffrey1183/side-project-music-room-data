到先前的課程為止，我們在用 command lines 跑了很多 commands，然後收到 terminal 的 output。這堂課我們主要會講 input and output \(I/O\) redirection.

Through redirection you can direct the input and output of a command to and from other files and programs, and chain commands together in a pipeline. Let's try it out.

## Echo Command

```
$ echo "Hello"
Hello
```

The `echo `command accepts the string "Hello" as _standard input_, and echoes the string "Hello" back to the terminal as

_standard output._

### Let's learn more about standard input, standard output, and standard error:

1. _standard input_, abbreviated as `stdin`, is information inputted into the terminal through the keyboard or input device.

2. _standard output_, abbreviated as `stdout`, is the information outputted after a process is run.

3. _standard error_, abbreviated as `stderr`, is an error message outputted by a failed process.

Redirection reroutes standard input, standard output, and standard error to or from a different location.

# How does redirection work?

## The Cat Command

* The cat \(short for “**concatenate**“\)
* 很常用!!
* 其實 Cat 有一堆[用法](http://www.tecmint.com/13-basic-cat-command-examples-in-linux/)。這邊有講到下面幾種
1. Use Standard Output with Redirection Operator. \(像 $ echo "Hello" &gt; hello.txt\)
2. 觀看檔案內容\(Display Contents of File

### 類型1

```
$ cat hello.txt
```

The `cat`command outputs the contents of a file to the terminal. When you type `cat hello.txt`, the contents of **hello.txt**

are displayed.

### 類型2

```
$ echo "Hello" > hello.txt
```

The`>`command redirects the standard output to a file.

Here,`"Hello"`is entered as the standard input. The standard output`"Hello"`is redirected by`>`to the file **hello.txt**.

```
$ cat oceans.txt > continents.txt
```

`>`takes the standard output of the command on the left, and redirects it to the file on the right. Here the standard output of

`cat oceans.txt `is redirected to **continents.txt**.

Note that`>`**overwrites** all original content in **continents.txt**. When you view the output data by typing `cat `on **continents.txt**

, you will see only the contents of **oceans.txt**.

* 會把原來的檔案覆蓋掉

### 類型3

```
$ cat glaciers.txt >> rivers.txt
```

* 添加的功能，rivers 這樣就會有 glaciers 的檔案

`>>`takes the standard output of the command on the left and _appends_\(adds\) it to the file on the right. You can view the output data of the file with `cat`and the filename.

Here, the output data of **rivers.txt **will contain the original contents of **rivers.txt **with the content of **glaciers.txt **appended to it.

### 類型4

```
$ cat < lakes.txt
```

`<`takes the standard input from the file on the right and inputs it into the program on the left. Here,

**lakes.txt **is the standard input for the `cat`command. The standard output appears in the terminal.

### WC \([Word Count](https://zh.wikipedia.org/wiki/Wc_%28Unix%29)\) Command 和 Pipe

```
$ cat volcanoes.txt | wc
```

`|`is a "pipe".The`|`takes the standard output of the command on the left, and _**pipes**_ it as standard input to the command on the right. You can think of this as **"command to command"** redirection. 

Here the output of `cat volcanoes.txt `is the standard input of `wc`. in turn, the `wc `command outputs the number of lines, words, and characters in `volcanoes.txt`, respectively.



```
$ cat volcanoes.txt | wc | cat > islands.txt
```


