# coding-guide

## Coding standard

Use the latest coding standard, at the moment of writing this is [PSR-12](https://www.php-fig.org/psr/psr-12/). Congirure your IDE to check this standard while developing. You can use [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer). 

## Tests

Make sure your application can be tested automatically.

## Strict typing

Use `declare(strict_types = 1);` at the top of every PHP file. [Strict typing](https://www.php.net/manual/en/language.types.declarations.php#language.types.declarations.strict)

### Return types

Use return types for methods 

    public function foo(): string
  
### Strong typed parameters

Use strong typed parameters in methods

    public function bar(string $foo, int $baz)
    
[Type declarations](https://www.php.net/manual/en/language.types.declarations.php)

## Smells

### Using CRUD controllers

Try to use only [CRUD](https://laravel.com/docs/8.x/controllers#actions-handled-by-resource-controller) methods in controllers. When using only CRUD methods the controller can't be bloated by to many methods. [Bloaters](https://refactoring.guru/refactoring/smells/bloaters)

### Small methods

Try to build as small as possible methods. [Long method](https://refactoring.guru/smells/long-method)

### Small classes

Try to build as small as possible classes. Big classes can 'wear to many hats'. [Large class](https://refactoring.guru/smells/large-class)

### Short parameter list

Try to use as little as possible parameters in methods. [Long parameter list](https://refactoring.guru/smells/long-parameter-list)
