# Table of Contents

Lightpack CSS framework support auto-generation of `table-of-contents` with a simple **JavaScript** utility function.

**Usage**

Add a container with the toc class wherever you want your Table of Contents to appear:

```html
<nav class="toc"></nav>
```

```javascript
Lightpack.generateToc('.toc', {
  levels: [2, 3],         // Include <h2> and <h3> headings
  scrollOffset: 64,       // Offset for fixed headers (in pixels)
  activeClass: 'toc-active' // Class for the currently active section link
});
```

---