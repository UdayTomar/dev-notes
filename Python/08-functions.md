# 08 — Functions

A function is a reusable block of code.

```python
def greet(name):
    return f"Hello, {name}!"

message = greet("Uday")
print(message)
```

Output: `Hello, Uday!`

## Parameters and arguments

```python
def introduce(name, course="BCA"):
    print(name, course)

introduce("Uday")
introduce("Uday", "AIML")
```

A parameter appears in the definition; an argument is passed when calling the function.

## Keyword and positional arguments

```python
def rectangle_area(length, width):
    return length * width

print(rectangle_area(5, 3))
print(rectangle_area(width=3, length=5))
```

## Variable-length arguments

```python
def total(*numbers):
    return sum(numbers)

def profile(**details):
    return details
```

`*args` collects extra positional arguments; `**kwargs` collects extra keyword arguments.

## Scope

Local names belong to a function. Prefer passing values and returning results over changing global state.

## Lambda

```python
square = lambda number: number ** 2
print(square(4))  # 16
```

Use `def` for functions needing clear names or multiple statements.

## Practice
Write functions for factorial, prime checking, maximum of two numbers, and temperature conversion.
