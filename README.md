Laravel 9

1. Clone repository
   1.1 Jika menggunakan SSH
   git clone git@github.com:yprogrammerID/base-code-laravel-9.git laravel9
   1.2 Jika menggunakan HTTPS
   git clone https://github.com/yprogrammerID/base-code-laravel-9.git laravel9
2. cd laravel9
3. duplicate .env.example
4. rename '.env.example copy' to .env
5. docker run --rm \
   -u "$(id -u):$(id -g)" \
   -v $(pwd):/var/www/html \
   -w /var/www/html \
   laravelsail/php81-composer:latest \
   composer install --ignore-platform-reqs
6. sail up -d atau ./vendor/bin/sail up -d
7. sail artisan key:generate
