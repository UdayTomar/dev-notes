# 01 — Getting started

Save a file as `hello.py` and run it:

```bash
python hello.py
```

Depending on your system, use `python3`.

## First program

```python
print("Hello, world!")
```

Output:

```text
Hello, world!
```

## Comments and indentation

```python
# A comment
if True:
    print("Indented block")
```

Python uses indentation to define blocks. Four spaces are conventional. Triple-quoted strings are commonly used for docstrings, not technically comment syntax.

## Input and output

```python
name = input("Enter your name: ")
print("Hello,", name)
age = int(input("Enter age: "))
```

`input()` returns a string. Convert it when numeric input is required.

## Practice
1. Print your name and course.
2. Ask for two numbers and print their sum.
3. Ask for a name and greet the user.
