## docker network create wordpress000net1
仮想ネットワークを構築し、ネットワーク内でコンテナ同士を連携させる。

## docker run --name --net=wordpress000net1 -e mysql1000exPASSWORD=myrootpass -e mysql
MySQLのコンテナを作成と起動をする。
-ditでバックグラウンドで実行する。-e MYSQSWORD=でMySQLのルートパスワードを設定する。
mysqlで、最新のsqlのイメージを持ってくる。
