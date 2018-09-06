
# Apache の設定のテスト用の Docker 環境

## 事前準備

`docker-compose` を使えるようにする。

Mac であれば [Docker for Mac](https://www.docker.com/docker-mac) など。

## 実行

"docker-compose.yml" のあるディレクトリに移動し、
つぎのコマンドでコンテナとサーバーを起動する。

```bash
docker-compose up --build
```

ブラウザから Web サーバーにアクセスする。

初期の構成では以下の結果になる。

<http://localhost:8000/index.html>
--> 200

<http://localhost:8000/.hidden/index.html>
-->404
