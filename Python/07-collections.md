# 07 — Lists, tuples, sets, and dictionaries

## List

Ordered, mutable collection; duplicates are allowed.

```python
fruits = ["apple", "mango"]
fruits.append("banana")
fruits[0] = "orange"
print(fruits)
```

Methods: `append`, `extend`, `insert`, `remove`, `pop`, `sort`, `reverse`, `copy`.

## Tuple

Ordered, immutable collection.

```python
point = (10, 20)
x, y = point
```

A one-item tuple needs a comma: `(5,)`.

## Set

Collection of unique elements; it has no positional indexing.

```python
numbers = {1, 2, 2, 3}
print(numbers)  # {1, 2, 3}
```

Operations: union `|`, intersection `&`, difference `-`, symmetric difference `^`.

## Dictionary

Stores key-value pairs. Keys must be hashable.

```python
student = {"name": "Uday", "marks": 90}
print(student["name"])
student["grade"] = "A"
print(student.get("course", "Not set"))
```

Methods: `keys()`, `values()`, `items()`, `get()`, `update()`, `pop()`.

## Comparison

| Type | Ordered? | Mutable? | Duplicates? |
|---|---|---|---|
| List | Yes | Yes | Yes |
| Tuple | Yes | No | Yes |
| Set | No positional order | Yes | No |
| Dictionary | Insertion order | Yes | Keys unique |

## Practice
Create a student dictionary, a list of marks, and a set of unique subjects.
