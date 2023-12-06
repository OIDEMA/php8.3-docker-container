# PHP8.3のDocker環境
2023年12月6日作成

## 使い方

```
$ docker compose build
```

### もしキャッシュを利用しない形でビルドしたい場合

```
$ docker compose build --no-cache
```

## コンテナを起動する
- ターミナル上でログなどを参照する場合は下記のコマンドでOK

```
$ docker compose up
```

### バックグラウンド実行したい場合は下記コマンド
- この場合、ログなどを見たい場合は、Docker Desktop側で見てください

```
$ docker compose up -d
```

## Dockerコンテナ内への初期データ入れ方
- mysql/seed内にdumpファイル（※.sql）を設置することで初回起動時にデータが閲覧できます


## phpMyAdminへのアクセス
- http://localhost:80


## サイトの確認
- http://localhost:8080/
