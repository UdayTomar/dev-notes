# 04 — The box model

Every element is represented by content, padding, border, and margin.

```css
.card {
  width: 300px;
  padding: 20px;
  border: 2px solid #333;
  margin: 16px;
}
```

With `content-box` (default), declared width applies to content only. Outer width is `300 + 40 + 4 = 344px`, excluding margins.

## Recommended sizing

```css
*, *::before, *::after {
  box-sizing: border-box;
}
```

With `border-box`, declared width includes content, padding, and border.

- Padding: space inside the border.
- Margin: space outside the border.
- Border: line around padding and content.

## Overflow

```css
.panel {
  max-height: 20rem;
  overflow: auto;
}
```

Common values: `visible`, `hidden`, `clip`, `scroll`, `auto`.

## Practice
Create three cards with consistent spacing. Compare `content-box` and `border-box`.
