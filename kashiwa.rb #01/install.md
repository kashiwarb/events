Ruby と Rails のインストール
========================
------------------------

## Ruby と Rails のインストール

#### ・Mac
[参考](http://www.oiax.jp/rails/zakkan/rails_3_1_installation_on_macosx.html)

Xcodeを一番はじめに入れておくこと

##### 用語説明
- Homebrew ： MacOS用のパッケージ管理ツール。いろいろなプログラミング言語やツールのインストールやアンインストールが行なえる。
- rbenv ： Rubyのバージョン管理ツール。様々なバージョンのRubyのインストールができ、バージョンの切り替えができるツール。Linuxでも使える。
- gem ： Rubyをインストールすると入る。プログラム内で使用するライブラリの操作が行なえる。PerlでいうCPAN、.NETでいうNuGet

##### 1.HomeBrew のインストール
terminalで以下を実行
HomebrewのインストールはこれでOK
```
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```

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
rbenv versions        ← rbenvで指定されているRubyのバージョン確認
ruby -v               ← macで使用されているRubyのバージョン確認
```

うまくインストールされていればインストールしたバージョンが表示されます。

##### 5.Railsのインストール
gemを最新版に更新して、gemでrailsをインストール
```
gem update
gem install rails
```
これでOK

#### ・Windows
[参考ページ](http://www.oiax.jp/rails/zakkan/rails_3_1_installation_on_windows.html)

## Scaffoldで感じをつかむ
[参考ページ](http://www.oiax.jp/rails/zakkan/rails_3_1_installation_on_windows.html)  
__動作確認用の新規アプリケーションの作成から下__を実行
