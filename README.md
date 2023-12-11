
# Lampstack-Project

# Lamp-stack-Implementation
The LAMP stack is a popular open-source software stack used for building and deploying web applications. LAMP stands for Linux, Apache, MySQL, and PHP/Python/Perl. 

![Lampstack](./img/1.%20lamp-stack-img.png)

# Launch an EC2 instance
Elastic Compute Cloud (EC2) is a web service that offers resizable compute capacity in the cloud. EC2 allows you to run virtual servers, known as instances, on-demand. These instances can be easily scaled up or down based on the computing requirements.
[EC2 instance launch](./img/1.1%20launch%20an%20EC2%20instance.png)

# Creat keypair
Key pair is a set of security credentials that consists of a public key and a private key. Key pairs are used to securely connect to EC2 instances. When an EC2 instance is launched, you specify a key pair, and the public key is associated with the instance. The private key is kept secure and is used to authenticate and connect to the instance.
[keypair](./img/1.2create%20key%20pair.png)

# Instance Running
[](./img/1.3%20Instance%20running.png)

# Edit inbound rules to activate Port 80
Inbound rules refer to the rules that control incoming traffic to instances or resources. These rules are configured in security groups or network access control lists, which act as virtual firewalls to control the traffic to and from the instances.
![](<img/1.4 editing inbound rules.png>)

# Here's an overview of how the LAMP stack can be implemented:

## sudo apt update
 First run this command to update the local package repository cache. it downloads package information from all configured sources
![Sudo apt update](./img/sudo%20apt%20update.png)

## sudo systemctl status apache2
this command is used to check the status of the Apache HTTP server on a system that uses the systemd init system. This command provides information about whether the Apache service is running, stopped, or encountering any issue

## sudo apt install apache2
The sudo apt install apache2 command is used to install the Apache HTTP Server on a Debian-based Linux distribution, such as Ubuntu. This command will download and install the Apache web server and its dependencies from the distribution's package repositories.

![sudo apt install apache2](./img/4.Apache2default%20page%202.png)

# sudo systemctl status apache2
this command shows apache2 sttus, if its active and running
![sudo systemctl status apache2](./img/2.%20apache2%20installation.png)


## install mysql
## sudo apt install mysql-server

The sudo apt install mysql-server command is used to install the MySQL server on a Debian-based Linux distribution, such as Ubuntu. This command will download and install the MySQL server and its dependencies from the distribution's package repositorie

![sudo apt install mysql-server](./img/5.%20sql%20installation.png)

## sudo mysql
Running sudo mysql is a command to start the MySQL command-line client with superuser privileges
![sudo mysql](./img/6.wlcom%20to%20Sql.png)

## Sudo mysql_secure_installation
The sudo mysql_secure_installation command is used to secure your MySQL installation by performing various security-related tasks. When you run this command, you will be prompted to answer several questions and take several actions to enhance the security of your MySQL installation. this includes setting a root password, remove anonymous users, disallow root login remotely, remove the test database and reload privilege tables

![Sudo mysql_secure_installation](./img/7.2secure%20installation%20and%20password%20validation.png)

![Sudo mysql_secure_installation](./img/7.2secure%20installation%20and%20password%20validation.png)

# Install php

## sudo apt install php libapache2-mod-php php-mysql

The command sudo apt install php 
libapache2-mod-php php-mysql is used to install PHP and related modules on a Debian-based Linux distribution, such as Ubuntu. This command installs PHP, the Apache module for PHP, and the MySQL extension for PHP, enabling PHP to communicate with MySQL databases.

![sudo apt install php libapache2-mod-php php-mysql](<img/8. php installation.png>)

## php -v
The php -v command is used to check the version of PHP installed on your system. When you run this command in the terminal, it will display information about the PHP version currently installed.

![php -v](./img/9.%20php%20version.png)

## phpinfo
Snippet of PHP code.
This function outputs information about the PHP environment and its configuration. To see this information in a web browser, you typically create a PHP file with this content and access it through a web server.
![phpinfo](./img/10.php%20check.png)

![phpinfo](./img/10.2php%20check.png)

## Temporary landing page

# Creatind a Virtual Host for Website using Apache

First, set up a domain name called projectlamp

1. Navigate to Apache configuration directory

2. Creat  a virtual host configuration file

3. Enable the virtual host

4. Restart Apache

![](./img/16%20vh%20conf.png)

6. Test virtual host with your ipv4 address
![](./img/17.%20vh%20test.png)
