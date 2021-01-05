# Project Setup

```
> composer create-project laravel/laravel="8.0.*" project_name
> composer create-project laravel/laravel project_name
```

```
> composer require laravel/ui
> composer require laravel/ui:^3.0
```

```
> composer require laravel/breeze --dev
> php artisan breeze:install
> php artisan ui vue --auth
```

```
> npm install && npm run dev
```


## .env update for database credentials

php artisan migrate


## xampp Setup 

- composer require
- php 7.3 require


### hosts File

```
127.0.0.1        local.app2104
```


### httpd-vhosts.conf

```
<VirtualHost *:80>   
	ServerName local.app2104
	DocumentRoot "C:\xampp\htdocs\app2104\public" 
</VirtualHost>
```


## Git Setup

```
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/primarypartition/app2104.git
git push -u origin main
```


## DB Fixes

```
app/Providers/AppServiceProvider.php file as follows:

use Illuminate\Support\Facades\Schema;

public function boot() 
{
    Schema::defaultStringLength(191); 
}
```


## Other

```
> php artisan server
> php artisan migrate
> php artisan migrate:fresh
> php artisan route:list
> php artisan make:controller CategoryController -r
> php artisan make:model Category -m
> php artisan storage:link
> php artisan make:middleware admin
> php artisan db:seed
> php artisan make:maik Sendmail
```

## UI

> https://github.com/mckenziearts/laravel-notify

> https://summernote.org/

> npm install @fontawesome/fontawesome-free


## Payment

```
https://dashboard.stripe.com/register
https://stripe.com/docs/stripe-js
https://stripe.com/docs/keys
https://github.com/cartalyst/stripe-laravel
https://cartalyst.com/manual/stripe-laravel/13.x
https://stripe.com/docs/testing

"cartalyst/stripe": "~2.0"
"cartalyst/stripe-laravel": "^13.0"
composer install && composer update
composer dump-autoload

```
