Caffeinated Modules
===================
[![Laravel 5.0](https://img.shields.io/badge/Laravel-5.0-orange.svg?style=flat-square)](http://laravel.com)
[![Laravel 5.1](https://img.shields.io/badge/Laravel-5.1-orange.svg?style=flat-square)](http://laravel.com)
[![Source](http://img.shields.io/badge/source-caffeinated/modules-blue.svg?style=flat-square)](https://github.com/caffeinated/modules)
[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](https://tldrlegal.com/license/mit-license)

Caffeinated Modules is a simple package to allow the means to separate your Laravel 5 application out into modules. Each module is completely self-contained allowing the ability to simply drop a module in for use. Caffeinated Modules supports both Laravel 5.0 and 5.1.

The package follows the FIG standards PSR-1, PSR-2, and PSR-4 to ensure a high level of interoperability between shared PHP code. At the moment the package is not unit tested, but is planned to be covered later down the road.

Documentation
-------------
You will find user friendly and updated documentation in the wiki here: [Caffeinated Modules Wiki](https://github.com/caffeinated/modules/wiki)

Quick Installation
------------------
Begin by installing the package through Composer. Depending on what version of Laravel you are using (5.0 or 5.1), you'll want to pull in the `~1.0` or `~2.0` release, respectively:

#### Laravel 5.0.x
```
composer require caffeinated/modules=~1.0
```

#### Laravel 5.1.x
```
composer require caffeinated/modules=~2.0
```

Once this operation is complete, simply add both the service provider and facade classes to your project's `config/app.php` file:

#### Laravel 5.0.x
##### Service Provider
```php
'Caffeinated\Modules\ModulesServiceProvider',
```

##### Facade
```php
'Module' => 'Caffeinated\Modules\Facades\Module',
```

#### Laravel 5.1.x
##### Service Provider
```php
Caffeinated\Modules\ModulesServiceProvider::class,
```

##### Facade
```php
'Module' => Caffeinated\Modules\Facades\Module::class,
```

And that's it! With your coffee in reach, start building out some awesome modules!
