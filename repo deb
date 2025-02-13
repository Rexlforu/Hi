1.	install ssh
	- apt install openssh-server
	- configure

2.	aplikasi tambahan
	- apt install links
	- apt install wget
	- apt install unzip

2.	web server
	- apt install nginx
	- configure nginx (port, virtualhost)

3.	php8.0
	- apt install ca-certificates apt-transport-https curl lsb-release
	- curl -fsSL http://packages.sury.org/php/README.txt | bash
	- apt install php8.0-fpm
	- cek versi php (php -v)
	- pico infophp.php (/var/www/html)
=============
<?php
phpinfo();
?>
=============
	enable display_errors
	/etc/php/8.0
	- nano /fpm php.ini
	- nano /fpm php.ini

4.	database server
	- apt install php8.0-mysql
	- apt install php8.0-intl
	- apt install php8.0-gd
	- apt install php8.0-mbstring
	- apt install php8.0-curl
	- apt install php8.0-zip
	- apt install php8.0-simpleXML
	- apt install mariadb-server mariadb-client

5.	konfigurasi database
	mysql (untuk masuk ke database)
	exit (untuk keluar)
	show databases; (untuk melihat isi database)

	- ALTER USER 'root'@'localhost' IDENTIFIED BY 'sani';
	- FLUSH PRIVILEGES; (lock akses root)
	- mysql -u root -p (login sebagai root)
	- CREATE DATABASE sani; (membuat database)
	- CREATE USER 'sani'@'localhost' IDENTIFIED BY 'sani'; (membuat user)
	- GRANT ALL PRIVILEGES ON sani.* TO 'sani'@'localhost'; (memberi user akses untuk database)
	- FLUSH PRIVILEGES; 

6.	php-2
	/var/www/html
	- rm index.nginx-debian.html
	- pico connect-db.php

script:
=========================================================================
<?php
$servername = "localhost";
$username = "sani";
$pswd = "sani";
$database = "sani";

$connection = mysqli_connect($servername, $username, $pswd, $database);

if (!$connection) {
            die("kok gabisa bjirr".mysqli_connect_error()) ;
}

echo "KONEK GINI NJIR, PALALU BAU NUGGET";
mysqli_close($connection) ;

?>
===========================================================================

7.	Prestashop
	- wget https://ukk25.smekindo.site/prestashop_8.2.0.zip
	- unzip prestashop_8.2.0.zip
	- rm index.php
	- unzip prestashop.zip
	- chmod 755 -R *
	  chown www-data:www-data -R *
	refresh webserver dan selesaikan konfigurasi 
	- rm -rf install/
	- mv admin/ etmin/
	

END-
