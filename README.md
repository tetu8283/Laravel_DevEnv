<!-- コンテナ立ち上げ -->
docker-compose up -d

<!-- コンテナに入る -->
docke exec -it コンテナ名 bash

<!-- laravelプロジェクトとの作成 -->
<!-- laravel11代を指定して、srcにプロジェクトを作成 -->
conposer create-project "laravel/laravel=11.*" ./src 

<!-- DBの設定を.envに記述 -->
DB_CONNECTION=pgsql
DB_HOST=postgres
DB_PORT=5432
DB_USERNAME=postgres
DB_DATABASE=main
DB_PASSWORD=postgres

