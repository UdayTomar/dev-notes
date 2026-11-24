# 03 — Links and images

## Links

```html
<a href="https://developer.mozilla.org/">MDN Web Docs</a>
<a href="about.html">About page</a>
<a href="#contact">Jump to contact</a>
<a href="mailto:hello@example.com">Send email</a>
<a href="tel:+911234567890">Call us</a>
```

For a new tab, use `target="_blank"` and `rel="noopener"`. Write descriptive link text.

## Images

```html
<img src="images/workspace.jpg"
     alt="A desk with a laptop and notebook"
     width="800" height="500">
```

- `src`: image path or URL.
- `alt`: text alternative.
- `width` and `height`: help reserve layout space.

Use `alt=""` for decorative images. Do not put important text only inside an image.

## Figure and caption

```html
<figure>
  <img src="prototype.jpg" alt="Dashboard prototype on a phone">
  <figcaption>Early dashboard prototype.</figcaption>
</figure>
```

## Path types

- `images/photo.jpg`: relative path.
- `../images/photo.jpg`: parent directory.
- `/assets/logo.svg`: root-relative path.
- `https://example.com/photo.jpg`: absolute URL.

## Responsive images

```html
<img src="small.jpg"
     srcset="small.jpg 480w, large.jpg 1200w"
     sizes="(max-width: 600px) 100vw, 600px"
     alt="Product on a clean background">
```

## Practice
Create a profile page with external and internal links, an email link, and an accessible image.
