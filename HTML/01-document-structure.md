# 01 — Document structure

## What is HTML?

HTML uses elements to describe page content. The browser parses HTML and builds the **DOM (Document Object Model)**.

## Basic document

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My First Page</title>
</head>
<body>
  <h1>Hello, world!</h1>
  <p>This is my first webpage.</p>
</body>
</html>
```

| Part | Purpose |
|---|---|
| `<!doctype html>` | Enables standards-mode HTML parsing |
| `<html>` | Root element |
| `<head>` | Metadata and linked resources |
| `<meta charset>` | Character encoding |
| viewport meta | Helps mobile browsers size the layout viewport |
| `<title>` | Browser tab title |
| `<body>` | Page content |

## Tags, elements, and attributes

A tag is markup such as `<p>`. An element is the complete structure. An attribute provides additional information.

```html
<a href="https://example.com" target="_blank" rel="noopener">Visit</a>
```

## Void elements

Void elements have no closing tag or child content: `img`, `br`, `hr`, `input`, `meta`, `link`.

```html
<img src="photo.jpg" alt="A mountain">
<br>
<hr>
```

## Nesting and comments

```html
<p>This is <strong>important</strong>.</p>
<!-- This is a comment -->
```

Elements must be nested correctly. Avoid duplicate `id` values.

## Practice
1. Create a page with a title, heading, and two paragraphs.
2. Add an image with useful alternative text.
3. Link to a second page in the same folder.
