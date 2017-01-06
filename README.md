Okinawa.pm Webサイトビルドツール
======================================================

環境構築
--------

    $ git clone git@github.com:OkinawaPM/website.git --recursive
    $ cd website
    $ carton install --deployment


開発時Webサーバ起動 / Riji
--------

    $ carton exec -- riji server


公開時Webサイト静的ビルド
--------

    $ carton exec -- riji publish 


タスク一覧
--------

    $ carton exec -- daiku -T


