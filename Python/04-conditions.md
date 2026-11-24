# 04 — Conditions

## if, elif, else

```python
marks = 76

if marks >= 90:
    grade = "A"
elif marks >= 75:
    grade = "B"
elif marks >= 50:
    grade = "C"
else:
    grade = "Needs improvement"

print(grade)
```

Output: `B`

Python checks conditions from top to bottom and executes the first matching branch.

## Nested conditions

```python
age = 20
has_id = True

if age >= 18:
    if has_id:
        print("Entry allowed")
    else:
        print("ID required")
else:
    print("Underage")
```

## Truthy and falsy

Common falsy values include `False`, `None`, numeric zero, and empty strings/collections. Most other objects are truthy.

## Conditional expression

```python
status = "Adult" if age >= 18 else "Minor"
```

## Practice
1. Check positive, negative, or zero.
2. Find the largest of three numbers.
3. Check whether a year is a leap year.
