# 09 — Transitions and animations

## Transition

```css
.button {
  background: #222;
  color: white;
  transition: background-color 180ms ease, transform 180ms ease;
}
.button:hover {
  background: #444;
  transform: translateY(-2px);
}
```

A transition animates a property change between states.

## Keyframe animation

```css
@keyframes fade-in {
  from { opacity: 0; transform: translateY(8px); }
  to { opacity: 1; transform: translateY(0); }
}
.card { animation: fade-in 400ms ease both; }
```

Common properties: `transition-property`, `transition-duration`, `transition-timing-function`, `animation-name`, `animation-duration`, `animation-iteration-count`, `animation-fill-mode`.

Prefer animating `transform` and `opacity` for smoother effects. Avoid excessive motion and honor reduced-motion settings.

## Practice
Add a subtle button hover transition and a card entrance animation.
