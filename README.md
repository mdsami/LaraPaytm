# LaraPaytm
Paytm Integration with Laravel

[![Latest Stable Version](https://poser.pugx.org/mdsami/LaraPaytm](https://packagist.org/packages/mdsami/LaraPaytm)
[![Total Downloads](https://poser.pugx.org/amdsami/LaraPaytm/downloads)](https://packagist.org/packages/mdsami/LaraPaytm)
[![License](https://poser.pugx.org/mdsami/LaraPaytm/license)](https://packagist.org/packages/mdsami/LaraPaytm)



For Laravel 5.6 and above

## Introduction
Integrate Paytm wallet in your laravel application easily with this package. This package uses official Paytm PHP SDK's.

## License
Laravel Paytm Wallet open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)

## Getting Started
To get started add the following package to your `composer.json` file using this command.

    composer require mdsami/LaraPaytm

## Configuring
**Note: For Laravel 5.5 and above auto-discovery takes care of below configuration.**

When composer installs Laravel Paytm Wallet library successfully, register the `MdSami\LaraPaytm\LaraPaytmServiceProvider` in your `config/app.php` configuration file.

```php
'providers' => [
    // Other service providers...
    MdSami\LaraPaytm\LaraPaytmServiceProvider::class,
],
```
Also, add the `PaytmWallet` facade to the `aliases` array in your `app` configuration file:

```php
'aliases' => [
    // Other aliases
    'PaytmWallet' => MdSami\LaraPaytm\Facades\PaytmWallet::class,
],
```
#### Add the paytm credentials to the `.env` file