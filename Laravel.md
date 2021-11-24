#  install laravel for windows


 - Laravel is a php framework.
 - To install Laravel on your device, all you have to do is use Composer.
 - Documentation [Download](https://laravel.com/docs/8.x/installation)

##  install xampp [Dawnload](https://www.apachefriends.org/xampp-files/7.3.31/xampp-windows-x64-7.3.31-3-VC15-installer.exe)
- After installation, open xammp Then
- Start (Apache)
- start (mysql)

##  install Composer [Download](https://getcomposer.org/Composer-Setup.exe)

## install laravel
- open cmd Then

        composer global require laravel/installer
 -   
        laravel new blog
    
- open folder The project from cmd
 
        php artisan serve 

[run](http://127.0.0.1:8000)

## View

- open  (from  Folder "blog" )
 - 1-write (code .)
 - 2-All directions can be found in the following path: routes/web.php
 - 3-and write
 - 
         Route::get('page-link' , function(){
         return "Hello World From Laravel";
         });

 - 4- [open](http://127.0.0.1:8000/page-link)
    
