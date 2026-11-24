# 11 — Modules and packages

A module is a Python file that can be imported. A package organizes modules.

## Import

```python
import math
print(math.sqrt(25))

from math import pi
print(pi)

import datetime as dt
```

Avoid wildcard imports in most application code because names become harder to trace.

## Standard library

```python
import random
import pathlib
import json
import statistics

print(random.randint(1, 6))
print(pathlib.Path(".").resolve())
```

## Main guard

```python
def main():
    print("Program starts here")

if __name__ == "__main__":
    main()
```

This lets a file be imported without automatically running its main program block.

## Install packages and virtual environments

```bash
python -m pip install package-name
python -m venv .venv
```

Use a virtual environment to isolate project dependencies.

## Practice
Create a module with arithmetic functions and import it into another Python file.
