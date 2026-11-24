# 03 — Colors, units, and typography

## Color formats

```css
.title { color: tomato; }
.panel { background: #121820; }
.accent { color: rgb(30 180 160); }
.overlay { background: rgb(0 0 0 / 50%); }
```

Common formats: named colors, hex, `rgb()`, `hsl()`, and modern color functions.

## Units

| Unit | Meaning |
|---|---|
| `px` | CSS pixel |
| `%` | Relative to a containing context/property |
| `em` | Relative to element font size for many properties |
| `rem` | Relative to root element font size |
| `vw` | 1% of viewport width |
| `vh` | 1% of viewport height |
| `fr` | Fraction of available grid space |

## Typography

```css
body {
  font-family: system-ui, sans-serif;
  font-size: 1rem;
  line-height: 1.6;
}

h1 {
  font-size: clamp(2rem, 5vw, 4rem);
  line-height: 1.1;
}
```

Useful properties: `font-family`, `font-size`, `font-weight`, `line-height`, `letter-spacing`, `text-align`, `text-decoration`.

## Practice
Create a type scale for body text, labels, section headings, and a hero heading.
