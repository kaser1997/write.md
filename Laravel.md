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

        ssh root@IP_ADDRESS -p PORT_NUMBER

        apt-get update -y
        
        apt-get upgrade -y

- Step 2: Install Apache and PHP

        apt-get install apache2 php7.4 libapache2-mod-php7.4 php7.4-curl php-pear php7.4-gd php7.4-dev php7.4-zip php7.4-mbstring php7.4-mysql php7.4-xml curl -y

        systemctl start apache2

        systemctl enable apache2

- Step 3: Install Composer  [download](https://getcomposer.org/installer) 

        mv composer.phar /usr/local/bin/composer
        
        chmod +x /usr/local/bin/composer

- Step 4: Install Laravel Framework

        cd /var/www/html
        
        composer create-project laravel/laravel laravelapp --prefer-dist

        chown -R www-data:www-data /var/www/html/laravelapp
        
        chmod -R 775 /var/www/html/laravelapp/storage

- Step 5: Configure Apache to Serve Laravel App
Next, create a new Apache virtual host configuration file to serve the Laravel app.

        nano /etc/apache2/sites-available/laravel.conf

Add the following lines:

<VirtualHost *:80>
ServerName laravel.example.com
ServerAdmin admin@example.com
DocumentRoot /var/www/html/laravelapp/public
<Directory /var/www/html/laravelapp>
AllowOverride All
</Directory>
ErrorLog ${APACHE_LOG_DIR}/error.log
CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>

- Save and close the file when you are finished. Then, enable the Apache virtual host and rewrite module with the following command:
        
        a2ensite laravel.conf
        
        a2enmod rewrite
        
- Finally, restart the Apache service to implement the changes:   
        
        systemctl restart apache2
        
 - Step 6: Access Laravel App [RUN]( http://laravel.example.com.)
       
        
