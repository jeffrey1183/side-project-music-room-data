# Requirements
Before you [install Jekyll](https://jekyllrb.com/docs/installation/#requirements), make sure your system has the following:

1.Installing [Homebrew](https://brew.sh) be your package manager for macOS. Homebrew is just one of way of installing Ruby.
> 在安裝 Jekyll 前要先搞定 Ruby 的安裝，在 Mac 上要安裝 Ruby 可以用 Homebrew 這個套件管理工具。

2.On macOS (High) Sierra and OS X El Capitan, Ruby 2.0 is included. Jekyll requires Ruby version 2.2.5 or above.
> macOS Sierra 和 OS X El Capitan 有內建 Ruby 2.0，但 Jekyll 需要 Ruby 2.2.5 版以上。

Many people on OS X use Homebrew as a package manager. It is really easy to get a newer version of Ruby using Homebrew:

`$ brew install ruby`

3.Check the [RubyGems](https://rubygems.org/pages/download) which is a package management framework for Ruby. 


4.Check you have installed [GCC](https://zh.wikipedia.org/wiki/GCC) and [GNU Make](https://www.gnu.org/software/make/)


#Install with RubyGems
[RubyGems](https://rubygems.org/pages/download) is a package management framework for Ruby.

The best way to install Jekyll is via RubyGems. At the terminal prompt, simply run the following command to install Jekyll:

`gem install jekyll`

#[Quick-start guide](https://jekyllrb.com/docs/quickstart/)

If you already have a full Ruby development environment with all headers and RubyGems installed, you can create a new Jekyll site by doing the following:

>在建置好 Ruby 的開發環境與安裝好 RubyGems 後，你可以按照下面的步驟建置一個 Jekyll 網站：

![](/assets/Install Jekyll_1.png)
* If you enter `gem install jekyll bundler` and pop up the message of "bundler's executable "bundle" conflicts with /usr/local/bin/bundle.Overwrite the executable?" [The conflict means you already have Bundler installed](https://stackoverflow.com/questions/49267951/bundlers-executable-bundle-conflicts-with-usr-local-bin-bundle-overwrite-the#_=_).

>如果在執行 `gem install jekyll bundler` 時跳出下面這些訊息：
bundler's executable "bundle" conflicts with /usr/local/bin/bundle.Overwrite the executable? 
表現你已經安裝過 bundler 了。

After executing those commands, you can browse to http://localhost:4000, here is [more detail](https://jekyllrb.com/docs/quickstart/#about-bundler) about bundle.

>在執行完上面的指令後，你可以輸入 http://localhost:4000
瀏覽一下頁面。更多關於 bundle 的細節可參考[這裡](https://jekyllrb.com/docs/quickstart/#about-bundler)。



##Fix the Error of ERROR `/favicon.ico' not found.







