# 08 — DOM basics

The DOM is the browser's object model of an HTML document. JavaScript can select nodes and update content, attributes, styles, and structure.

## Select elements

```javascript
const heading = document.querySelector("h1");
const cards = document.querySelectorAll(".card");
const byId = document.getElementById("main");
```

`querySelector` returns the first match or `null`; `querySelectorAll` returns a static NodeList.

## Update content

```javascript
heading.textContent = "Welcome!";
```

Use `textContent` for plain text. Avoid putting untrusted input into `innerHTML because it can create XSS vulnerabilities.

## Classes and attributes

```javascript
const panel = document.querySelector(".panel");
panel.classList.add("active");
panel.classList.toggle("hidden");
panel.setAttribute("aria-expanded", "true");
```

## Create an element

```javascript
const item = document.createElement("li");
item.textContent = "JavaScript";
document.querySelector("ul").append(item);
```

With a deferred external script, HTML has been parsed before the script runs. Otherwise, use `DOMContentLoaded` if your code needs the parsed document.

## Practice
Build a button that changes a heading and toggles a class on a card.
