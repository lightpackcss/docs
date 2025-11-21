# CSS Reset

Lightpack includes a modern CSS reset that ensures consistent styling across all browsers while providing sensible defaults that work with the framework's design system.

## Features

- **Modern Normalize** - Based on modern CSS reset practices
- **Design Token Integration** - Uses Lightpack variables for all defaults
- **Typography Defaults** - Sensible heading and text styles
- **Accessibility** - Respects `prefers-reduced-motion`
- **Theme-Aware** - Adapts to light/dark themes

---

## What's Included

### Box Sizing
```css
html {
  box-sizing: border-box;
}

*, *::before, *::after {
  box-sizing: inherit;
}
```

### Body Defaults
- Background: `var(--color-background)`
- Text color: `var(--color-text)`
- Font family: `var(--font-family)` (system UI stack)
- Font size: `var(--fs-base)` (16px)
- Line height: `var(--line-height-normal)` (1.5)
- Font smoothing enabled for better rendering

### Typography

**Headings:**
- All headings use `font-weight: 700` (bold)
- Tight line-height for better hierarchy
- Negative letter-spacing for improved readability
- Margin top: `var(--g-4)`, Margin bottom: `var(--g-2)`

**Heading Sizes:**
- `h1`: `--fs-4xl` (3rem / 48px)
- `h2`: `--fs-3xl` (2.25rem / 36px)
- `h3`: `--fs-2xl` (1.875rem / 30px)
- `h4`: `--fs-xl` (1.5rem / 24px)
- `h5`: `--fs-lg` (1.25rem / 20px)
- `h6`: `--fs-base` (1rem / 16px) with `font-weight: 600`

**Paragraphs:**
- Margin bottom: `var(--g-3)` (1rem)
- No top margin

### Links
- Color: `var(--color-primary)`
- Hover color: `var(--color-primary-dark)`
- Smooth color transitions (0.2s)
- Theme-aware (adapts in dark mode)

### Horizontal Rules
```css
hr {
  border: none;
  border-top: 1px solid var(--color-border);
  margin: var(--g-4) 0;
}
```

### Images
- `max-width: 100%` - Responsive by default
- `display: block` - Removes inline spacing issues
- `vertical-align: middle` - Better alignment

### Code & Pre
- Font family: `var(--font-family-mono)`
- Inline `code`: Background with padding and border-radius
- `pre` blocks: Padding, background, horizontal scroll
- Syntax: `<code>`, `<kbd>`, `<samp>`, `<pre>`

### Text Formatting
- `strong`, `b`: `font-weight: 700`
- `em`, `i`: Italic style
- `small`: `font-size: var(--fs-sm)`
- `mark`: Yellow highlight background

### Form Elements
All form elements inherit font properties from parent:
```css
input, button, textarea, select {
  font: inherit;
}
```

### Accessibility

**Reduced Motion Support:**
```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms;
    animation-iteration-count: 1;
    transition-duration: 0.01ms;
    scroll-behavior: auto;
  }
}
```

---

## Usage

The reset is automatically included when you import Lightpack CSS:

```html
<link rel="stylesheet" href="lightpack.min.css">
```

**Import Order** (in source):
1. Variables
2. **Reset** ← You are here
3. Utilities
4. Layout
5. Components

---

## Customization

All reset styles use CSS variables, so you can customize them by overriding variables:

```css
:root {
  --color-background: #f5f5f5;
  --color-text: #1a1a1a;
  --font-family: 'Inter', sans-serif;
  --fs-base: 18px;
}
```

---

## Dark Theme Support

The reset automatically adapts to dark theme when `.theme-dark` is applied to `<body>`:

- Background switches to dark
- Text color inverts
- Links adjust for better contrast
- All semantic colors update

---

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

---

**See `/src/css/_reset.css` for complete implementation.**
