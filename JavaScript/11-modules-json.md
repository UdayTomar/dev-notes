# 11 — Modules and JSON

## Export

```javascript
// math.js
export function add(a, b) {
  return a + b;
}
export const PI = 3.14159;
```

## Import

```javascript
// app.js
import { add, PI } from "./math.js";
console.log(add(2, 3));
```

Default export:

```javascript
// greeting.js
export default function greet(name) {
  return `Hello, ${name}`;
}
```

```javascript
import greet from "./greeting.js";
```

In HTML:

```html
<script type="module" src="app.js"></script>
```

Modules have their own scope and use strict mode. Browser modules are subject to origin and CORS rules; use a local development server rather than opening module files directly with `file://`.

## JSON

```javascript
const user = { name: "Uday", active: true };
const jsonText = JSON.stringify(user);
const parsed = JSON.parse(jsonText);
```

JSON supports objects, arrays, strings, numbers, booleans, and `null`. It does not support functions or `undefined`.

## Practice
Move helper functions into a separate module and import them into the main application.
