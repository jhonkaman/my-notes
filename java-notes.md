# Java

## Comments
```java
// Single line comment
/*
 Multi-line
 comment
*/
```

## Print
```java
System.out.println("value");
```

## Data Types

### Strings/Chars
```java
char character = 'A';
String text = "Hello World";
```

### Numbers
```java
int integer = 42; // Integer
long longInteger = 123456789L; // Long integer
double floatingPoint = 3.14; // Floating point number
float singlePrecision = 3.14F; // Single precision floating point number
```

### Booleans
```java
boolean isTrue = true;
boolean isFalse = false;
```

## Arrays
```java
String[] arrayName = { "element1", "element2", "element3" };
arrayName[0];
arrayName[0] = "newValue";
```

## Operators

### Arithmetic Operators
```java
+ // Addition
- // Subtraction
* // Multiplication
/ // Division
% // Modulus
```

### Assignment Operators
```java
=  // Assignment
+= // Addition assignment
-= // Subtraction assignment
*= // Multiplication assignment
/= // Division assignment
%= // Modulus assignment
```

### Increment/Decrement Operators
```java
a++; // Increment
++a; // Increment
a--; // Decrement
--a; // Decrement
```

### Comparison Operators
```java
== // Equal
!= // Not equal
>  // Greater than
<  // Less than
>= // Greater than or equal
<= // Less than or equal
```

### Logical Operators
```java
&& // AND
|| // OR
!  // NOT
```

## Conditionals

### if/else if/else
```java
if (condition1) {
  // ...
} else if (condition2) {
  // ...
} else {
  // ...
}
```

### switch
```java
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
```java
for (int i = 0; i < 5; i++) {
  System.out.println(i);
}
```

### while
```java
int i = 0;
while (i < 5) {
  System.out.println(i);
  i++;
}
```

### do while
```java
int i = 0;
do {
  System.out.println(i);
  i++;
} while (i < 5);
```

### foreach
```java
String[] arrayName = { "element1", "element2", "element3" };
for (String element : arrayName) {
  System.out.println(element);
}
```

### break
```java
for (int i = 0; i < 5; i++) {
  if (i == 4) {
    break;
  }
  System.out.println(i);
}
```

### continue
```java
for (int i = 0; i < 5; i++) {
  if (i == 4) {
    continue;
  }
  System.out.println(i);
}
```

## Methods

### Method
```java
static void methodName() {
  // ...
}

methodName();
```

### Parameters
```java
static void methodName(String text) {
  // ...
}

methodName("value");
```

### return
```java
static String methodName() {
  // ...
  return "value";
}

methodName();
```

## Classes

### class
```java
public class MyClass {
  // Class body
}
```

### constructor
```java
public class MyClass {
  String name;
  int age;

  // Constructor
  public MyClass(String name, int age) {
    this.name = name; // Assigning parameter to the field
    this.age = age;
  }
}
```

### method
```java
public class MyClass {
  String name;
  int age;

  public MyClass(String name, int age) {
    this.name = name;
    this.age = age;
  }

  // Method to display information
  public void displayInfo() {
    System.out.println("Name: " + name + ", Age: " + age);
  }
}
```

### instance
```java
public class Main {
  public static void main(String[] args) {
    // Create an object of MyClass
    MyClass person = new MyClass("Alice", 25);

    // Use methods of the class
    person.displayInfo();

    // Update the age
    person.setAge(30);
    System.out.println("Updated Age: " + person.getAge());
  }
}
```

###
```java

```
