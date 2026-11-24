# 05 — Functions and scope

## Function declaration

```javascript
function greet(name) {
  return `Hello, ${name}!`;
}
console.log(greet("Uday"));
```

## Function expression and arrow function

```javascript
const add = function (a, b) {
  return a + b;
};

const square = number => number * number;
```

Arrow functions have lexical `this` and are not interchangeable with ordinary functions in every context.

## Default and rest parameters

```javascript
function welcome(name = "Guest") {
  return `Welcome, ${name}`;
}

function sum(...numbers) {
  return numbers.reduce((total, number) => total + number, 0);
}
```

## Scope
- Global: available in the relevant global environment.
- Function: local to a function.
- Block: applies to `let` and `const` inside blocks.
- Lexical: nested functions can access surrounding scope.

## Closure

A closure is a function together with access to its surrounding lexical environment.

```javascript
function makeCounter() {
  let count = 0;
  return function () {
    count++;
    return count;
  };
}
const counter = makeCounter();
console.log(counter()); // 1
console.log(counter()); // 2
```

## Practice
Write functions for temperature conversion and finding the largest of three values.
