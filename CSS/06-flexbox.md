# 06 — Flexbox

Flexbox is a one-dimensional layout system with a main axis and cross axis.

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  gap: 1rem;
  flex-wrap: wrap;
}
```

| Property | Purpose |
|---|---|
| `flex-direction` | Main-axis direction |
| `justify-content` | Alignment on main axis |
| `align-items` | Alignment on cross axis |
| `align-content` | Spacing between flex lines |
| `flex-wrap` | Whether items wrap |
| `gap` | Space between items |
| `flex` | Grow, shrink, basis shorthand |
| `align-self` | Override cross-axis alignment |

With `row`, the main axis is horizontal in the usual writing mode. With `column`, it is vertical.

## Center content

```css
.hero {
  min-height: 60vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
```

## Practice
Create a responsive navigation bar with a logo and links. Let items wrap on narrow screens.
