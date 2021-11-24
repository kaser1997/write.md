#  `install laravel on windows`


 - Laravel is a php framework.
 - To install Laravel on your device, all you have to do is use Composer.
 - Documentation [Open](https://laravel.com/docs/8.x/installation)

##  install xampp [Dawnload](https://www.apachefriends.org/xampp-files/7.3.31/xampp-windows-x64-7.3.31-3-VC15-installer.exe)
- After installation, open xammp Then
- Start (Apache)
- start (mysql)

##  install Composer [Download](https://getcomposer.org/Composer-Setup.exe)

## install laravel
- open cmd Then
 -
        composer global require laravel/installer
 -   
        laravel new blog
    
- open folder The project from cmd
 
        php artisan serve 

[run](http://127.0.0.1:8000)


#  `Installing Laravel on Ubuntu` 


- Step 1: Log in via SSH and Update your System

      sudo apt-get update && sudo apt-get install mariadb-server mariadb-client


- Step 2: Install Apache and PHP

        sudo apt-get install php
-      
        sudo apt-get install cur
-        
        sudo apt-get install php7.1-zip
-        
        sudo apt-get install php7.1-mbstring
-       
        sudo apt-get install php-xml
        
        

- Step 3: Install Composer  [download](https://getcomposer.org/installer) 

        curl -sS https://getcomposer.org/installer | sudo php --
-

        composer
        
-

        sudo chown -R $ USER .composer /
        
- Step 4: Install Laravel Framework

        sudo apt-get install git
-        
        echo 'export PATH="$HOME/.composer/vendor/bin:$PATH"' >> ~/.bashrc
-        
        source ~/.bashrc


- Step 5: After executing the above command, you have to reopen the terminal again to install Laravel.
 Open a new terminal and run the command to install Laravel.

        composer global require "laravel/installer"



 - Step 6: Run Laravel command to create a new project.
       
         laravel new laravelpro
         
Go to the project folder.
 
         cd laravelpro
         
Run the command to start Laravel server
 
         php artisan serve
         
[Run](http://localhost:8000)
