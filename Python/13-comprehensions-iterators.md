# 13 — Comprehensions and iterators

## List comprehension

```python
squares = [number ** 2 for number in range(1, 6)]
print(squares)
```

Output: `[1, 4, 9, 16, 25]`

With a condition:

```python
evens = [number for number in range(10) if number % 2 == 0]
```

## Dictionary and set comprehensions

```python
square_map = {number: number ** 2 for number in range(1, 4)}
unique_lengths = {len(word) for word in ["cat", "dog", "tiger"]}
```

## Iterables and iterators

An iterable can provide an iterator. An iterator produces values one at a time.

```python
numbers = [10, 20, 30]
iterator = iter(numbers)
print(next(iterator))
print(next(iterator))
```

Calling `next()` after exhaustion raises `StopIteration`.

## Generators

```python
def count_up_to(limit):
    number = 1
    while number <= limit:
        yield number
        number += 1

for value in count_up_to(3):
    print(value)
```

Generators produce values lazily and can reduce memory use for large sequences.

## Practice
Create a list of squares, a dictionary of word lengths, and a generator for even numbers.
