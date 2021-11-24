#  install laravel for windows


 - Laravel is a php framework.
 - To install Laravel on your device, all you have to do is use Composer.
 - Documentation
  `https://laravel.com/docs/8.x/installation`
## Contents

[TOC]

##  install Composer
`https://getcomposer.org/Composer-Setup.exe`

## install laravel
- open cmd and write
 - 1-`composer global require laravel/installer`
 - 2-`laravel new blog`
- open cmd and open Folder "blog"
 - 3-`php artisan serve`
 - 4-`http://127.0.0.1:8000`

## View

- open code . (from  Folder "blog" )
 - 1-All directions can be found in the following path: routes/web.php
 - 2-and write
 `Route::get('page-link' , function(){
   return "Hello World From Laravel";
});`
 - 3-open in Browser
 - `http://127.0.0.1:8000/page-link`
