# 初めに
composer update
php artisan migrate
npm install
npm run build

# 開発
php artisan make:controller IndexController --resource


public function index() {
    // print("<h1>こんにちは！ Laravel です！</h1>");
    return view('index', ['message' => 'こんにちは', 'name' => '山田']);
}

# マイグレーション
php artisan make:migration create-books-table --create=books

php artisan migrate

モデルの作成
php artisan make:model Book;
