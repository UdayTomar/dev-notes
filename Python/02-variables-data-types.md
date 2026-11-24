# 02 — Variables and data types

## Variables

```python
name = "Uday"
age = 20
height = 1.65
is_learning = True
```

Python is dynamically typed: you do not declare a variable's type in advance.

## Common built-in types

| Type | Example |
|---|---|
| `int` | `25` |
| `float` | `3.14` |
| `str` | `"Hello"` |
| `bool` | `True` |
| `list` | `[1, 2, 3]` |
| `tuple` | `(1, 2, 3)` |
| `set` | `{1, 2, 3}` |
| `dict` | `{"name": "Uday"}` |
| `NoneType` | `None` |

```python
value = 10
print(type(value))
```

Output: `<class 'int'>`

## Type conversion

```python
age = int("20")
price = float("19.5")
text = str(100)
```

Invalid conversions can raise `ValueError`.

## Naming rules
- Names may contain letters, digits, and underscores.
- Names cannot begin with a digit.
- Names are case-sensitive.
- Avoid reserved keywords.
- Prefer descriptive `snake_case` names.

## Practice
Store a product name, price, quantity, and availability flag. Print values and types.
