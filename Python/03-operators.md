# 03 — Operators

## Arithmetic

| Operator | Meaning | Example |
|---|---|---|
| `+` | Addition | `5 + 2` → `7` |
| `-` | Subtraction | `5 - 2` → `3` |
| `*` | Multiplication | `5 * 2` → `10` |
| `/` | Division | `5 / 2` → `2.5` |
| `//` | Floor division | `5 // 2` → `2` |
| `%` | Remainder | `5 % 2` → `1` |
| `**` | Power | `5 ** 2` → `25` |

## Comparison
`==`, `!=`, `>`, `<`, `>=`, `<=` return Boolean results.

## Logical
- `and`: both operands must be truthy.
- `or`: at least one operand is truthy.
- `not`: reverses truth value.

## Assignment

```python
count = 5
count += 1
count *= 2
```

## Membership and identity

```python
print("a" in "cat")       # True
print(10 not in [1, 2])   # True

a = [1, 2]
b = a
print(a is b)             # True: same object
print(a == b)             # True: equal values
```

`==` checks equality; `is` checks identity.

## Practice
Calculate the area and perimeter of a rectangle.
