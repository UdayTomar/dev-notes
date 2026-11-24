# 07 — Strings

Strings are immutable sequences of UTF-16 code units in JavaScript.

## Useful methods

```javascript
const text = "  Hello JavaScript  ";
console.log(text.trim());
console.log(text.toUpperCase());
console.log(text.toLowerCase());
console.log(text.includes("Java"));
console.log(text.replace("JavaScript", "World"));
console.log("a,b,c".split(","));
console.log(["a", "b", "c"].join("-"));
console.log(text.slice(2, 7));
```

## Template literals

```javascript
const item = "Notebook";
const price = 50;
console.log(`${item} costs ₹${price}.`);
```

## Conversion

```javascript
String(123);
(123).toString();
```

## Practice
Count words in a sentence and check whether a word is a palindrome. Consider extra spaces.
