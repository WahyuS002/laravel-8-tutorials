<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## Fitur Baru Laravel 8

- Model mempunyai sebuah folder
- Fitur [maintenance](https://laravel.com/docs/8.x/configuration#maintenance-mode) sekarang lebih keren bisa di cek juga menggunakan artisan `php artisan down --help`
- Factory laravel 8 sekarang telah memiliki class, dan cara penggunaan factory berbeda dari yang versi sebelumnya
    - Sebelumnya `factory('App\User', 5)->create();`
    - Sekarang `User::factory()->count(5)->make();`
- Syntax route berubah
    - Sebelumnya `Route::get('welcome', 'WelcomeController@index);`
    - Sekarang `Route::get('welcome', [WelcomeController::class, 'index']);
    
    ```
    Note :
    Perubahan syntax route terjadi karena di RouteServiceProvider.php tidak disediakan variable $protected namespace
    ```
