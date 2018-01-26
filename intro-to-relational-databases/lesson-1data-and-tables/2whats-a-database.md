#What's A Database
When you've written code before, you've used data structures such as variables, lists, [dictionaries](http://www.python-course.eu/dictionaries.php), and objects. These all let you store information while your program is running. You can build up complex data structures like a list of dictionaries. When your program exits, the structure will be gone in memory.
>如果你之前寫過程式，你應該會用 variable、list、dictionaries 這些資料結構去存資料。但當你關閉程式這些 variable 也會從記憶體消失。

You've probably worked with files. The files contain your own code. If you edit code in the text editor and save it, then quit the editor, you code doesn't vanish the way variable does, when the program exits. The file is persistent and durable, whereas in memory data is ephemeral(短暫的) or temporary. Programs can read and write files just fine, so why bother with databases?
>另外你應該有用過檔案存你的 code，如果你在編輯器存了檔案，然後關閉編輯器，檔案不會像 variable 那樣消失。檔案是可以保存的，不像記憶體裡的資料只是暫時性的。如此說來可以存起檔案就好了，為何還要 database 呢？

There are several different kind of databases, but what they all have in common is that they give us both persistence, like a file, as well as data structures for storing and searching our data, usually much faster and easier than we could search a flat file.
>其實有好幾種資料庫，他們的共同之處就是持久性，就像檔案一樣，另外還可以儲存和搜尋數據結構。

They also make it possible for multiple programs or users to access and modify data at the same time without stepping on each other's toes or accidentally undoing each other's changes. That's generally not possible with flat files. If two programs write the same version at the same time, then one will overwrite the other.
>另外資料庫可以在用戶讀取時，同時也進行修改，如果是一般檔案就會有覆寫檔案的問題。

So these other sorts of databases do all that, but relational databases do even more. Aside from storing your data, relational databases also offer very flexible tools for querying and summarizing data. If we're doing comparison, and if we're drawing connections between related pieces of information. They also let set up constrains which are rules to ensure the changes to our data are consistent. We'll see more about those later in the course.
> relational databases 除了上面那些功能外，還有一些工具可以查詢或彙整資料。還可以設定一些限制，確認我們對數據的修改是一致的，下面的課程會再細講。