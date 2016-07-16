# behat_test1
```
{
  "require-dev": {
    "behat/behat": "~3.1.0",
    "behat/mink": "~1.7.1",
    "behat/mink-extension": "~2.2",
    "behat/mink-goutte-driver": "~1.2.1",
    "behat/mink-selenium2-driver": "~1.3.1",
    "peridot-php/webdriver-manager": "~1.3.0",
    "bossa/phpspec2-expect": "~1.0.3"
  },
  "config": {
    "bin-dir": "bin"
  }
}


https://packagist.org/packages/behat/behat
(Scenario-oriented BDD framework for PHP 5.3)

https://packagist.org/packages/behat/mink
(Browser controller/emulator abstraction for PHP)

https://packagist.org/packages/behat/mink-extension
(Mink extension for Behat)

https://packagist.org/packages/behat/mink-goutte-driver
(Goutte driver for Mink framework)

https://packagist.org/packages/behat/mink-selenium2-driver
(Selenium2 (WebDriver) driver for Mink framework)

https://packagist.org/packages/peridot-php/webdriver-manager
(Library and command line tool for managing Selenium WebDriver)

https://packagist.org/packages/bossa/phpspec2-expect
(Helper that decorates any SUS with a phpspec lazy object wrapper)


composer install

./bin/manager update

./bin/manager

./bin/manager status


sanjay@sanjay-desktop:/var/www/behat_test1$ ./bin/behat --init
+d features - place your *.feature files here
+d features/bootstrap - place your context classes here
+f features/bootstrap/FeatureContext.php - place your definitions, transformations and hooks here


sanjay@sanjay-desktop:/var/www/behat_test1$ ll
total 112
drwxrwsr-x  5 sanjay www-data  4096 Jul 16 10:07 ./
drwxrwsr-x 21 sanjay www-data  4096 Jul 16 08:33 ../
-rw-rw-r--  1 sanjay www-data   194 Jul 16 10:06 behat.yml
drwxrwsr-x  2 sanjay www-data  4096 Jul 16 09:39 bin/
-rw-rw-r--  1 sanjay www-data   332 Jul 16 09:38 composer.json
-rw-rw-r--  1 sanjay www-data 84156 Jul 16 09:39 composer.lock
drwxrwsr-x  3 sanjay www-data  4096 Jul 16 10:07 features/
drwxrwsr-x 18 sanjay www-data  4096 Jul 16 09:39 vendor/



sanjay@sanjay-desktop:/var/www/behat_test1$ tree -L 1 features/
features/
-- bootstrap

1 directory, 0 files


Open /bootstrap/FeatureContext.php


Run "./bin/behat" on command line
you will see all the features



./bin/behat --append-snippets
will add the features to the FeatureContext.php file


Add the mink context in the FeatureContext.php
use Behat\MinkExtension\Context\RawMinkContext;

and extend RawMinkContext


modify content of iAmInWikipedia()

start selenium driver
./bin/manager start


change the browser to chrome in yml file
```







