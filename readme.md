# 練習の目的

Dockerコマンドを覚える
Spring Boot開発になれる


# できたこと

dockerコンテナ上で、SpringBootアプリのビルド

# できていないこと

SpringBootアプリのホットリロード（アプリを再起動させずに、ソースコードの変更をリアルタイムに反映）

# セットアップ手順

OS：Windows10
Docker：ver.25.0.3

1.
blockディレクトリに移動し、コマンドプロンプトで「gradlew build」を実行する。
（このとき前回のビルド生成物があると、この後の操作がうまくいかないことがある。上記コマンドに先んじて「gradlew clean」を実行する。）

2.
SpringBootOnDockerディレクトリに移動し、コマンドプロンプトで「docker-compose build --no-cache」でコンテナを生成する。

3.
さらにコマンドプロンプトで「docker-compose up -d」でdockerコンテナを起動する。

> http://localhost:8080へアクセスすると、/block/src/main/resources/templates/index.htmlが表示される。

> 停止するときは、コマンドプロンプトで「docker-compose stop」を実行する。