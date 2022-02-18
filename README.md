# project-2 : Installing LEMP stack
Step 1a: Updating, Upgrading and Installing nginx 
1. sudo apt update -y
2. sudo apt upgrade -y


![test](./images/update-upgrade.png)

Step 1b: Install nginx
1. sudo apt install nginx 
2. sudo systemctl status nginx

![test](./images/install-nginx.png

Step 2: Installing and Securing Mysql 
      
      1.Install Mysql by running:
        sudo apt install mysql-server

![test](./images/install-mysql-server.png)

2. Secure Mysql by running: 
          
    sudo mysql_secure_installation

![test](./images/mysql-secure.png)

MySQL server is now installed and secured. 
Next, we will install PHP

Step 3: Installing and configuring PHP to process code and generate dynamic content for the web server.

install the following 2 packages:

i. php-fpm 

ii.php-mysql

To install these 2 packages at once, run

sudo apt install php-fpm php-mysql

![test](./images/install-php.png)

Confirm installed php version by:
   
   php -v 
![test](./images/php-info.png)
We have successfully installed PHP and its components.

Next, we will configure Nginx to use the php processor.

Step 4 - Configuring Nginx to Use PHP Processor

Created a directory for projectLEMP using:

sudo mkdir /var/www/projectLEMP

![test](./images/sites-available.png)

![test](./images/sites-availablea.png)

Assign ownership to the directory 

$ sudo chown -R $USER:$USER /var/www/projectLEMP

![test](./images/chown-projectLEMP.png)

Step 5: Test PHP with Nginx
Created a test PHP file in the document root using nano text editor, this is to validate that Nginx can correctly hand .php files off to the PHP Processor

$ nano /var/www/projectLEMP/info.php

![test](./images/test-config.png)

STEP 6 – RETRIEVING DATA FROM MYSQL DATABASE WITH PHP
![test](./images/todo_list.png)


![test](./images/todo-list.png)


