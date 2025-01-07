# Lua Notes

## Comments

```lua
-- Comment

--[[ a
multi-line
comment
--]]
```

## Print

```lua
print('value')
```

## Data Types

### Strings
```lua
text = 'Hello World'
text = "Hello World"
```

### Numbers
```lua
integer = 42 -- Integer
floatingPoint = 3.14 -- Float
```

### Booleans
```lua
boolean = true
boolean = false
```

### Tables

```lua
listName = {element1, element2, element3}
print(listName[1])
print(listName[#listName]) -- Access the last element
```



### Tables

```lua
dictionaryName = {
  key1 = "value1",
  key2 = "value2",
  key3 = "value3"
}

print(dictionaryName.key1)
```

## Operators

### Concatenate
```lua
..
```

### Arithmetic Operators

```lua
+  -- Add
-  -- Subtract
*  -- Multiply
/  -- Divide
%  -- Remainder
^  -- Exponent
```



### Assignment Operators
Lua does not support augmented assignment operators like `+=`.

<!-- ```lua
a = a + b
a = a - b
a = a * b
a = a / b
a = a % b
a = a ^ b
``` -->

### Increment/Decrement Operators
Lua does not have increment/decrement operators.

### Comparison Operators

```lua
== -- Equal
~= -- Not equal
>  -- Greater than
<  -- Less than
>= -- Greater than or equal
<= -- Less than or equal
```



### Logical Operators

```lua
and -- AND
or  -- OR
not -- NOT
```


## Conditionals
### if/elseif/else

```lua
if condition1 then
  -- ...
elseif condition2 then
  -- ...
else
  -- ...
end
```


## Loops
### for

```lua
for i = 1, 5, 1 do
  -- Code to execute
end

for i = 1, 5 do
  -- Code to execute
end
```
<!-- ```lua
-- Iterating over a sequence
listName = {element1, element2, element3}
for index, value in ipairs(listName) do
  -- Code to execute for each element
end
```

**Note**: `ipairs` is used for iterating over tables. -->



### while

```lua
local counter = 1
while counter <= 5 do
  -- ...
  counter = counter + 1
end
```



## Functions

### function
```lua
function function_name()
  -- ...
end

function_name()
```

### return
```lua
function function_name()
  -- ...
  return value
end

function_name()
```
