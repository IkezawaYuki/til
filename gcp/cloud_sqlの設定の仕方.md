
goでクラウドSQLの使用
https://cloud.google.com/go/getting-started/using-cloud-sql?hl=ja

gcloud sql instances describe [YOUR_INSTANCE_NAME]
これで connection_nameを確認する

./cloud_sql_proxy -instances="[YOUR_INSTANCE_CONNECTION_NAME]"=tcp:3306

このコマンドの実行でcloudsqlへ。

3306ポートが使われている場合の確認コマンド
$ lsof -i :3306
https://ja.stackoverflow.com/questions/50813/3306%E3%83%9D%E3%83%BC%E3%83%88%E3%81%8C%E6%97%A2%E3%81%AB%E4%BD%BF%E3%82%8F%E3%82%8C%E3%81%A6%E3%81%84%E3%81%A6docker-run%E3%81%A7%E3%81%8D%E3%81%AA%E3%81%84