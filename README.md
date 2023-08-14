## Usage/Setup <br>
Setup the repository <br>
```
git clone https://github.com/Chriscoded/books-laravel-api.git
cd books-laravel-api
composer install
cp .env.example .env 
php artisan key:generate
php artisan cache:clear && php artisan config:clear 
php artisan serve 
```

## Database Setup <br>
We are going to pull in data from the database so make sure that you have your database setup
```
mysql;
create database bookstore;
exit;
```


Setup your database credentials in the .env file <br>
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=bookstore
DB_USERNAME={USERNAME}
DB_PASSWORD={PASSWORD}
```

Migrate the tables
```
php artisan migrate
```	



