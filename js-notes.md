# JavaScript Notes

## Comments
```js
// Single line comment

/*
 Multi-line
 comment
*/
```

## Console
```js
console.log('value');
```

## Data Types

### Strings
```js
let text = 'Hello World';
let text = "Hello World";
```

### Numbers
```js
let integer = 42; // Integer (Number)
let floatingPoint = 1.234; // Float (Number)
```

### Booleans
```js
let boolean = true;
let boolean = false;
```

### Arrays
```js
let arrayName = [element1, element2, element3];
arrayName[0];
arrayName[0] = 'new value';
```

### Objects
```js
let objectName = {
  key1: value1,
  key2: value2,
  key3: value3
};

objectName.key1;
objectName["key1"];

objectName.key1 = 'new value';
objectName["key1"] = 'new value';
```

## Operators
### Arithmetic Operators
```js
+  // Addition
-  // Subtraction
*  // Multiplication
/  // Division
%  // Modulus
** // Exponent
```

### Assignment Operators
```js
=   // Assignment
+=  // Addition assignment
-=  // Subtraction assignment
*=  // Multiplication assignment
/=  // Division assignment
%=  // Modulus assignment
**= // Exponent assignment
```

### Increment/Decrement Operators
```js
a++ // Post-increment
++a // Pre-increment
a-- // Post-decrement
--a // Pre-decrement
```

### Comparison Operators
```js
==  // Equal
=== // Equal value and type
!=  // Not equal
!== // Not equal to type
>   // Greater than
<   // Less than
>=  // Greater than or equal
<=  // Less than or equal
```

### Logical Operators
```js
&& // AND
|| // OR
!  // NOT
```

## Conditionals
### if/else if/else
```js
if (condition1) {
  // ...
} else if (condition2) {
  // ...
} else {
  // ...
}
```

### ternary
```js
let result = condition ? valueIfTrue : valueIfFalse;
```

### switch
```js
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
```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

### while
```js
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

### do while
```js
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

### for of
```js
let arrayName = [element1, element2, element3];
for (item of arrayName) {
  console.log(item);
}
```

### for of
```js
let objectName = {
  key1: value1,
  key2: value2,
  key3: value3
};
for (item in objectName) {
  console.log(item);
}
```

### break
```js
for (let i = 0; i < 5; i++) {
  if (i == 3) {
    break;
  }
  console.log(i);
}
```

### continue
```js
for (let i = 0; i < 5; i++) {
  if (i == 3) {
    continue;
  }
  console.log(i);
}
```

## Functions

### Function Declaration
```js
function functionName() {
  // ...
}

functionName();
```

### return
```js
function functionName() {
  // ...
  return value;
}

functionName();
```

### Function Expression
```js
functionName = function() {
  // ...
}

functionName();
```

### Default Parameters
```js
function functionName(a, b = 1) {
  // ...
}

functionName(x);
```

### Rest
```js
function functionName(a, b, ...rest) {
  // ...
}
```

### Spread
```js
function functionName(a, b, c) {
  // ...
}

functionName(...arrayName);
```

## Arrow Functions
### No parameters
```js
functionName = () => {
  return 'value';
}
```

```js
functionName = () => 'value';
```

### 1 parameter
```js
functionName = (a) => {
  return a;
}
```

```js
functionName = (a) => a;
```

```js
functionName = a => a;
```

### 2+ parameters
```js
functionName = (a, b) => {
  return a + b;
}
```

```js
functionName = (a, b) => a + b;
```

## Classes
### class
```js
class Person {
}

```

### constructor
```js
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }
}

```

### method
```js
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
  }
}

```

### instance
```js
const person1 = new Person('Alice', 30);
person1.greet();
```

##
```js

```
