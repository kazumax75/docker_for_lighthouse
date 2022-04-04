LaravelのGraphQLライブラリlighthouseのテスト用に作ったdocker環境。
/src内に「laravel」フォルダとして下記リポジトリgit pullしておく。

lighthouse-example
https://github.com/nuwave/lighthouse-example

lighthouse-tutorial
https://github.com/nuwave/lighthouse-tutorial


・各種バージョン
PHP8.0
Composer version 2.3.3
mysql5.7

DBのホスト側ポートは4306

プレイグラウンドURL
http://127.0.0.1:8001/graphql-playground

.env.laravelは.envにリネームしてpull後にlaravelプロジェクトに置く良い


マイグレーション
php artisan migrate


ファクトリー
php artisan tinker
\App\Models\Comment::factory(10)->create()


========================================================

・注意点、ハマった罠
dc.ymlのMYSQL_PASSWORDとMYSQL_ROOT_PASSWORDに同じパスワードを入れるとエラーとなりdbコンテナが終了してしまう。
.envのDBユーザはMYSQL_USERを指定。rootユーザ指定するとマイグレーション実行時ユーザ権限SQLエラーが出る。

今まではdocker環境では共有のDBを使用してきたためDBコンテナ関係で躓きがちだったのでメモ＾＾；
