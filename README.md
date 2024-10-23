# Coral Electronic Resource Management Installation Guide

Welcome to the Coral ERM Installation Guide! This guide will help you set up the environment and install prerequisites on Ubuntu using the terminal.

**Note:** Coral ERM is compatible with PHP versions 5.5, 5.6, and 5.7, as well as MySQL versions 5.6 and 5.7. In case of any issues or encountering a white screen, please ensure you are using the supported versions.

## Update and Upgrade Ubuntu

`sudo apt-get update`
`sudo apt-get upgrade`

## Install and Check Apache2 (Server) Status

`sudo apt-get install apache2`
`sudo systemctl status apache2`

## Add Repository for PHP 5.6

`sudo add-apt-repository ppa:ondrej/php`
`sudo apt-get update`

## Install PHP 5.6 and Its Modules

`sudo apt-get install -y php5.6`<br>
`php -v`<br>
`sudo apt-get install -y php5.6-cli php5.6-json php5.6-common php5.6-mysql php5.6-zip php5.6-gd php5.6-mbstring php5.6-curl php5.6-xml php5.6-bcmath php5.6-intl`<br>
`php -m`<br>
`sudo apt-get install php5.6-gettext`

##Add Repository for MySQL-5.7

`sudo add-apt-repository 'deb http://kr.archive.ubuntu.com/ubuntu xenial main'`

## Install MySQL-5.7 and Check Its Status

`sudo apt-get install aptitude`
`sudo aptitude install mysql-server-5.7 mysql-client-5.7`
`sudo systemctl status mysql`

## Enable Necessary PHP Modules for Coral

`sudo phpenmod mbstring`
`sudo phpenmod gettext`
`sudo phpenmod mysqlnd`

## Restart Apache2

`sudo systemctl restart apache2`


You've successfully set up the environment and installed prerequisites for Coral ERM on your Ubuntu system. Enjoy efficient resource management with Coral!

# Now Please follow the installation guide for installing CORAL20.09
