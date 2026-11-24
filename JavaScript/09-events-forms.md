# 09 — Events and forms

Events represent browser activity such as clicks, key presses, input changes, and form submissions.

## addEventListener

```javascript
const button = document.querySelector("#save");
button.addEventListener("click", () => {
  console.log("Button clicked");
});
```

Prefer `addEventListener` over inline HTML event attributes.

## Event object

```javascript
button.addEventListener("click", event => {
  console.log(event.type);
  console.log(event.currentTarget);
});
```

- `target`: originating event target.
- `currentTarget`: element whose listener is running.
- `preventDefault()`: prevents the default action when applicable.
- `stopPropagation()`: stops further propagation.

## Form handling

```html
<form id="signup">
  <label for="email">Email</label>
  <input id="email" name="email" type="email" required>
  <button>Submit</button>
</form>
```

```javascript
const form = document.querySelector("#signup");
form.addEventListener("submit", event => {
  event.preventDefault();
  const data = new FormData(form);
  console.log(data.get("email"));
});
```

Client-side validation improves usability; server-side validation is still required.

## Event delegation
Attach one listener to a parent and inspect `event.target` to handle events from children, including dynamic elements.

## Practice
Create a task list where clicking a button adds a task and clicking a task marks it complete.
