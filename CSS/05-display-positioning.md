# 05 — Display and positioning

## Display values

- `block`: starts a new line and typically takes available inline space.
- `inline`: flows with text; width/height behavior is limited.
- `inline-block`: inline flow with box dimensions.
- `none`: removes the element from layout.
- `flex`: creates a flex formatting context.
- `grid`: creates a grid formatting context.

## Position

```css
.static { position: static; }
.relative { position: relative; }
.absolute { position: absolute; top: 1rem; right: 1rem; }
.fixed { position: fixed; bottom: 1rem; right: 1rem; }
.sticky { position: sticky; top: 0; }
```

- `static`: normal flow.
- `relative`: stays in flow; offsets change visual position.
- `absolute`: removed from normal flow and positioned against its containing block.
- `fixed`: commonly positioned relative to viewport.
- `sticky`: acts relatively until a scroll threshold.

`z-index` controls stacking within stacking contexts; a child cannot escape its ancestor's stacking context just by using a large value.

## Practice
Create a card with a badge in its top-right corner using a relative parent and absolute badge.
