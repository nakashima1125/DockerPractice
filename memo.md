# チュートリアル
## docker ps
動いてるコンテナを表示

## docker ps -a
存在するコンテナを表示

## docker run --name apa000ex1 -d httpd
apa000ex1というコンテナを作成し、バックグラウンドで実行。Apatchを最新バージョンを使用。

## docker rm apa000ex1
apa000ex1を削除する。

## docker stop apa000ex1
apa000ex1を停止する。

## docker run --name apa000ex2 -d -p 8080:80 httpd
ホストのポート番号を8080, コンテナのポート番号を80で設定する。
Apachサーバのコンテナはポート番号80で待ち構えているので、上記の設定でApachサーバのコンテナへアクセスできる。
複数のコンテナを立ち上げる際はホスト側のポート番号は異なる値にすること。

## docker run --name nginx000ex2 -d -p 8080:80 nginx
nginxのコンテナを、nginx000ex2という名前で立ち上げる。

## docker run --name mysql1000ex7 -dit -e MYSQSWORD=myrootpass mysql
MySQLのコンテナを、mysql1000ex7という名前で作成する。
-ditでバックグラウンドで実行する。-e MYSQSWORD=でMySQLのルートパスワードを設定する。
mysqlで、最新のsqlのイメージを持ってくる。

## docker image ls
存在するイメージの一覧

## docker image rm httpd mysql
イメージの削除。コンテナを消してもイメージは消えないので、消す必要がある。
