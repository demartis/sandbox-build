# Doctrine Database Migrations

## Status

[![Build Status](https://travis-ci.org/doctrine/migrations.svg)](https://travis-ci.org/doctrine/migrations)
[![Dependency Status](https://www.versioneye.com/php/doctrine:migrations/badge.svg)](https://www.versioneye.com/php/doctrine:migrations/)


## Official Documentation

All available documentation can be found [here](http://docs.doctrine-project.org/projects/doctrine-migrations/en/latest/).

The repository containing the documentation is [there](https://github.com/doctrine/migrations-documentation).

## Working with Doctrine Migrations
    
### Using the integration of your framework

  * symfony 2 [doctrine/doctrine-migrations-bundle](https://packagist.org/packages/doctrine/doctrine-migrations-bundle)
  * ZF2 [doctrine/doctrine-orm-module](https://packagist.org/packages/doctrine/doctrine-orm-module) 
  * laravel [mitchellvanw/laravel-doctrine](https://packagist.org/packages/mitchellvanw/laravel-doctrine)
  * Silex [kurl/silex-doctrine-migrations-provider](https://packagist.org/packages/kurl/silex-doctrine-migrations-provider)
  * nette [zenify/doctrine-migrations](https://packagist.org/packages/zenify/doctrine-migrations)
  * others...
        
### Using composer
            
```composer require doctrine/migrations```
        
### Downloading the latest phar release

You can download the [doctrine migrations phar](https://github.com/doctrine/migrations/releases) directly on the release page

### Building Your own Phar

Make sure Composer and all necessary dependencies are installed:

```bash
curl -s https://getcomposer.org/installer | php
php composer.phar install --dev
```

Make sure that the Box project is installed:

```bash
curl -s http://box-project.org/installer.php | php
```

Build the PHAR archive:

```bash
php box.phar build
```

The `doctrine-migrations.phar` archive is built in the `build` directory.

#### Creating archive disabled by INI setting

If you receive an error that looks like:

    creating archive "build/doctrine-migrations.phar" disabled by INI setting

This can be fixed by setting the following in your php.ini:

```ini
; http://php.net/phar.readonly
phar.readonly = Off
```

## Installing Dependencies

To install dependencies run a composer update:

```composer update```
