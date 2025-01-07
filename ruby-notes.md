# Ruby Notes

## Comments

```ruby
# Comment
```

```ruby
# Comment
```

## Print
```ruby
print 'value'
```
```ruby
puts 'value'
```

## Data Types

### Strings
```ruby
text = 'Hello World'
text = "Hello World"
```

### Numbers
```ruby
integer = 42 # Integer
floating_point = 3.14 # Float
```

### Booleans
```ruby
boolean = true
boolean = false
```



### Arrays

```ruby
array_name = [element1, element2, element3]
array_name[0] # Access the first element
array_name[-1] # Access the last element
```



<!-- ## Sets

Ruby has a built-in `Set` class in the `set` library.

```ruby
require 'set'

set_name = Set.new([element1, element2, element3])
```

**Note**: Membership can be checked with `set_name.include?(element1)`. -->



### Hashes

```ruby
hash_name = {
  "key1" => "value1",
  "key2" => "value2",
  "key3" => "value3"
}

hash_name["key1"]
```


## Operators
### Arithmetic Operators

```ruby
+  # Add
-  # Subtract
*  # Multiply
/  # Divide
%  # Remainder
** # Exponent
```



### Assignment Operators

```ruby
+=  # Addition assignment
-=  # Subtraction assignment
*=  # Multiplication assignment
/=  # Division assignment
%=  # Modulo assignment
**= # Exponent assignment
```



### Comparison Operators

```ruby
== # Equal
!= # Not equal
>  # Greater than
<  # Less than
>= # Greater than or equal
<= # Less than or equal
```



### Logical Operators

```ruby
&& # AND
|| # OR
!  # NOT

and # AND
or  # OR
not # NOT
```


## Conditionals
### if/elsif/else

```ruby
if condition1
  # ...
elsif condition2
  # ...
else
  # ...
end
```


## Loops
### for

```ruby
# Generic version of a for loop
for variable in sequence
  # ...
end

list_name = [element1, element2, element3]
for variable in list_name
  # ...
end

# Using range
for variable in (start..end)
  # ...
end
```

**Note**: While Ruby supports `for`, `each` is more idiomatic.



### while

```ruby
counter = 0
while counter < 5
  # ...
  counter += 1
end
```



## Methods

### Method
```ruby
def function_name()
  # Code for the function
end

function_name()
```

### return
```ruby
def function_name()
  # Code for the function
  return value
end

function_name()
```

## Classes

### class
```ruby
class Person
end
```

### initialize
```ruby
class Person
  def initialize(name, age)
    @name = name
    @age = age
  end
end
```

### method
```ruby
class Person
  def initialize(name, age)
    @name = name
    @age = age
  end

  def introduce
    "Hi, I'm #{@name}, and I'm #{@age} years old."
  end
end
```

### instance
```ruby
person = Person.new("Alice", 30)
puts person.introduce
# Output: Hi, I'm Alice, and I'm 30 years old.
```

###
```ruby

```
