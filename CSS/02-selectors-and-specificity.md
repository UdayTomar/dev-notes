# 02 — Selectors and specificity

## Common selectors

```css
* { box-sizing: border-box; } /* universal */
p { line-height: 1.6; }       /* type */
.note { color: teal; }        /* class */
#hero { padding: 2rem; }       /* ID */
h1, h2 { font-weight: 700; }  /* grouping */
```

## Attribute and combinators

```css
input[type="email"] { border-color: teal; }
.card p { margin: 0; }        /* descendant */
.card > h2 { margin: 0; }     /* child */
h2 + p { color: gray; }       /* adjacent sibling */
h2 ~ p { max-width: 60ch; }   /* general sibling */
```

## Pseudo-classes and pseudo-elements

```css
a:hover { text-decoration: underline; }
input:focus { outline: 2px solid royalblue; }
li:first-child { font-weight: bold; }
p::first-line { letter-spacing: .02em; }
```

## Specificity quick model

Specificity is commonly represented as ID, class/attribute/pseudo-class, and type/pseudo-element components:

- `p` → `0-0-1`
- `.card` → `0-1-0`
- `#hero` → `1-0-0`
- `#hero .card p` → `1-1-1`

This is a comparison model, not a decimal number. Cascade layers and importance also affect the full cascade.

## Inheritance

Properties such as `color` and `font-family` commonly inherit. `margin` and `border` generally do not.

## Practice
Style a card using a class, descendant selector, hover state, and focus state.
