-What is Laravel?
*Laravel is a php framework
*Laravel is based on the famous MVC method that separates the Model
 from the View from the Controller, 
providing you with a smooth and easy working environment.



-Install Laravel on your device
*To install Laravel on your device, 
all you have to do is use Composer 
(composer is a package manager for PHP,
 what Composer does is collect all the packages you need and manage them 
from one place,
 which facilitates the development process, 
especially the joint development process among members of a work team

*Composer's package management is not a new concept in the programming world,
 in fact many composer services are inspired by Node.js's npm and Ruby's Bundler).

-How to install Composer

*(To install Composer on Windows, all you have to do is go to the official website:
 https://getcomposer.org/ 
and download the installation package from the official website
 and install it like any normal program.)

-How to install Composer (linux)
To install through the command line (Terminal)

$ curl -s https://getcomposer.org/installer | php

This line enables you to download composer.phar . file

$ sudo mv composer.phar /usr/local/bin/composer
In this line, we move the file to the bin path so that it will be circulated 
to the entire system

This command will install a composer in your operating system, 
then you can easily work on a composer and update packages 
or add them to a specific project you have.

$ composer


-We return to the installation of Laravel on your device 
and type the following command

A new package will be installed on your device
 for use in installing Laravel projects using the following command

composer global require laravel/installer

-This command will create a folder called Blog in the current directory 
and create a Laravel project in it


laravel new blog


-And you can choose the process of installing a Laravel package on your device
 and create a Laravel project directly using Composer

composer create-project --prefer-dist laravel/laravel blog


-All you have to do is, using the Command Line, whatever you prefer to use
, go to the project via the cd command, 
and when you reach it, type the following command:
 to run the server


php artisan serve


-The project link will appear to you, 
open it in your browser and your first project using Laravel will appear,
and the link is often as follows


http://localhost:8000

http://127.0.0.1:8000









