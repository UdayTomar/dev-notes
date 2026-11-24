# 05 — Loops

## for loop

```python
for number in range(1, 6):
    print(number)
```

Output: `1 2 3 4 5` (each on a new line).

`range(start, stop, step)` excludes the stop value.

## while loop

```python
count = 1
while count <= 3:
    print(count)
    count += 1
```

Output: `1 2 3`.

## break and continue

- `break`: exits the nearest loop.
- `continue`: skips to the next iteration.

```python
for number in range(1, 6):
    if number == 3:
        continue
    print(number)
```

Output: `1 2 4 5`.

## Loop else

A loop's `else` block runs if the loop finishes normally, not via `break`.

## Nested loops

```python
for row in range(2):
    for col in range(3):
        print(row, col)
```

## Practice
1. Print a multiplication table.
2. Sum numbers from 1 to n.
3. Count digits in an integer.
4. Check whether a number is prime.
