# 08 — Responsive design

Responsive design adapts content and layout to different viewport sizes and user preferences.

## Viewport meta

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

## Mobile-first media queries

```css
.grid { display: grid; grid-template-columns: 1fr; }

@media (min-width: 700px) {
  .grid { grid-template-columns: repeat(2, 1fr); }
}

@media (min-width: 1000px) {
  .grid { grid-template-columns: repeat(3, 1fr); }
}
```

## Fluid sizing

```css
.container {
  width: min(100% - 2rem, 1100px);
  margin-inline: auto;
}
h1 { font-size: clamp(2rem, 6vw, 4.5rem); }
img { max-width: 100%; height: auto; }
```

## Reduced motion

```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    scroll-behavior: auto !important;
    animation-duration: .01ms !important;
    transition-duration: .01ms !important;
  }
}
```

Respect reduced-motion preferences. Test contrast, zoom, keyboard access, and content reflow.

## Practice
Test a page at phone, tablet, and desktop widths. Fix layout issues without adding unnecessary breakpoints.
