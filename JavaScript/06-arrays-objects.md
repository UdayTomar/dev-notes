# 06 — Arrays and objects

## Arrays

```javascript
const skills = ["HTML", "CSS"];
skills.push("JavaScript");
console.log(skills[0]);
console.log(skills.length);
```

Common methods: `push`, `pop`, `shift`, `unshift`, `includes`, `indexOf`, `slice`, `splice`, `map`, `filter`, `find`, `reduce`, `forEach`.

## Transform, filter, and reduce

```javascript
const numbers = [1, 2, 3, 4];
const doubled = numbers.map(n => n * 2);
const evens = numbers.filter(n => n % 2 === 0);
const total = numbers.reduce((sum, n) => sum + n, 0);
```

`map`, `filter`, and `slice` return new arrays. `sort` and `splice` mutate the array.

## Objects

```javascript
const student = {
  name: "Uday",
  marks: 90,
  introduce() {
    return `I am ${this.name}`;
  }
};

console.log(student.name);
console.log(student["marks"]);
console.log(student.introduce());
```

## Destructuring and spread

```javascript
const { name, marks } = student;
const copy = { ...student, marks: 95 };
const [first, second] = ["HTML", "CSS"];
const moreSkills = [...skills, "Python"];
```

Spread creates a shallow copy; nested objects remain shared references unless separately copied.

## Practice
Filter products below a price and calculate the total using `reduce`.
