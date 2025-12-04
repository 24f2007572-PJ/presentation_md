---
marp: true
title: Product Documentation Overview
author: 24f2007572@ds.study.iitm.ac.in
paginate: true
theme: custom-theme
---

<!--
Custom Theme Definition
You can store this at the top of the file or move it to a separate CSS file.
-->
<style>
section {
  font-family: "Segoe UI", sans-serif;
}

h1, h2, h3 {
  color: #005f9e;
}

img.full-bg {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

footer {
  color: #888;
  font-size: 0.8rem;
}

/* Custom highlight box */
.highlight-box {
  background: #e6f2ff;
  padding: 12px;
  border-left: 6px solid #005f9e;
  border-radius: 4px;
}
</style>

<!-- Theme Configuration -->
<style id="theme">
:root {
  --background-color: #ffffff;
  --text-color: #222;
  --heading-color: #005f9e;
  --link-color: #0066cc;
}
</style>

# Product Documentation  
### Using Marp for Maintainable Presentations  
**Author:** 24f2007572@ds.study.iitm.ac.in

---

## Why Marp?
- Write presentations in **Markdown**
- Store version-controlled documentation in Git repos
- Export to **PDF, PPTX, HTML**
- Custom themes and full CSS control  
- Friendly for technical writers and developers

---

## Custom Theme Features
<div class="highlight-box">

- Corporate-aligned color scheme  
- Typography overrides  
- Styled callouts and code blocks  
- Enhanced layout control through CSS  

</div>

---

## Algorithmic Complexity Example

We can embed LaTeX formulas using Marp’s math support:

### Time Complexity

For a binary search operation:

\[
T(n) = O(\log n)
\]

### More complex recurrence:

\[
T(n) = 2T\left(\frac{n}{2}\right) + n 
\Rightarrow T(n) = O(n \log n)
\]

---

## Background Image Slide

<!-- Set a background image (replace the URL/path to your own asset) -->
![bg](https://picsum.photos/1600/900)

# Visual Enhancements

The background image can be full-slide and still allow
normal text formatting using Marp directives.

---

## Code Example

```python
def fetch_data():
    """Fetches API data with caching."""
    if cache.exists():
        return cache.load()
    data = api.request("/endpoint")
    cache.save(data)
    return data
