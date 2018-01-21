[git sum](https://git-scm.com/book/zh-tw/v1/開始-關於版本控制)

#名詞解釋
[res (Revision Control System)](https://en.wikipedia.org/wiki/Revision_Control_System)





目前有的問題：
* 為何無法建立 repository 的問題
 * https://help.github.com/articles/changing-a-remote-s-url/
 * https://git-scm.com/book/zh-tw/v1/Git-分支-遠端分支
* 我要在兩台電腦用同一個帳號下，更新 repository

What is Gitignore
* [參考文章](https://ithelp.ithome.com.tw/articles/10138831)


方向
* Git Remote
* [SSH key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

#SSH Key

https://gitlab.kkinternal.com/help/ssh/README
* Secure communication channel for sharing information
* 讓你不用每次都提供 username 或 password
* 先看完第一段，第二段之後就是實作

#[Digital Ocean Tutorial of SSH Key](https://www.digitalocean.com/community/tutorials/understanding-the-ssh-encryption-and-connection-process)
* 英文版直接看上面，中文版如下

為了資料傳遞上的安全，SSH 在不同的地方用了許多種資料控制的技巧( data manipulation techniques)， 主要包含三種方式

## Symmetrical Encryption
who holds the key can encrypt and decrypt messages to anyone else holding the key
有 key 的人就可以編碼與解碼

看到 This type of encryption scheme is often called "shared secret" encryption, or "secret key" encryption. 

這一段

## Asymmetrical Encryption

## Hashing



##相關名詞
* cryptographically 加密的
* authenticate 驗證

## 裡面有提到，後續還有三篇文章
1. [how to configure SSH key-based access](https://www.digitalocean.com/community/tutorials/how-to-configure-ssh-key-based-authentication-on-a-linux-server)
2. [how to connect using SSH](https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server-in-ubuntu)
3. [some SSH tips and tricks](https://www.digitalocean.com/community/tutorials/ssh-essentials-working-with-ssh-servers-clients-and-keys)

 
