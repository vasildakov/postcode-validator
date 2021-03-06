# Postcode Validator

[![Build Status](https://travis-ci.org/vasildakov/postcode-validator.svg?branch=master)](https://travis-ci.org/vasildakov/postcode-validator)
[![Coverage Status](https://coveralls.io/repos/github/vasildakov/postcode-validator/badge.svg?branch=master)](https://coveralls.io/github/vasildakov/postcode-validator?branch=master)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/vasildakov/postcode-validator/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/vasildakov/postcode-validator/?branch=master)
[![Latest Stable Version](https://poser.pugx.org/vasildakov/postcode-validator/v/stable)](https://packagist.org/packages/vasildakov/postcode-validator)
[![Total Downloads](https://poser.pugx.org/vasildakov/postcode-validator/downloads)](https://packagist.org/packages/vasildakov/postcode-validator)
[![License](https://poser.pugx.org/vasildakov/postcode-validator/license)](https://packagist.org/packages/vasildakov/postcode-validator)


## Installation

The preferred method of installation is via [Packagist][] and [Composer][]. Run
the following command to install the package and add it as a requirement to
your project's `composer.json`:

```bash
composer require vasildakov/postcode-validator
```

## Examples

### Validate United Kingdom postcodes
```php
<?php

$validator = new Postcode\Validator('UK');

var_dump($validator->isValid('EC1V 9LB')); // true
var_dump($validator->isValid('ABC1 XYZ')); // false
```

### Validate Netherlands postcodes
```php
<?php

$validator = new Postcode\Validator('NL');

var_dump($validator->isValid('1012 JS')); // true
var_dump($validator->isValid('1234 JS')); // false
```

## License

Code released under [the MIT license](https://github.com/vasildakov/postcode-validator/blob/master/LICENSE)


[packagist]: https://packagist.org/packages/vasildakov/postcode-validator
[composer]: http://getcomposer.org/