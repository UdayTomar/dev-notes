# 07 — CSS Grid

Grid is a two-dimensional layout system for rows and columns.

## Basic grid

```css
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}
```

## Responsive grid

```css
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1rem;
}
```

## Placement

```css
.featured { grid-column: span 2; }
```

Useful properties: `grid-template-columns`, `grid-template-rows`, `grid-column`, `grid-row`, `gap`, `place-items`, and `grid-template-areas`.

## Named areas

```css
.layout {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
  grid-template-columns: 220px 1fr;
  gap: 1rem;
}
.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }
```

Flexbox is often best for one-dimensional alignment; Grid is useful for two-dimensional layouts. They work well together.

## Practice
Build a responsive project gallery.
