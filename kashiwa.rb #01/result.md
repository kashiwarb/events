当日の振り返り
===============================
-------------------------------

- RubyとRailsってそもそも何なの？  
Rubyはスクリプト言語で、RailsはRubyを使用するWeb開発用のフレームワーク  

- RailsでRuby以外の言語を使う事はできるの？  
RailsはRuby専用。他の言語にも似たようなフレームワークは存在する。PHP：CakePHPなど

- MVCモデルとは？  
MVC(Model View Controller)の略、ソフトウェアを３つの構成に分けて構築する設計思想。Modelは業務処理、Viewは画面入出力、ControllerはModelとViewを接続する処理を担います。RailsはMVCモデルを採用しているフレームワーク。

- Railsプロジェクトの__超基本的な構成__
      ・app  
        ・controllers  
          Controllerクラスを記述
        ・models
          Modelクラスを記述
        ・view
          .erbや.slimで画面を記述
      ・config  
        ・database.yml  
          データベース接続設定を記述
        ・routes.rb  
        ・画面繊維を記述
      ・db  
        ・migrate  
            データベースの変更が記述されていく
      ・Gemfile  
        Ruby、Railsのバージョン、使用されるgemを記述する

- CSSは何処に書けばいいか？
app/assets/styleseets内

- WebAPIを作れるようになりたい(なった方が良い)
- 他に出てきたキーワード、REST、Sinatra、Chef、Docker、NSRails、ATOM


## 次回以降の開催について
- それぞれ、作成したいものを作って行くもくもく形式で行なう。
- 次回は７月２３日に予定
- LTもやりたい
