# 12 — Object-oriented programming

OOP organizes code around objects that combine data and behavior.

## Class and object

```python
class Student:
    def __init__(self, name, marks):
        self.name = name
        self.marks = marks

    def introduce(self):
        return f"I am {self.name}"

student = Student("Uday", 90)
print(student.introduce())
```

- Class: blueprint for objects.
- Object/instance: a value created from a class.
- `__init__`: initializer called when an instance is created.
- `self`: conventional name for the instance parameter.

## Class and instance attributes

```python
class Counter:
    total = 0

    def __init__(self):
        Counter.total += 1
        self.value = 0
```

## Inheritance and overriding

```python
class Animal:
    def speak(self):
        return "Some sound"

class Dog(Animal):
    def speak(self):
        return "Woof"
```

## Key ideas
- Encapsulation: group data and related behavior; manage access through conventions and properties.
- Abstraction: expose a useful interface while hiding implementation details.
- Polymorphism: different object types respond to a common interface in their own way.
- Inheritance: derive a class from another class.

Python uses conventions such as a leading underscore for internal attributes; it does not enforce private instance attributes like some languages.

## Practice
Create a `BankAccount` class with deposit, withdraw, and balance methods. Validate amounts.
