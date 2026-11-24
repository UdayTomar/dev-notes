# 10 — Asynchronous JavaScript

Asynchronous code lets an operation start while the program can continue without waiting synchronously for it to finish.

## setTimeout

```javascript
setTimeout(() => {
  console.log("Runs later");
}, 1000);
```

## Promise

A Promise represents the eventual completion or failure of an asynchronous operation.

```javascript
const task = new Promise((resolve, reject) => {
  const success = true;
  if (success) resolve("Done");
  else reject(new Error("Something failed"));
});

task
  .then(result => console.log(result))
  .catch(error => console.error(error))
  .finally(() => console.log("Finished"));
```

## async and await

```javascript
async function loadData() {
  try {
    const response = await fetch("https://jsonplaceholder.typicode.com/todos/1");
    if (!response.ok) throw new Error(`HTTP error: ${response.status}`);
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Request failed:", error);
  }
}
loadData();
```

`fetch()` does not automatically reject for HTTP statuses such as 404. Check `response.ok`.

## Promise.all

`Promise.all()` fulfills when all inputs fulfill and rejects when one rejects. Use `Promise.allSettled()` when every outcome is needed.

## Practice
Fetch sample JSON, check response status, parse JSON, and display a field.
