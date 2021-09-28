# composer2spec

Quick and dirty script for converting PHP Composer packages into RPM packages.

## Usage

Run the `composer2spec` script with the name of a PHP composer package to
generate an `autoload.php` and a `.spec` file in the current directory.

Example:

```bash
composer2spec psr/http-message

ls
# autoload.php
# php-psr-http-message.spec
```

## Limitations

* only tested on a handful of small PHP packages
* makes some assumptions about the structure of the package source repos
* doesn't run tests

## Thanks

* [packagist.org](packagist.org)'s API for supplying the composer data
