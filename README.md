# A Small Docker LAMP stack
You never know when you need a LAMP stack. Here's a small LAMP stack that contains 2 containers

1. MYSQL (mysql:latest)
2. PHP + Apache (tutum/apache-php)

The PHP+Apache container has ports 80 and 443 exposed and is linked to MYSQL. Also worth mentioning is I mounted local volumes for both the Database and PHP container to make for easier tweaking. 

The local volumes are mounted locally inside your docker-compose directory.

* www - PHP application directory
* var - MYSQL files
