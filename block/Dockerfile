# ベースとなるDockerイメージ
FROM openjdk:17

# アプリケーションのJARファイルをコンテナ内にコピー
COPY build/libs/block-0.0.1-SNAPSHOT.jar /app.jar

# アプリケーションのポートを指定
EXPOSE 8080

# コンテナ起動時に実行されるコマンド
ENTRYPOINT ["sh", "-c", "java -jar /app.jar"]

