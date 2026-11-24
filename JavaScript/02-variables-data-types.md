# 02 — Variables and data types

## Declarations

```javascript
const name = "Uday";
let score = 90;
score = 95;
```

- `const`: binding cannot be reassigned; object contents can still be mutable.
- `let`: block-scoped and reassignable.
- `var`: older function-scoped declaration; avoid in most modern code.

Prefer `const` by default and `let` when reassignment is needed.

## Primitive types
`string`, `number`, `bigint`, `boolean`, `undefined`, `symbol`, and `null`.

Objects, arrays, and functions are reference values. `typeof null` historically returns `"object"`.

## typeof

```javascript
console.log(typeof "hello"); // "string"
console.log(typeof 42);      // "number"
console.log(typeof true);    // "boolean"
console.log(typeof {});      // "object"
```

## Template literals

```javascript
const user = "Uday";
console.log(`Hello, ${user}!`);
```

## Equality
- `===`: strict equality without type coercion.
- `==`: loose equality with coercion in many cases.

Prefer `===` unless coercion is intentional.

## Practice
Declare a product name, price, and stock status. Print a sentence using a template literal.
