# PHP Concept

## Syntax

- [Syntax](#syntax)

## Output

- [echo](#echo)
- [print](#print)
- [var_dump](#var_dump)
- [Single quote Vs Double Quote](#single-quote-vs-double-quote)

## Variable And Data Types

- [String](#string)
- [Integer](#integer)
- [Float](#float)
- [Boolean](#boolean)
- [Constant](#constant)
- [Null](#null)
- [Heredoc](#heredoc)
- [Nowdoc](#nowdoc)
- [Array](#array)

## Comments

- [One-line Comments](#one-line-comments)
- [Multi-line Comments](#multi-line-comments)

## PHP Array

- [Index Array](#index-array)
- [Associative Array](#associative-array)
- [Multidimensional Array](#multidimensional-array)

## Operator

- [Arithemtic Operators](#arithemtic-operators)
- [Assigment Operators](#assigment-operators)
- [Comparison Operators](#comparison-operators)
- [Increment/Decrement Operators](#increment-decrement-operators)
- [Logical Operators](#logical-operators)
- [String Operators](#string-operators)

## Control Flow

- [if](#if)
- [if else](#if-else)
- [if elseif](#if-elseif)
- [switch](#if-elseif)
- [enum](#enum)

## Loop

- [for](#for)
- [while](#while)
- [do while](#do-while)
- [foreach](#foreach)
- [break](#break)
- [continue](#continue)

## Function

- [Build-in Function](#)
- [User Defined Function](#)
- [Parameters]()
- [Default Parameters]()
- [Named Arguments]()
- [Type Declarations]()
- [Strict Typing]()
- [Return]()
- [Variable Scopes]()
- [Lambda Function]()
- [Closures Function]()
- [Arrow Function]()

## Syntax

```php
<?php

?>
```

## echo

```php
echo "Hello PHP!"
```

## print

```php
print "Hello PHP!"
```

## var_dump

```php
var_dump("Hello PHP!");
```

## Single Quote Vs Double Quote

```php
$name = 'PHP';
echo "Hello $name";
echo 'Hello $name';
```

## String

```php
$msg = "Hello World!";
var_dump($msg);
```

## Integer

```php
$msg = 12345;
var_dump($msg);
```

## Float

```php
$msg = 12345.789;
var_dump($msg);
```

## Boolean

```php
$msg = true; // or $msg = false;
var_dump($msg);
```

## Constant

```php
define("NAME","Hello World!");
var_dump(NAME);
```

## Null

```php
$name = null;
var_dump($name);
```

## Heredoc

```php
<?php
echo <<<"FOOBAR"
Hello World!
FOOBAR;
?>
```

## Heredoc

```php
<?php
echo <<<'FOOBAR'
Hello World!
FOOBAR;
?>
```

## Array

```php
$msg = [1, 2, 3, 4, 5];
var_dump($msg);
```

## Index Array

```php
$array = array(1, 2, 3, 4, 5); // as of PHP 5.4
$array = [1, 2, 3, 4, 5];
```

## Associative Array

```php
$array = [
    "foo" => "bar",
    "bar" => "foo",
];
```

## Multidimensional Array

```php
$array = [
"foo" => "bar",
"bar" => [1, 2, 3, 4, 5],
"foobar" => [
        "foo" => "bar",
        "bar" => "foo",
    ]
];
```