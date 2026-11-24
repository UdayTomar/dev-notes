# 09 — File handling

File handling reads and writes data stored in files.

## Open and read

```python
file = open("notes.txt", "r", encoding="utf-8")
content = file.read()
file.close()
```

Prefer a context manager, which closes the file automatically:

```python
with open("notes.txt", "r", encoding="utf-8") as file:
    content = file.read()

print(content)
```

## File modes

| Mode | Meaning |
|---|---|
| `r` | Read; file must exist |
| `w` | Write; creates or truncates |
| `a` | Append; creates if needed |
| `x` | Create; fails if file exists |
| `b` | Binary modifier |
| `t` | Text modifier (default) |
| `+` | Update/read and write modifier |

Examples: `rb`, `w+`, `a+`.

## Reading methods

- `read()`: reads content or up to a size.
- `readline()`: reads one line.
- `readlines()`: returns remaining lines as a list.
- Iterating over a file: reads line by line.

```python
with open("notes.txt", "r", encoding="utf-8") as file:
    for line in file:
        print(line, end="")
```

## Writing and appending

```python
with open("notes.txt", "w", encoding="utf-8") as file:
    file.write("First line\n")
    file.write("Second line\n")

with open("notes.txt", "a", encoding="utf-8") as file:
    file.write("Added later\n")
```

`write()` writes a string; it does not automatically add a newline. `print()` writes to standard output by default, not to a file unless its `file=` argument is used.

## Common errors
`FileNotFoundError`, `PermissionError`, `UnicodeDecodeError`, `IsADirectoryError`.

## Practice
Create a text file, write three lines, read and display them, then append a fourth line.
