![alt tag](https://raw.githubusercontent.com/JarJarBernie/jimmybox5/master/public/src/jimmybox.png)

# jimmybox5 1.0.2: PHP 5.6 developer box
vagrant box for PHP Developers with IonCube and Zend Guard Loader for professional E-Commerce development. Works with many applications and frameworks such as Oxid, Magento, Wordpress, Typo3 or Laravel 5.3.

## Quick Setup:
1) Get the latest Versions of Vagrant and Virtual Box

2) clone the latest version and run vagrant up
```bash
git clone https://github.com/JarJarBernie/jimmybox5.git .
vagrant up
```

3) open **192.168.33.12** in your browser


(IP can be changed in your Vagrantfile, the "public" directory is your document root)

## Made for PHP professionals and E-Commerce developers

Works out of the box with Oxid EE/PE, Shopware PE. Comes with Zend Guard Loader and IonCube Loader.

##### Performance: Try NFS share instead of the synced folder. Just uncomment in your Vagrantfile

### Oxid ready
- tested with Oxid EE 5.3.1
- tested with Oxid CE/PE 4.10.1

### Shopware ready
- tested with Shopware 5.2.9

### Magento ready
- tested with Magento 2.1

### Laravel ready
- tested with Laravel 5.3

### Typo3 6.2 ready
- tested with Typo3 6.2.27

## Features
- Ubuntu 14.04 LTS (Trusty Tahr)
- PHP 5.6.23
- MySQL 5.7
- IonCube Loader
- Zend Guard Loader
- Ruby 2.2.x
- Vim
- Git
- cURL
- GD and Imagick
- Composer
- Beanstalkd
- Node
- NPM
- Mcrypt

## MySQL Access

- Hostname: localhost or 127.0.0.1
- Username: root
- Password: root

## All features are based on scotch/box:
https://github.com/scotch-io/scotch-box

## Need the MySQL 5.7 strict SQL mode?
We have disabled the strict SQL mode for better compatibility with older apps. You can simplay enable it doing this:

```bash
vagrant ssh
sudo rm /etc/mysql/conf.d/disable_strict_mode.cnf
sudo service mysql restart
```
