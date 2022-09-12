# LEMP STACK IMPLEMENTATION
Joseph Akinrinmade's Freestyle Project

## Connected to EC2 instance via GitBash

I spun a new EC2 instance, downloaded and installed Mobaxterm with my WSL2. Then I connect to the same ubuntu server via SSH

## Installed the Nginx web server

I installed the Nginx web server by using the following command:
> sudo apt update 
> sudo apt install nginx
- <img src="images/p2%20nginx.png" width="650">
I also added a rule to the EC2 configuration to open inbound connection through port 80 and then, was now able to access the web server.

## Installed MySQL as confirmed below
- <img src="images/p2_mysql.png" width="650">

## Installed PHP by using the command - sudo apt install php-fpm php-mysql
- <img src="images/p2_instalphp.png" width="650">

## Configured Nginx to use the PHP processor
First, I created a directory for the new Project. i.e. ProjectlEMP with this command
 > $sudo mkdir /var/www/projectlEMP

Next, I assigned ownership of the directory with the $ USER environment variable by entering the following command

 ==$sudo chown -R $USER:$USER /var/www/projectlEMP==

- On using the echo command, it resulted in the following:
- <img src="images/p2%20config_nginx.png" width="650">

- <img src="images/p2_confignginx.png" width="650">

### Tested out PHP with Nginx
- <img src="images/p2_nginxservephp.png" width="650">

## created and retrived data from a new database I just created
- <img src="images/p2_mysqlUserCreate.png" width="650">

## Created a todo_list on PHP

- <img src="images/p2_mysqlpopulated.png" width="650">

## Tested the connection and all worked as expected
- <img src="images/p2_phpqueriesdb.png" width="600">
