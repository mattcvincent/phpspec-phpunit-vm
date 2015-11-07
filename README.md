# Quickstart 
A PHP starter project with phpspec, PHPUnit, and the Homestead Vagrant virtual machine

Use this project to quickly boostrap a new PHP project.

##Requirements:

- [PHP >= 5.5](http://www.php.net)
- [Vagrant](https://www.vagrantup.com/downloads.html)
- [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
- [Composer](https://getcomposer.org/download/)

##Directions:

###Clone this project

`git clone git@github.com:gcummins/phpspec-phpunit-vm.git quickstart`

###Change to the project directory

`cd quickstart`

###Install the dependencies

`composer install`

###Prepare the virtual machine

```
php vendor/bin/homestead make
vagrant up
```

###Point the test domain to the virtual machine
Add this line to your hosts file:

`192.168.10.10 homestead.app`

On OS X and Linux, the hosts file is at:

`/etc/hosts`

On Windows, the hosts file is at:

`C:\Windows\System32\drivers\etc\hosts`

###Put your code in public/index.php

The virtual machine will look for code in that location.

###View your application in a browser
Browse to http://homestead.app
