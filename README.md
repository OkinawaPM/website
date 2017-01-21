Okinawa.pm Webサイトビルドツール
======================================================

環境構築 / use v5.24
--------

    $ git clone git@github.com:OkinawaPM/website.git --recursive
    $ cd website
    $ git submodule update --init
    $ git submodule foreach git checkout master
    $ carton install --deployment


タスク一覧
--------

    $ carton exec -- daiku -T

記事の確認
--------

    $ git add article/entry/someday.md
    $ git commit -m 何かしらのコミットメッセージ
    $ daiku site:build    # サイトをビルド
    $ daiku site:preview  # ビルドしたサイトを表示

これは少し違うなと感じた場合
    
    $ git reset 'HEAD^'

を行うことで直前のコミットを取消せます！
