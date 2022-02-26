# PHP Concept

## Syntax

- [Syntax](#syntax)

## Output

- [echo](#echo)
- [print](#print)
- [var_dump](#vardump)
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
- [match (PHP 8)](#match)

## Loop

- [for](#for)
- [while](#while)
- [do while](#do-while)
- [foreach](#foreach)
- [break](#break)
- [continue](#continue)

## Function

- [Build-in Function](#)
- [User Defined Function](#user-defined-function)
- [Parameters](#parameters)
- [Default Parameters](#default-parameters)
- [Named Arguments (PHP 8)](#named-arguments)
- [Type Declarations (PHP 7.4)](#type-declarations)
- [Return](#return)
- [Variable Scopes](#variable-scopes)
- [Lambda Function](#lambda-function)
- [Closures Function](#closures-function)
- [Arrow Function (PHP 7.4)](#arrow-function)

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

## NowDoc
```php
<?php
echo <<<'FOOBAR'
Hello World!
FOOBAR;
?>
```

## One-line Comments

```php
// This is one line comments
# This is one line comments
```

## Multi-line Comments

```php
/*
This is 
multi line comments
*/
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

## Arithmetic operators

```php
echo 5 + 3;     // prints 8
echo 5 - 3;     // prints 2
echo 5 * 3;     // prints 15
echo 6 / 3;     // prints 2
echo 6 % 3;     // prints 0
```

## Assignment operators

```php
$a = 3;
$a += 5; // sets $a to 8, as if we had said: $a = $a + 5;
$b = "Hello ";
$b .= "There!"; // sets $b to "Hello There!", just like $b = $b . "There!";
```

## Comparison operators

```php
var_dump(1 == 1); // true
var_dump(1 != 2); // false
var_dump(1 > 2); // false
var_dump(1 < 2); // true
var_dump(1 >= 2); // false
var_dump(1 <= 2); // true
```

## Increment/Decrement operators

```php
// increment
$i = 1;
echo $i; // 1
$i += 1;
echo $i; // 2
$i++;
echo $i; // 3
echo ++$i; // 4

// decrement
$i = 5;
echo $i; // 5
$i -= 1;
echo $i; // 4
$i--;
echo $i; // 3
echo --$i;  //2
```

## Logical operators

```php
var_dump(false and true); // false
var_dump(false or true); // true
var_dump(false && true); // false
var_dump(false || true); // true
```

## String operators

```php
$a = "Hello ";
$b = $a . "World!"; // now $b contains "Hello World!"

$a = "Hello ";
$a .= "World!";     // now $a contains "Hello World!"
```

## if

```php
if(boolean) {
    // do something
}

if(true) {
    echo "Hello World!";
}
```

## if else

```php
$score = 50;
if($score >= 40) {
    echo "Pass";
} else {
    echo "Failed";
}
```

## if elseif

```php
$age = 50;
if($age < 18) {
    echo "Young";
} else if($age < 40) {
    echo "Adult";
} else {
    echo "Old";
}
```

## switch

```php
$day = 1
switch ($day) {
    case 0:
        echo "Sunday";
        break;
    case 1:
        echo "Monday";
        break;
    case 2:
        echo "Tuesday";
        break;
}
```

## match

```php
// PHP 8
$food = 'cake';

$return_value = match ($food) {
    'apple' => 'This food is an apple',
    'bar' => 'This food is a bar',
    'cake' => 'This food is a cake',
};

var_dump($return_value);
```

## User Defined Function

```php
function greeting() {
    echo "Hello World!";
}
```

## Parameters

```php
function greeting($name) {
    echo "Hello $name";
}
```

## Default Parameters

```php
function greeting($name = "World") {
    echo "Hello $name";
}
```

## Named Arguments

```php
function greeting($name = "World") {
    echo "Hello $name";
}
greeting(name: "Mg Mg");
```

## Type Declarations

```php
function greeting(string $name) {
    echo "Hello $name";
}
```

## Return

```php
function greeting(string $name) {
    return "Hello $name";
}
echo greeting("World");
```

## Variable Scopes

```php
$name = "Mg Mg"  // Global scope
function greeting() {
  $name = "Aung Aung"; // local scope
  echo "Hello $name";
}
```

## Lambda Function

```php
$greeting = function() {
    echo "Hello World!";
}
$greeting();
```

## Closures Function

```php
$name = "World!";
$greeting = function() use ($name) {
    echo "Hello $name";
}
$greeting();
```
## Arrow Function

```php
$greeting = fn() => "Hello World!";
$greeting();
```