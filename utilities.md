# Utility Classes

Lightpack provides a comprehensive set of utility classes for rapid UI development. These single-purpose classes let you build complex layouts and designs without writing custom CSS.

---

## Spacing

Lightpack uses a consistent spacing scale based on CSS variables (`--g-1` through `--g-9`).

**Scale Reference:**
- `0` = 0
- `1` = 0.25rem (4px)
- `2` = 0.5rem (8px)
- `3` = 1rem (16px)
- `4` = 1.5rem (24px)
- `5` = 2rem (32px)
- `6` = 3rem (48px)
- `7` = 4rem (64px)
- `8` = 6rem (96px)
- `9` = 8rem (128px)

### Margin

Control outer spacing around elements.

**All Sides:**
```html
<div class="m-0">No margin</div>
<div class="m-3">1rem margin on all sides</div>
<div class="m-5">2rem margin on all sides</div>
```

**Individual Sides:**
```html
<div class="mt-4">Margin top: 1.5rem</div>
<div class="mr-2">Margin right: 0.5rem</div>
<div class="mb-3">Margin bottom: 1rem</div>
<div class="ml-1">Margin left: 0.25rem</div>
```

**Horizontal & Vertical:**
```html
<!-- Horizontal (left + right) -->
<div class="mx-4">Margin left & right: 1.5rem</div>

<!-- Vertical (top + bottom) -->
<div class="my-3">Margin top & bottom: 1rem</div>

<!-- Center horizontally -->
<div class="mx-auto" style="width: 300px;">Centered block</div>
```

**Common Patterns:**
```html
<!-- Card spacing -->
<div class="card p-4 mb-3">
  <h3 class="mb-2">Card Title</h3>
  <p class="mb-0">Card content</p>
</div>

<!-- Section spacing -->
<section class="py-8 px-4">
  <h2 class="mb-4">Section Title</h2>
  <p>Content</p>
</section>
```

### Padding

Control inner spacing within elements.

**All Sides:**
```html
<div class="p-0">No padding</div>
<div class="p-3">1rem padding on all sides</div>
<div class="p-6">3rem padding on all sides</div>
```

**Individual Sides:**
```html
<div class="pt-4">Padding top: 1.5rem</div>
<div class="pr-2">Padding right: 0.5rem</div>
<div class="pb-3">Padding bottom: 1rem</div>
<div class="pl-1">Padding left: 0.25rem</div>
```

**Horizontal & Vertical:**
```html
<!-- Horizontal (left + right) -->
<button class="btn px-5">Wide button</button>

<!-- Vertical (top + bottom) -->
<div class="py-4">Tall container</div>
```

### Gap

Control spacing between flex/grid children.

```html
<!-- Flexbox with gap -->
<div class="flex gap-3">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>

<!-- Grid with gap -->
<div class="grid grid-cols-3 gap-4">
  <div>Cell 1</div>
  <div>Cell 2</div>
  <div>Cell 3</div>
</div>

<!-- Column gap only -->
<div class="flex flex-wrap gap-x-4">
  <div>Item</div>
  <div>Item</div>
</div>

<!-- Row gap only -->
<div class="flex flex-wrap gap-y-3">
  <div>Item</div>
  <div>Item</div>
</div>
```

---

## Layout & Display

### Display

Control how elements are displayed.

```html
<!-- Block (full width, stacks vertically) -->
<div class="d-block">Block element</div>

<!-- Inline (flows with text) -->
<span class="d-inline">Inline element</span>

<!-- Inline-block (flows with text but accepts width/height) -->
<span class="d-inline-block" style="width: 100px;">Inline-block</span>

<!-- Hide element -->
<div class="d-none">Hidden element</div>
```

**Use Cases:**
```html
<!-- Show/hide on mobile -->
<div class="d-none d-block-md">Visible on desktop only</div>
<div class="d-block d-none-md">Visible on mobile only</div>

<!-- Toggle visibility -->
<button onclick="document.querySelector('.content').classList.toggle('d-none')">
  Toggle
</button>
<div class="content">Toggleable content</div>
```

### Position

Control element positioning.

```html
<!-- Static (default) -->
<div class="static">Normal flow</div>

<!-- Relative (positioned relative to normal position) -->
<div class="relative">
  <span class="absolute" style="top: 0; right: 0;">Badge</span>
</div>

<!-- Absolute (positioned relative to nearest positioned ancestor) -->
<div class="relative">
  <div class="absolute" style="top: 10px; left: 10px;">Overlay</div>
</div>

<!-- Fixed (positioned relative to viewport) -->
<div class="fixed" style="top: 0; right: 0;">Fixed notification</div>

<!-- Sticky (toggles between relative and fixed) -->
<div class="sticky" style="top: 0;">Sticky header</div>
```

**Positioning Utilities:**
```html
<!-- Position from edges -->
<div class="absolute top-0 right-0">Top-right corner</div>
<div class="absolute bottom-0 left-0">Bottom-left corner</div>

<!-- Center absolutely -->
<div class="absolute" style="top: 50%; left: 50%; transform: translate(-50%, -50%);">
  Centered
</div>
```

### Overflow

Control content overflow behavior.

```html
<!-- Auto scrollbars (only when needed) -->
<div class="overflow-auto" style="height: 200px;">
  Long content...
</div>

<!-- Always show scrollbars -->
<div class="overflow-scroll" style="height: 200px;">
  Long content...
</div>

<!-- Hide overflow -->
<div class="overflow-hidden">
  Content is clipped
</div>

<!-- Horizontal only -->
<div class="overflow-x-auto">
  <table style="width: 2000px;">Wide table</table>
</div>

<!-- Vertical only -->
<div class="overflow-y-auto" style="height: 300px;">
  Long vertical content...
</div>
```

---

## Flexbox

Build flexible layouts with flexbox utilities.

### Basic Flex

```html
<!-- Enable flexbox -->
<div class="flex">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>

<!-- Inline flex -->
<div class="inline-flex">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

### Direction

```html
<!-- Row (default - horizontal) -->
<div class="flex flex-row">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>

<!-- Row reverse -->
<div class="flex flex-row-reverse">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>

<!-- Column (vertical) -->
<div class="flex flex-col">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>

<!-- Column reverse -->
<div class="flex flex-col-reverse">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>
```

### Wrapping

```html
<!-- Wrap items -->
<div class="flex flex-wrap gap-2">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
  <div>Item 5</div>
</div>

<!-- No wrap (default) -->
<div class="flex flex-nowrap">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

### Justify Content (Horizontal Alignment)

```html
<!-- Start (default) -->
<div class="flex justify-start">
  <div>Item</div>
</div>

<!-- Center -->
<div class="flex justify-center">
  <div>Centered</div>
</div>

<!-- End -->
<div class="flex justify-end">
  <div>Item</div>
</div>

<!-- Space between -->
<div class="flex justify-between">
  <div>Left</div>
  <div>Right</div>
</div>

<!-- Space around -->
<div class="flex justify-around">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>

<!-- Space evenly -->
<div class="flex justify-evenly">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>
```

### Align Items (Vertical Alignment)

```html
<!-- Start -->
<div class="flex items-start" style="height: 200px;">
  <div>Top aligned</div>
</div>

<!-- Center -->
<div class="flex items-center" style="height: 200px;">
  <div>Vertically centered</div>
</div>

<!-- End -->
<div class="flex items-end" style="height: 200px;">
  <div>Bottom aligned</div>
</div>

<!-- Stretch (default) -->
<div class="flex items-stretch" style="height: 200px;">
  <div>Stretched</div>
</div>

<!-- Baseline -->
<div class="flex items-baseline">
  <div class="fs-xl">Large</div>
  <div class="fs-sm">Small</div>
</div>
```

### Common Flexbox Patterns

```html
<!-- Center everything -->
<div class="flex items-center justify-center" style="height: 300px;">
  <div>Perfectly centered</div>
</div>

<!-- Navbar layout -->
<nav class="flex items-center justify-between p-4">
  <div class="navbar-brand">Logo</div>
  <div class="flex gap-4">
    <a href="#">Link 1</a>
    <a href="#">Link 2</a>
  </div>
</nav>

<!-- Card with footer at bottom -->
<div class="card flex flex-col" style="height: 300px;">
  <div class="flex-1 p-4">
    <h3>Title</h3>
    <p>Content</p>
  </div>
  <div class="p-4">
    <button class="btn">Action</button>
  </div>
</div>

<!-- Equal width columns -->
<div class="flex gap-4">
  <div class="flex-1">Column 1</div>
  <div class="flex-1">Column 2</div>
  <div class="flex-1">Column 3</div>
</div>

<!-- Sidebar layout -->
<div class="flex gap-4">
  <aside class="flex-none" style="width: 250px;">Sidebar</aside>
  <main class="flex-1">Main content</main>
</div>
```

---

## Grid

Build grid layouts with CSS Grid utilities.

### Basic Grid

```html
<!-- 3 column grid -->
<div class="grid grid-cols-3 gap-4">
  <div>Cell 1</div>
  <div>Cell 2</div>
  <div>Cell 3</div>
  <div>Cell 4</div>
  <div>Cell 5</div>
  <div>Cell 6</div>
</div>

<!-- 4 column grid -->
<div class="grid grid-cols-4 gap-3">
  <div>1</div>
  <div>2</div>
  <div>3</div>
  <div>4</div>
</div>
```

### Responsive Grid

```html
<!-- 1 column on mobile, 2 on tablet, 4 on desktop -->
<div class="grid grid-cols-1 grid-cols-md-2 grid-cols-lg-4 gap-4">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>
```

### Common Grid Patterns

```html
<!-- Product grid -->
<div class="grid grid-cols-2 grid-cols-md-3 grid-cols-lg-4 gap-5">
  <div class="card">Product 1</div>
  <div class="card">Product 2</div>
  <div class="card">Product 3</div>
  <div class="card">Product 4</div>
</div>

<!-- Dashboard grid -->
<div class="grid grid-cols-1 grid-cols-lg-3 gap-4">
  <div class="card">Stat 1</div>
  <div class="card">Stat 2</div>
  <div class="card">Stat 3</div>
</div>

<!-- Gallery grid -->
<div class="grid grid-cols-2 grid-cols-md-4 gap-2">
  <img src="image1.jpg" alt="">
  <img src="image2.jpg" alt="">
  <img src="image3.jpg" alt="">
  <img src="image4.jpg" alt="">
</div>
```

---

## Typography

### Font Sizes

```html
<p class="fs-xs">Extra small text (12px)</p>
<p class="fs-sm">Small text (14px)</p>
<p class="fs-base">Base text (16px)</p>
<p class="fs-md">Medium text (18px)</p>
<p class="fs-lg">Large text (20px)</p>
<p class="fs-xl">Extra large text (24px)</p>
<p class="fs-2xl">2X large text (30px)</p>
<p class="fs-3xl">3X large text (36px)</p>
<p class="fs-4xl">4X large text (48px)</p>
<p class="fs-5xl">5X large text (60px)</p>
```

**Use Cases:**
```html
<!-- Hero heading -->
<h1 class="fs-5xl fw-700">Welcome</h1>

<!-- Subheading -->
<h2 class="fs-2xl fw-600">Subtitle</h2>

<!-- Small print -->
<p class="fs-sm text-muted">Terms and conditions apply</p>
```

### Font Weights

```html
<p class="fw-100">Thin (100)</p>
<p class="fw-200">Extra Light (200)</p>
<p class="fw-300">Light (300)</p>
<p class="fw-400">Normal (400)</p>
<p class="fw-500">Medium (500)</p>
<p class="fw-600">Semi Bold (600)</p>
<p class="fw-700">Bold (700)</p>
<p class="fw-800">Extra Bold (800)</p>
<p class="fw-900">Black (900)</p>
```

### Text Alignment

```html
<p class="text-left">Left aligned text</p>
<p class="text-center">Center aligned text</p>
<p class="text-right">Right aligned text</p>
<p class="text-justify">Justified text that stretches to fill the line width</p>
```

**Responsive:**
```html
<!-- Left on mobile, center on desktop -->
<p class="text-left text-center-md">Responsive alignment</p>
```

### Text Transform & Decoration

```html
<p class="uppercase">UPPERCASE TEXT</p>
<p class="lowercase">lowercase text</p>
<p class="capitalize">Capitalized Text</p>

<p class="underline">Underlined text</p>
<p class="line-through">Strikethrough text</p>
```

### Text Utilities

```html
<!-- Truncate with ellipsis -->
<p class="truncate" style="width: 200px;">
  This is a very long text that will be truncated with an ellipsis
</p>

<!-- Prevent wrapping -->
<p class="whitespace-nowrap">This text will not wrap</p>

<!-- Break long words -->
<p class="break-words">
  Supercalifragilisticexpialidocious
</p>
```

---

## Colors

### Background Colors

**Semantic Colors:**
```html
<div class="bg-primary text-white p-3">Primary background</div>
<div class="bg-secondary text-white p-3">Secondary background</div>
<div class="bg-success text-white p-3">Success background</div>
<div class="bg-danger text-white p-3">Danger background</div>
<div class="bg-warning text-white p-3">Warning background</div>
<div class="bg-info text-white p-3">Info background</div>
```

**Shades:**
```html
<div class="bg-primary-lighter p-3">Lighter primary</div>
<div class="bg-primary-light p-3">Light primary</div>
<div class="bg-primary p-3">Primary</div>
<div class="bg-primary-dark text-white p-3">Dark primary</div>
```

**Natural Colors:**
```html
<div class="bg-red text-white p-3">Red</div>
<div class="bg-blue text-white p-3">Blue</div>
<div class="bg-green text-white p-3">Green</div>
<div class="bg-purple text-white p-3">Purple</div>
<div class="bg-indigo text-white p-3">Indigo</div>
<div class="bg-gray p-3">Gray</div>
```

**Surface Colors:**
```html
<div class="bg-surface p-3">Surface background</div>
<div class="bg-surface-dark p-3">Dark surface</div>
<div class="bg-muted p-3">Muted background</div>
```

### Text Colors

```html
<p class="text-primary">Primary text</p>
<p class="text-secondary">Secondary text</p>
<p class="text-success">Success text</p>
<p class="text-danger">Danger text</p>
<p class="text-warning">Warning text</p>
<p class="text-info">Info text</p>
<p class="text-muted">Muted text</p>
```

**Use Cases:**
```html
<!-- Status indicators -->
<span class="text-success">✓ Completed</span>
<span class="text-danger">✗ Failed</span>
<span class="text-warning">⚠ Warning</span>

<!-- Highlighted text -->
<p>This is <span class="text-primary fw-600">important</span> information</p>
```

---

## Borders

### Border Sides

```html
<!-- All sides -->
<div class="border p-3">Border on all sides</div>

<!-- Individual sides -->
<div class="border-top p-3">Top border only</div>
<div class="border-right p-3">Right border only</div>
<div class="border-bottom p-3">Bottom border only</div>
<div class="border-left p-3">Left border only</div>

<!-- Horizontal & Vertical -->
<div class="border-x p-3">Left and right borders</div>
<div class="border-y p-3">Top and bottom borders</div>
```

### Border Radius

```html
<div class="border radius-sm p-3">Small radius (4px)</div>
<div class="border radius-md p-3">Medium radius (8px)</div>
<div class="border radius-lg p-3">Large radius (12px)</div>
```

**Use Cases:**
```html
<!-- Rounded button -->
<button class="btn btn-primary radius-lg">Rounded Button</button>

<!-- Circular avatar -->
<img src="avatar.jpg" class="avatar" style="border-radius: 50%;">

<!-- Card with rounded corners -->
<div class="card radius-md">
  <div class="card-body">Content</div>
</div>
```

### Border Colors

```html
<div class="border border-red p-3">Red border</div>
<div class="border border-blue p-3">Blue border</div>
<div class="border border-green p-3">Green border</div>
<div class="border border-gray p-3">Gray border</div>
```

---

## Sizing

### Width

```html
<!-- Percentage widths -->
<div class="w-100">100% width</div>

<!-- Fixed widths (using gap scale) -->
<div class="w-1">Width: 0.25rem</div>
<div class="w-5">Width: 2rem</div>

<!-- Container widths -->
<div class="w-xs">Extra small container</div>
<div class="w-sm">Small container</div>
<div class="w-md">Medium container</div>
<div class="w-lg">Large container</div>

<!-- Min/Max widths -->
<div class="min-w-sm">Minimum small width</div>
<div class="max-w-md">Maximum medium width</div>
```

**Use Cases:**
```html
<!-- Centered container -->
<div class="max-w-lg mx-auto">
  <h1>Centered Content</h1>
  <p>This content is centered and has a max width</p>
</div>

<!-- Sidebar layout -->
<div class="flex gap-4">
  <aside class="w-sm">Sidebar</aside>
  <main class="flex-1">Main content</main>
</div>
```

### Height

```html
<!-- Percentage heights -->
<div class="h-100">100% height</div>

<!-- Viewport height -->
<div class="h-100vh">Full viewport height</div>

<!-- Min height -->
<div class="min-h-100vh">Minimum full viewport height</div>
```

**Use Cases:**
```html
<!-- Full-screen hero -->
<section class="h-100vh flex items-center justify-center">
  <div class="text-center">
    <h1 class="fs-5xl">Welcome</h1>
    <p class="fs-lg">Scroll down to explore</p>
  </div>
</section>

<!-- Sticky footer -->
<div class="flex flex-col min-h-100vh">
  <header>Header</header>
  <main class="flex-1">Content</main>
  <footer>Footer</footer>
</div>
```

---

## Effects & Animations

### Shadows

```html
<div class="shadow-sm p-4">Small shadow</div>
<div class="shadow-md p-4">Medium shadow</div>
<div class="shadow-lg p-4">Large shadow</div>
```

**Use Cases:**
```html
<!-- Elevated card -->
<div class="card shadow-md">
  <div class="card-body">Elevated content</div>
</div>

<!-- Hover effect -->
<style>
  .hover-lift:hover {
    transform: translateY(-4px);
    box-shadow: var(--shadow-lg);
  }
</style>
<div class="card shadow-sm hover-lift transition-base">
  Hover me
</div>
```

### Opacity

```html
<div class="opacity-100">Fully opaque</div>
<div class="opacity-80">80% opaque</div>
<div class="opacity-50">50% opaque</div>
<div class="opacity-25">25% opaque</div>
```

### Transitions

```html
<div class="transition-fast">Fast transition (150ms)</div>
<div class="transition-base">Base transition (250ms)</div>
<div class="transition-slow">Slow transition (500ms)</div>
```

### Animations

```html
<div class="animate-spin">Spinning element</div>
<div class="animate-bounce">Bouncing element</div>
<div class="animate-fade-in">Fading in</div>
<div class="animate-fade-out">Fading out</div>
<div class="animate-slide-up">Sliding up</div>
```

---

## Responsive Design

### Breakpoints

- `sm`: 640px
- `md`: 768px
- `lg`: 1024px
- `xl`: 1280px

### Mobile-First Approach

Classes apply to all screen sizes unless overridden at larger breakpoints.

```html
<!-- Stack on mobile, row on desktop -->
<div class="flex flex-col flex-row-md gap-4">
  <div>Item 1</div>
  <div>Item 2</div>
</div>

<!-- 1 column on mobile, 2 on tablet, 4 on desktop -->
<div class="grid grid-cols-1 grid-cols-md-2 grid-cols-lg-4 gap-4">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>

<!-- Hide on mobile, show on desktop -->
<div class="d-none d-block-md">Desktop only</div>

<!-- Show on mobile, hide on desktop -->
<div class="d-block d-none-md">Mobile only</div>

<!-- Different padding at different sizes -->
<div class="p-3 p-md-5 p-lg-7">
  Responsive padding
</div>

<!-- Center on mobile, left-align on desktop -->
<p class="text-center text-left-md">
  Responsive text alignment
</p>
```

---

## Best Practices

### ✅ Do's

1. **Combine utilities** for complex layouts
2. **Use responsive variants** for mobile-first design
3. **Leverage flexbox and grid** for layouts
4. **Use semantic color classes** for consistency
5. **Apply spacing consistently** using the scale

### ❌ Don'ts

1. **Don't mix layout systems** (flexbox + grid on same element)
2. **Don't override utilities** with inline styles
3. **Don't use arbitrary values** - stick to the scale
4. **Don't forget responsive design**
5. **Don't use utilities for complex components** - create component classes instead

---

## Quick Reference

**Most Common Utilities:**

```html
<!-- Layout -->
flex, grid, d-block, d-none, relative, absolute

<!-- Spacing -->
m-0 to m-9, p-0 to p-9, gap-0 to gap-9, mx-auto

<!-- Flexbox -->
flex-col, flex-row, items-center, justify-between, flex-1

<!-- Typography -->
fs-xs to fs-5xl, fw-400 to fw-700, text-center

<!-- Colors -->
bg-primary, text-primary, bg-surface, text-muted

<!-- Sizing -->
w-100, h-100vh, max-w-lg, min-h-100vh

<!-- Effects -->
shadow-md, opacity-50, transition-base
```

---

For customization options, see [Customization Guide](customization.md).
