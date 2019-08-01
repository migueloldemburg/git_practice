# First steps to install Laravel (-V 5.4)

## Pre-Requisites

In order to install Laravel you need to:

Install Mbstring PHP Extension
> sudo apt-get install php7.0-mbstring

The XML PHP Extension
> sudo apt-get install php-xml

And the ZIP PHP Extension
> sudo apt-get install php7.0-zip

## Installing Composer

Copy and paste this to get Composer installed:
> php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'a5c698ffe4b8e849a443b120cd5ba38043260d5c4023dbf93e1558871f1f07f58274fc6f4c93bcfd858c6bd0775cd8d1') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"

Then, run the following command to set it globally:
> mv composer.phar /usr/local/bin/composer

To check if everything is ok, type **composer** and you shoud get all the commands.
> composer

Change the permissions to run the composer command without sudo
> *sudo chown -R $USER ~/.composer/*

## Installing Laravel

First, download the Laravel installer using Composer:
> composer global require "laravel/installer"

Make sure to place the **export PATH="$HOME/.composer/vendor/bin:$PATH"**  in your **$PATH** so the laravel executable can be located by your system
> *echo 'export PATH="$HOME/.composer/vendor/bin:$PATH"' >> ~/.bashrc*
> *source ~/.bashrc*

Restart the terminal.
And initialize a Laravel project.
> laravel new blog

Alternatively, you may also install Laravel by issuing the Composer create-project command in your terminal:
> *composer create-project --prefer-dist laravel/laravel blog "5.4.*"*

Run the Laravel server. Enjoy!
> php artisan serve