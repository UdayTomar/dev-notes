# 13 — Modern JavaScript concepts

## Optional chaining

```javascript
const city = user.address?.city;
```

Returns `undefined` instead of throwing when an intermediate value is nullish.

## Nullish coalescing

```javascript
const label = inputValue ?? "Untitled";
```

Uses the fallback only for `null` or `undefined`, unlike `||`, which also falls back for `0` and empty strings.

## Map and Set

```javascript
const unique = new Set([1, 1, 2]);
const scores = new Map();
scores.set("Uday", 90);
```

`Set` stores unique values. `Map` stores key-value pairs and supports many key types.

## Classes

```javascript
class Person {
  constructor(name) {
    this.name = name;
  }
  greet() {
    return `Hello, ${this.name}`;
  }
}
const person = new Person("Uday");
console.log(person.greet());
```

JavaScript classes use prototype-based inheritance under the hood.

## this

The value of `this` depends on how a function is called. Arrow functions capture `this` lexically from the surrounding context.

## Practice
Build a product list using `filter`, `map`, optional chaining, and a `Set` to remove duplicate categories.
