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

        composer global require laravel/installer
    
    `laravel new blog`
    
- open cmd and open Folder "blog"
 
    `php artisan serve`
    
    `http://127.0.0.1:8000`

## View

- open  (from  Folder "blog" )
 - 1-write (code .)
 - 2-All directions can be found in the following path: routes/web.php
 - 3-and write
 - 
     `Route::get('page-link' , function(){
   return "Hello World From Laravel";
});`

 - 4-open in Browser
    `http://127.0.0.1:8000/page-link`
    
