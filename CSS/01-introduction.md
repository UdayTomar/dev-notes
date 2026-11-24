# 01 — CSS introduction

CSS describes how HTML elements should look and be laid out.

## Ways to add CSS

External stylesheet (recommended):

```html
<link rel="stylesheet" href="styles.css">
```

Internal stylesheet:

```html
<style>
  h1 { color: navy; }
</style>
```

Inline style:

```html
<p style="color: tomato;">Hello</p>
```

## Rule syntax

```css
selector {
  property: value;
}
```

A selector chooses elements; a declaration is a property/value pair.

## Cascade

When declarations conflict, the browser considers origin, importance, cascade layers, specificity, and source order. Avoid using `!important` as a routine fix.

## Comment

```css
/* This is a CSS comment. */
```

## Practice
Link an external stylesheet and style the body, heading, paragraph, and button.
