# 03 — Operators and type conversion

## Arithmetic
`+`, `-`, `*`, `/`, `%`, `**`, `++`, `--`.

The `+` operator can add numbers or concatenate strings:

```javascript
console.log(2 + 3);   // 5
console.log("2" + 3); // "23"
console.log(8 - "3"); // 5
```

## Comparison
`===`, `!==`, `>`, `<`, `>=`, `<=`.

## Logical
- `&&`: AND
- `||`: OR
- `!`: NOT
- `??`: nullish coalescing; fallback only for null or undefined

## Assignment

```javascript
let total = 10;
total += 5;
total *= 2;
```

## Conversion

```javascript
Number("42");          // 42
String(42);            // "42"
Boolean(1);            // true
parseInt("12px", 10);  // 12
```

Invalid numeric conversion can produce `NaN`. Check with `Number.isNaN(value)`.

Falsy values include `false`, `0`, `-0`, `0n`, `""`, `null`, `undefined`, and `NaN`. Empty arrays and objects are truthy.

## Practice
Convert a prompt value to a number, calculate its square, and handle invalid input.
