# 06 — Media and embedded content

## Audio

```html
<audio controls>
  <source src="audio/sample.mp3" type="audio/mpeg">
  Your browser does not support audio.
</audio>
```

## Video

```html
<video controls width="640" poster="preview.jpg">
  <source src="video/demo.mp4" type="video/mp4">
  Your browser does not support video.
</video>
```

Useful attributes include `controls`, `autoplay`, `muted`, `loop`, `poster`, and `playsinline`. Browsers may restrict autoplay.

## Iframe

```html
<iframe src="https://example.com"
        title="Example website"
        width="600" height="400"
        loading="lazy"></iframe>
```

Some sites block embedding. Give iframes a meaningful title. Use an appropriate `sandbox` policy for untrusted embedded content.

## Details and summary

```html
<details>
  <summary>Show the answer</summary>
  <p>HTML provides structure for web content.</p>
</details>
```

## Practice
Create a media page with audio, video, and an expandable FAQ.
