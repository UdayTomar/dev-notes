# 06 — Strings

Strings are immutable sequences of Unicode characters.

## Create strings

```python
single = 'Hello'
double = "Python"
multi = '''Multiple
lines'''
```

## Indexing and slicing

```python
word = "Python"
print(word[0])    # P
print(word[-1])   # n
print(word[1:4])  # yth
print(word[::-1]) # nohtyP
```

The slice stop index is excluded.

## Common methods

```python
text = "  Hello Python  "
print(text.strip())
print(text.lower())
print(text.upper())
print(text.replace("Python", "World"))
print("a,b,c".split(","))
print("-".join(["a", "b", "c"]))
print("Python".startswith("Py"))
```

Methods return new strings; they do not modify the original.

## f-strings

```python
name = "Uday"
score = 95
print(f"{name} scored {score}%")
```

Output: `Uday scored 95%`

## Escape sequences
- `\n`: newline
- `\t`: tab
- `\\`: backslash
- `\\"`: double quote

## Practice
Count vowels, reverse a string, and check whether a word is a palindrome.
