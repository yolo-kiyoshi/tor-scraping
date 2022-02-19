# 概要
Torネットワークを使ったスクレイピングを検証する

# 使い方
## ビルドとコンテナ起動
以下のコマンドによりDockerイメージのビルドとコンテナを起動できる。
```
docker-compose up
```

_※`Dockerfile`を変更しリビルドしたい場合は`docker-compose up -d --build`を実行する_

## コンテナ実行
以下のコマンドによりDockerコンテナを実行できる。
```
docker-compose run --rm app python -m main
```

複数コンテナを非同期実行したい場合は以下のshellを実行する。
```
./start.sh
```

## パッケージの追加
以下のコマンドでPythonパッケージを追加できる。
```
poetry add <追加したいパッケージ>
```