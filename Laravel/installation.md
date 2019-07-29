# First steps to install Laravel (-V 5.4)

## Install Composer

Copy and paste this to get Composer installed:

> php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'a5c698ffe4b8e849a443b120cd5ba38043260d5c4023dbf93e1558871f1f07f58274fc6f4c93bcfd858c6bd0775cd8d1') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"

Then, run the following command to set it globally:

> mv composer.phar /usr/local/bin/composer

To check if everything is ok, type **composer** and you shoud get all the commands.