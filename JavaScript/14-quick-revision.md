# 14 — JavaScript quick revision

## Core reminders
- `const`: binding cannot be reassigned.
- `let`: block-scoped and reassignable.
- `===`: strict equality.
- `typeof`: returns a type description string.
- `Array.isArray(value)`: checks for an array.
- `map()`: transforms into a new array.
- `filter()`: selects matching items.
- `reduce()`: accumulates a result.
- `querySelector()`: selects the first matching DOM element.
- `addEventListener()`: registers an event listener.
- `JSON.stringify()`: converts a value to JSON text.
- `JSON.parse()`: parses JSON text.
- `async` functions return Promises.
- `await` pauses within an async function until a Promise settles.

## Common mistakes
- Using `=` instead of `===` in a comparison.
- Assuming `const` objects cannot be mutated.
- Assuming an empty array is falsy (it is truthy).
- Using `innerHTML` with untrusted input.
- Forgetting to check `response.ok` after `fetch`.
- Using `for...in` as the normal array-value loop.
- Forgetting `sort()` mutates and sorts strings by default.
- Accessing a DOM element before it exists.

## Quick questions
1. Difference between `let` and `const`?
2. Difference between `==` and `===`?
3. What is a closure?
4. Difference between `map` and `forEach`?
5. What is the DOM?
6. What does `preventDefault()` do?
7. What is a Promise?
8. Why check `response.ok` after `fetch()`?
9. Difference between `null` and `undefined`?
10. What is event delegation?
