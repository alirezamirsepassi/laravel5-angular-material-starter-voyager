# laravel5-angular-material-starter-voyager 
you can use this https://github.com/followtheart/laravel5-angular-material-starter-voyager.git  directly,
Or you can do it yourself, just follow steps below:

# Step 1, laravel5-starter
Also see here :https://laravel-angular.readme.io/docs
```bash
git clone https://github.com/jadjoubran/laravel5-angular-material-starter.git
cd laravel5-angular-material-starter
npm install -g gulp bower
npm install
bower install
#fix database credentials in .env
php artisan migrate
gulp
```
# Step 2, voyager
Also see here: https://github.com/the-control-group/voyager
```bash
composer require tcg/voyager
```

Next make sure to create a new database and add your database credentials to your .env file:

```
DB_HOST=localhost
DB_DATABASE=homestead
DB_USERNAME=homestead
DB_PASSWORD=secret
```

Add the Voyager service provider to the `config/app.php` file in the `providers` array:

```php
'providers' => [
    // Laravel Framework Service Providers...
    //...
    
    // Package Service Providers
    TCG\Voyager\VoyagerServiceProvider::class,
    // ...
    
    // Application Service Providers
    // ...
],
```

Lastly, we can install voyager by running

```bash
php artisan voyager:install
```

# extra steps:
```php
##(ONLY IN STARTER!!)  
php artisan migrate:refresh
php artisan db:seed --class=VoyagerDatabaseSeeder
```
# run server
```php
php artisan serve 
```









----------------------------------------------------------------------------------------------------

## Laravel 5.3 Angular Material Starter

[![Latest Stable Version](https://poser.pugx.org/jadjoubran/laravel5-angular-material-starter/v/stable)](https://packagist.org/packages/jadjoubran/laravel5-angular-material-starter)
[![Latest Unstable Version](https://poser.pugx.org/jadjoubran/laravel5-angular-material-starter/v/unstable)](https://packagist.org/packages/jadjoubran/laravel5-angular-material-starter)
[![Build Status](https://travis-ci.org/jadjoubran/laravel5-angular-material-starter.svg?branch=master)](https://travis-ci.org/jadjoubran/laravel5-angular-material-starter)
[![StyleCI](https://styleci.io/repos/34944760/shield?style=flat)](https://styleci.io/repos/34944760)
[![Code Climate](https://codeclimate.com/github/jadjoubran/laravel5-angular-material-starter/badges/gpa.svg)](https://codeclimate.com/github/jadjoubran/laravel5-angular-material-starter)
[![License](https://poser.pugx.org/jadjoubran/laravel5-angular-material-starter/license)](https://packagist.org/packages/jadjoubran/laravel5-angular-material-starter)
[![Join the chat at https://gitter.im/jadjoubran/laravel5-angular-material-starter](https://badges.gitter.im/jadjoubran/laravel5-angular-material-starter.svg)](https://gitter.im/jadjoubran/laravel5-angular-material-starter?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

![Laravel & Angular](http://i.imgur.com/CwQy3Il.png)


## Demo

An online <a href="http://www.laravel-angular.io/" target="_blank">demo</a> is available.


## Docs

[View Latest Docs](http://laravel-angular.readme.io/) for installation steps & tutorials.



Running on 3.2? Here are the [3.2 Docs](https://laravel-angular.readme.io/v3.2)

## Laravel 5 & Angular 2

Join the discussion on
- [Laravel & Angular](https://github.com/jadjoubran/laravel-angular)
- [Angular & Laravel](https://github.com/jadjoubran/angular-laravel)

## Screencasts

Screencasts on [Youtube](https://www.youtube.com/c/LaravelAngularMaterialStarter).


## Issues, questions and feature requests
Open a new issue, I'd love to help.



## Do It Yourself (Outdated)

A nice article on <a href="http://www.sitepoint.com/flexible-and-easily-maintainable-laravel-angular-material-apps/" target="_blank">sitepoint</a> that explains the first few versions of this repository. Recommended read if you're not familiar with the underlying technologies.


## Contributing

Thank you for contributing to this repository.

Here are the guidelines:

1. If you are adding/modifying backend functionality, make sure to include the appropriate `test`. Let me know if you need help writing the test.
