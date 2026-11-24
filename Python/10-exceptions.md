# 10 — Exceptions

Exceptions are runtime errors or unusual conditions that interrupt normal flow unless handled.

## try and except

```python
try:
    number = int(input("Enter a number: "))
    print(10 / number)
except ValueError:
    print("Enter a valid integer.")
except ZeroDivisionError:
    print("Cannot divide by zero.")
```

## else and finally

```python
try:
    result = 10 / 2
except ZeroDivisionError:
    print("Division failed")
else:
    print("Result:", result)
finally:
    print("Cleanup")
```

- `except`: handles a matching exception.
- `else`: runs if no exception occurred in `try`.
- `finally`: runs during cleanup whether or not an exception occurred.

## Raise

```python
def set_age(age):
    if age < 0:
        raise ValueError("Age cannot be negative")
    return age
```

Catch specific exceptions rather than using a broad `except:` without a clear reason.

## Practice
Ask for two numbers and handle invalid input and division by zero.
