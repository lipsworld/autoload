# WordPress Autoload

[![Build Status](https://travis-ci.org/wpup/autoload.svg?branch=master)](https://travis-ci.org/wpup/autoload)
[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)

Simple autoloader that will autoload classes, interfaces or traits with namespace prefix

# Install

```
composer require frozzare/wp-autoload
```

## Example

Example of your main php file.

```php
require 'vendor/autoload.php';
register_wp_autoload( 'Example\\', __DIR__ . '/src' );
```

Example of `src/class-plugin-loader.php`

```php
namespace Example;
class Plugin_Loader {}
```

Example of `src/trait-crawler.php`

```php
namespace Example;
trait Crawler {}
```

Example of `src/interface-say.php`

```php
namespace Example;
interface Say {}
```

## License

MIT © [Fredrik Forsmo](https://github.com/frozzare)
