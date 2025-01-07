# C# Notes

## Comments
```cs
// Single line comment
/*
 Multi-line
 comment
*/
```

## Print
```cs
Console.WriteLine("value");
```


## Data Types

### Strings/Chars
```cs
char character = 'A'; // Character
string text = "Hello World"; // String
```

### Numbers
```cs
int integer = 42; // Integer
long longInteger = 123456789L; // Long integer
double floatingPoint = 3.14; // Floating point number
float singlePrecision = 3.14F; // Single precision floating point number
```

### Booleans
```cs
bool isTrue = true;
bool isFalse = false;
```

## Arrays
```cs
string[] arrayName = {element1, element2, element3};
arrayName[0];
arrayName[0] = newValue;
```

## Operators
### Arithmetic Operators
```cs
+ // Addition
- // Subtraction
* // Multiplication
/ // Division
% // Modulus
```

### Assignment Operators
```cs
= // Assignment
+= // Addition assignment
-= // Subtraction assignment
*= // Multiplication assignment
/= // Division assignment
%= // Modulus assignment
```

### Increment/Decrement Operators
```cs
a++ // Increment
++a // Increment
a-- // Decrement
--a // Decrement
```

### Comparison Operators
```cs
== // Equal
!= // Not equal
> // Greater than
< // Less than
>= // Greater than or equal
<= // Less than or equal
```

### Logical Operators
```cs
&& // AND
|| // OR
!  // NOT
```

## Conditionals
### if/else if/else
```cs
if (condition1)
{
  // ...
}
else if (condition2)
{
  // ...
}
else
{
  // ...
}
```

### switch
```cs
switch(expression)
{
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
```cs
for (int i = 0; i < 5; i++)
{
  Console.WriteLine(i);
}
```

### while
```cs
int i = 0;
while (i < 5)
{
  Console.WriteLine(i);
  i++;
}
```

### do while
```cs
int i = 0;
do
{
  Console.WriteLine(i);
  i++;
}
while (i < 5);
```

### foreach
```cs
string[] arrayName = {element1, element2, element3};
foreach (string i in arrayName)
{
  Console.WriteLine(i);
}
```

### break
```cs
for (int i = 0; i < 5; i++)
{
  if (i == 4)
  {
    break;
  }
  Console.WriteLine(i);
}
```

### continue
```cs
for (int i = 0; i < 5; i++)
{
  if (i == 4)
  {
    continue;
  }
  Console.WriteLine(i);
}
```

## Methods

### Method
```cs
static void MethodName()
{
  // ...
}

MethodName();
```

### Parameters
```cs
static void MethodName(string text)
{
  // ...
}

MethodName("value");
```

### return
```cs
static string MethodName()
{
  // ...
  return "value";
}

MethodName();
```

## Classes

### class
```cs
public class Person
{
}
```

### constructor
```cs
public class Person
{
  public string Name { get; set; }
  public int Age { get; set; }

  public Person(string name, int age)
  {
    Name = name;
    Age = age;
  }
}
```

### method
```cs
public class Person
{
  public string Name { get; set; }
  public int Age { get; set; }

  public Person(string name, int age)
  {
    Name = name;
    Age = age;
  }

  public void Introduce()
  {
    Console.WriteLine($"Hi, my name is {Name} and I am {Age} years old.");
  }
}
```

### instance
```cs
class Program
{
  static void Main(string[] args)
  {
    Person person = new Person("John", 30);
    person.Introduce();
  }
}
```
