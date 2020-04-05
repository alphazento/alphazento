<p align="center">
 <svg
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 312 335"
    width="200"
    height="200"
    >
    <path
        id="Shape 2"
        style="fill: #2ab473;"
        d="M0 335C180.51 62.98 167 -94.55 187 64C207 222.55 79.46 227.14 172 225C264.54 222.86 14.02 306.65 115 301C215.98 295.35 437.27 284.27 219 313"
    />
    </svg>
</p>

<p align="center">
<!-- <a href="https://travis-ci.org/alphazento/ecommerce"><img src="https://travis-ci.org/alphazento/ecommerce.svg" alt="Build Status"></a> -->
<a href="https://packagist.org/packages/alphazento/ecommerce"><img src="https://poser.pugx.org/alphazento/ecommerce/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/alphazento/ecommerce"><img src="https://poser.pugx.org/alphazento/ecommerce/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/alphazento/ecommerce"><img src="https://poser.pugx.org/alphazento/ecommerce/license.svg" alt="License"></a>
</p>

## About Alphazento

Alphazento is a eCommerce framework base on Laravel. We're glad you chose to install Alphazento, a cutting-edge, feature-rich eCommerce solution that gets results.

## System Requirements

The Alphazento framework has a few system requirements:

-   PHP >= 7.2
-   Mcrypt PHP Extension
-   OpenSSL PHP Extension
-   Mbstring PHP Extension
-   Tokenizer PHP Extension

## Installation

Please install it via composer:

```shell
composer create-project alphazento/alphazento alphazento
```

## Configuration

Please refer to [Laravel Configuration](https://laravel.com/docs/5.0#configuration) and [Laravel Enviroment Configuration](https://laravel.com/docs/5.0/configuration#environment-configuration) to complete Alphazento initial configuration.

## Initialization

After DB connection is configurated in .env, you need to run command to initialize the system.

```
php artizan alphazento:init
```

The command will try to enable some necessary modules to the system.

And for more modules if you want to discover or enable them, these commands below will help:

```
php artizan package:discover
php artizan package:enable packagename
php artizan package:disable package_name
```

## Permissions

Alphazento may require some permissions to be configured: folders within storage and vendor require write access by the web server.

## Pretty URLs

#### Apache

The framework ships with a public/.htaccess file that is used to allow URLs without index.php. If you use Apache to serve your Laravel application, be sure to enable the mod_rewrite module.

If the .htaccess file that ships with Laravel does not work with your Apache installation, try this one:

```
Options +FollowSymLinks
RewriteEngine On

RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^ index.php [L]
```

#### Nginx

On Nginx, the following directive in your site configuration will allow "pretty" URLs:

```
location / {
    try_files $uri $uri/ /index.php?$query_string;
}
```

## Contributing

Thank you for considering contributing to the Alphazento framework! The contribution guide can be found in the Alphazento documentation.

## Security Vulnerabilities

If you discover a security vulnerability within Alphazento, please send an e-mail to Yongcheng Chen via alphazento88@gmail.com. All security vulnerabilities will be promptly addressed.

### License

The Alphazento framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
