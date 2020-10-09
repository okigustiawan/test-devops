###  6. Install aplikasi web server di komputer kamu, kemudian install php di web server tersebut (dilarang menggunakan aplikasi seperti xampp, lampp).

###Install webserver apache

$ sudo apt-get update
$ sudo apt-get install -y apache2 (menggunakan webserver apache)
$ sudo apache2ctl configtestOutput

Syntax OK

$ sudo nano /etc/apache2/apache2.conf

Tambahkan perintah ini pada akhir baris, ip address bisa diisi dengan 127.0.0.1 atau ip statis server.ServerName 

$ sudo ufw app listOutput
Available applications:
  Apache
  Apache Full
  Apache Secure
  OpenSSH

$ sudo service apache2 start
http://localhost/

###Install MySql

$ sudo apt-get install mysql-server
$ sudo service mysql start

###Install Php

sudo apt update
sudo apt install -y build-essential
sudo apt install php php-pear php-dev libmcrypt-dev
sudo pecl install mcrypt
sudo apt-get install php libapache2-mod-php php-mcrypt php-mysql
cd /var/www/html
sudo vim test.php
isi:
	<?php 
		phpinfo(); 
	?>

http://localhost/test.php
