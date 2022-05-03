# jupyterlab_mysql
jupyterlabとMySQLをセットにしたdocker-composeディレクトリです

(dbとworkは自動で生成されます)
```
jupyterlab_mysql
├── db => (MySQLのデータ保存場所)
│── work => （jupyterlabのコードを保存する場所）
│           
└── docker-compose.yml
```


## ディレクトリのクローンのやり方
```
git clone git@github.com:keikois/jupyterlab_mysql.git
```

クローンした後
```
cd jupyterlab_mysql
```
```
docker-compose up -d
```
上記コマンドを打つと、jupyterlabとMySQLとphpMyAdminが起動します。

localhost:8888をブラウザで開くとjupyterlabが開きます。（pyhtonとRとJulia言語が使えます）

localhost:8080をブラウザで開くとmySQLとphpMyAdminが連携された状態で開きます。

コンテナ終了コマンドは
```
docker-compose down
```
