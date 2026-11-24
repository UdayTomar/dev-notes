# 02 — Text and semantic elements

## Headings and paragraphs

```html
<h1>My Portfolio</h1>
<h2>Projects</h2>
<h3>Website Redesign</h3>
<p>This project explores a clearer browsing experience.</p>
```

Use headings to create a logical document outline, not merely to make text large.

## Text meaning

```html
<strong>Important</strong>
<em>Emphasis</em>
<mark>Highlighted</mark>
<small>Small print</small>
H<sub>2</sub>O
2<sup>3</sup>
<del>Old text</del>
<ins>New text</ins>
```

`strong` indicates importance; `em` indicates stress emphasis.

## Semantic layout

```html
<header>
  <h1>Studio Journal</h1>
  <nav aria-label="Main navigation">
    <a href="/">Home</a>
    <a href="/work.html">Work</a>
  </nav>
</header>
<main>
  <article>
    <h2>Designing for clarity</h2>
    <p>Article content...</p>
  </article>
  <aside>Related links</aside>
</main>
<footer>Copyright information</footer>
```

| Element | Meaning |
|---|---|
| `header` | Introductory content |
| `nav` | Major navigation |
| `main` | Main page content |
| `section` | Thematic grouping |
| `article` | Self-contained composition |
| `aside` | Supplementary content |
| `footer` | Footer for a page or section |

Other useful elements: `div`, `span`, `blockquote`, `q`, `code`, `pre`, and `time`.

## Practice
Build a blog article using `header`, `main`, `article`, `section`, and `footer`.
