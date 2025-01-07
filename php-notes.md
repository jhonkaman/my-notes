# PHP Notes

## Comments
```php
// Single line comment

# Single line comment

/*
 Multi-line
 comment
*/
```

## Echo/Print
```php
echo 'value';
echo 'value1', 'value2';

echo('value');
echo('value1', 'value2');
```
```php
print 'value';
print('value');
```

## Data Types

### Strings
```php
$text = 'Hello World';
$text = "Hello World";
```

### Numbers
```php
$integer = 42; // Integer
$floatingPoint = 1.234; // Float
```

### Booleans
```php
$boolean = true;
$boolean = false;
```

### Arrays
```php
$arrayName = array(element1, element2, element3);
$arrayName[0];
$arrayName[0] = newValue;
```
```php
$arrayName = [element1, element2, element3];
$arrayName[0];
$arrayName[0] = newValue;
```

### Associative Arrays
```php
$arrayName = [
  'key1' => 'value1',
  'key2' => 'value2',
  'key3' => 'value3'
];

$arrayName['key1'];
$arrayName['key1'] = 'new value';
```

## Operators
### Concatenate
```php
.  // Concatenation
.= // Concatenation assignment
```

### Interpolate
```php
"Hello $name"
```
### Arithmetic Operators
```php
+  // Addition
-  // Subtraction
*  // Multiplication
/  // Division
%  // Modulus
** // Exponent
```

### Assignment Operators
```php
=   // Assignment
+=  // Addition assignment
-=  // Subtraction assignment
*=  // Multiplication assignment
/=  // Division assignment
%=  // Modulus assignment
**= // Exponent assignment
```

### Increment/Decrement Operators
```php
$a++ // Post-increment
++$a // Pre-increment
$a-- // Post-decrement
--$a // Pre-decrement
```

### Comparison Operators
```php
==  // Equal
=== // Identical
!=  // Not equal
<>  // Not equal
!== // Not identical
>   // Greater than
<   // Less than
>=  // Greater than or equal
<=  // Less than or equal
<=> // Spaceship
```

### Logical Operators
```php
&&  // AND
||  // OR
!   // NOT

and // AND
or  // OR
```

## Conditionals
### if/else if/else
```php
if (condition1) {
  // ...
} elseif (condition2) {
  // ...
} else {
  // ...
}
```

### ternary
```php
$result = $condition ? $value_if_true : $value_if_false;
```

### switch
```php
switch(expression) {
  case x:
    // ...
    break;
  case y:
    // ...
    break;
  default:
    // ...
    break;
}
```

## Loops
### for
```php
for ($i = 0; $i < 5; $i++) {
  echo $i;
}
```

### while
```php
$i = 0;
while ($i < 5) {
  echo $i;
  $i++;
}
```
```php
$i = 0;
while ($i < 5):
  echo $i;
  $i++;
endwhile;
```

### do while
```php
$i = 0;
do {
  echo $i;
  $i++;
} while ($i < 5);
```

### foreach
```php
$arrayName = [$element1, $element2, $element3];
foreach ($arrayName as $item) {
  echo $item;
}
```
```php
$arrayName = [$element1, $element2, $element3];
foreach ($arrayName as $item):
  echo $item;
endforeach;
```

```php
$arrayName = [
  'key1' => 'value1',
  'key2' => 'value2',
  'key3' => 'value3'
];
foreach ($arrayName as $a => $b) {
  echo $a, $b;
}
```

### break
```php
for (int $i = 0; $i < 5; $i++) {
  if ($i == 3) {
    break;
  }
  echo $i;
}
```

### continue
```php
for (int $i = 0; $i < 5; $i++) {
  if ($i == 3) {
    continue;
  }
  echo $i;
}
```

## Functions
### Function Declaration
```php
function functionName() {
  // ...
}

functionName();
```

### return
```php
function functionName() {
  // ...
  return value;
}

functionName();
```

### Default Parameters
```php
function functionName($a, $b = 1) {
  // ...
}

functionName($x);
```

## Rest
```php
function functionName(a, b, ...rest) {
  // ...
}
```

## Spread
```php
function functionName(a, b, c) {
  // ...
}

functionName(...arrayName);
```

##

### class
```php
class MyClass {
  // Class body goes here
}
```

### constructor
```php
class MyClass {
  public $name;

  public function __construct($name) {
    $this->name = $name;
  }
}
```

### method
```php
class MyClass {
  public function sayHello() {
    echo "Hello, World!";
  }
}
```

### instance
```php
$myObject = new MyClass("John");
echo $myObject->name; // Access property
$myObject->greet();   // Call method
```
