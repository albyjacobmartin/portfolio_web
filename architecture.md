I’m building a single-page scrolling website with a 2-layer design:

1. **Fixed background:** `page.svg` — a 1920×1080 sky illustration fixed to the viewport and never moves while scrolling.
2. **Scrollable foreground:** transparent sections containing all website content/elements. These sections scroll over the fixed sky.

Core CSS:

```css
.sky-background {
  position: fixed;
  inset: 0;
  z-index: 0;
  background: url("./page.svg") center / cover no-repeat;
}

.content-layer {
  position: relative;
  z-index: 1;
  background: transparent;
}
```

Project:

```text
index.html
style.css
script.js
page.svg
```

Use vanilla HTML/CSS/JS for now. Keep the fixed-sky + transparent-scrolling-content architecture unchanged. I’ll provide the design/content requirements as we build the site.
