【使用リポジトリについて】
・
・



【環境構築について】
1. フォルダを作成し、下記のような配置にします。
pinos_room(任意の名前)
    ├── backend
    ├── frontend
    └── docker-compose.yml

※docker-compose.ymlはbackendリポジトリに配置されているため、上記のように移動する。



2. pinos_roomディレクトリにて、初回ビルドコマンドを実行します。
- docker-compose build


上記コマンドにて、下記のコンテナが作成・起動されます。
・frontend
・backend
・db



【backendのセットアップ】

1. 下記コマンドを実行します。
- docker compose exec backend bash
- composer install
（backendコンテナ内で実行）


2. http://localhost:8080 にアクセスし、Laravelのデフォルト画面が表示されることを確認します。


laravelのセットアップは完了です。




【frontendのセットアップ】

1. http://localhost:3000にアクセスし、Next.jsのデフォルト画面が表示されることを確認します。
