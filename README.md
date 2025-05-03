DB_CONNECTION=mysql
DB_HOST=db
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=laravel
DB_PASSWORD=secret

docker-compose up -d --build

docker exec -it laravel_app bash
php artisan migrate
