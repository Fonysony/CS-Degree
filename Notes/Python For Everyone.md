## Operator Precedence Rules

Highest precedence rule to lowest precedence rule:

    - Parentheses are always respected
    - Exponentiation (raise to a power)
    - Mutiplication
    - Division and Remainder
    - Addition and Subtraction
    - Left to Right

```py
x = 1 + 2 ** 3 / 4 * 5
print(x) # 11.0
```

## Type Matters

    - Python knows waht "type" everything is
    - Some operations are prohibited
    - You cannot "add 1" to a string
    - We can ask Python what type something is by using the type() function

```py
eee = 'hello' + 'there'
eee = eee + 1
TypeError: "Can not convert 'int' object to str implicitly"
type(eee) # <class 'str'>
type('hello') # <class 'str'>
type(1) # <class 'int'>
```

## Type Conversions

    - When you put an integer and floating point in an expression, the integer is implicitly converted to a float 
    - You can control this with the built-in functions int() and float() 

```py
print(float(99) + 100) # 199.0
i = 42
print(i)
print(type(i)) # <class 'int'>
f = float(i)
print(f) # 42.0
print(type(f)) # <class 'float'>
```

## Integer Divsion

    - Integer division produces a floating point result
    
This was different in Python 2.x

```py
print(10 / 2) # 5.0
print(9 / 2) # 4.5 old python gives 4
print(99 / 100) # 0.99 old python gives 0
print(10.0 / 2.0) # 5.0
print(99.0 / 100.0) # 0.99
```

