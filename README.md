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


