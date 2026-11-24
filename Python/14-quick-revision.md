# 14 — Python quick revision

## Fundamentals
- `print()` displays output.
- `input()` reads a line and returns a string.
- `type()` inspects an object's type.
- `int()`, `float()`, `str()` convert values.
- Indentation defines blocks.

## Control flow
- `if / elif / else`: branching.
- `for`: iterate over an iterable.
- `while`: repeat while a condition is true.
- `break`: exit loop.
- `continue`: skip iteration.
- `return`: return a value from a function.

## Collections

| Type | Key property |
|---|---|
| List | Ordered, mutable |
| Tuple | Ordered, immutable |
| Set | Unique elements |
| Dictionary | Key-value mapping |

## File handling
`open(path, mode)`, `read()`, `readline()`, `readlines()`, `write()`, `close()`. Prefer `with open(...) as file:`.

## Common mistakes
- Forgetting `input()` returns a string.
- Using `=` instead of `==` in a comparison.
- Incorrect indentation.
- Not updating a `while` loop condition.
- Using `w` when you meant `a`.
- Assuming `write()` adds a newline.
- Catching every exception without understanding it.

## Quick questions
1. List vs tuple?
2. `==` vs `is`?
3. What does `range(1, 5)` produce?
4. Purpose of `return`?
5. Why use `with` for files?
6. `w` vs `a`?
7. What is an exception?
8. What are class and object?
