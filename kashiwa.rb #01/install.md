Ruby と Rails のインストール

========================

## Ruby と Rails のインストール

#### ・Mac
XCoceを一番はじめに入れておくこと

##### 用語説明
- Homebrew ： MacOS用のパッケージ管理ツール。いろいろなプログラミング言語やツールのインストールやアンインストールが行なえる。
- rbenv ： Rubyのバージョン管理ツール。様々なバージョンのRubyのインストールができ、バージョンの切り替えができるツール。Linuxでも使える。
- gem ： Rubyをインストールすると入る。プログラム内で使用するライブラリの操作が行なえる。PerlでいうCPAN、.NETでいうNuGet

##### 1.HomeBrew のインストール
terminalで以下を実行
```
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```
HomebrewのインストールはこれでOK

##### 3.rbenvのインストールまで
homebrewでopenssl、readline、ruby-build、rbenvをインストールして行きます。以下を上から順にterinalで実行する。
```
brew install openssl
brew install readline
brew install ruby-build
brew install rbenv
```
rbenvのインストール後、__~/.bash_profile__に以下を追加してパスを通す。__実行後ターミナルを再起動__
```
export PATH="$HOME/.rbenv/bin:$PATH"
eval "$(rbenv init -)"
```


##### 4.Rubyのインストール
rbenvでインストールできるRubyの確認
```
rbenv install -l
```
2.1.2のインストール（例）
```
rbenv install 2.1.2
```
以下を実行
```
rbenv rehash
rbenv global 2.1.2
```
有効なバージョンの確認
```
ruby -v
```
うまくインストールされていればインストールしたバージョンが表示されます。

##### 5.Railsのインストール
```
gem install rails
```
これでOK

#### ・Windows

##### 1.RubyインストーラーとDevKitをダウンロード
- Rubyインストーラーを使う方法
[http://rubyinstaller.org/](http://rubyinstaller.org/)
- pikを使う方法？

##### 3.Railsのインストール
- gem のアップデート
```
gem update 
gem upgrade
```
- Rails のインストール
```
gem install rails 
```
コレでOK(要確認)


## 動かしてみる



