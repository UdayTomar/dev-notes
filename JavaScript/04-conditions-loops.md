# 04 — Conditions and loops

## if / else

```javascript
const marks = 82;

if (marks >= 90) {
  console.log("A");
} else if (marks >= 75) {
  console.log("B");
} else {
  console.log("Keep practising");
}
```

## switch

```javascript
const day = 2;
switch (day) {
  case 1:
    console.log("Monday");
    break;
  case 2:
    console.log("Tuesday");
    break;
  default:
    console.log("Unknown day");
}
```

## for and while

```javascript
for (let i = 1; i <= 5; i++) {
  console.log(i);
}

let count = 1;
while (count <= 3) {
  console.log(count);
  count++;
}
```

## for...of and for...in

```javascript
const colors = ["red", "blue"];
for (const color of colors) console.log(color); // values

const user = { name: "Uday", level: "beginner" };
for (const key in user) console.log(key, user[key]); // keys
```

Use `for...of` for iterable values. `for...in` iterates enumerable property keys and is not generally preferred for array values.

`break` exits a loop; `continue` skips to the next iteration.

## Practice
Print even numbers from 1 to 50 and calculate their sum.
