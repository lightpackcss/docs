# Lightpack CSS Utilities

This file lists **every available utility class** in Lightpack CSS, grouped by category. All utilities are defined in `/src/css/_utilities.css`.

---

## Spacing Utilities
### Gap Utilities
- `.gap-0` ... `.gap-9` - Gap on both axes
- `.gap-x-0` ... `.gap-x-9` - Column gap only
- `.gap-y-0` ... `.gap-y-9` - Row gap only

### Margin Utilities
- `.m-0` ... `.m-9` - All sides
- `.mt-0` ... `.mt-9` - Top
- `.mr-0` ... `.mr-9` - Right
- `.mb-0` ... `.mb-9` - Bottom
- `.ml-0` ... `.ml-9` - Left
- `.mx-0` ... `.mx-9` - Horizontal (left + right)
- `.my-0` ... `.my-9` - Vertical (top + bottom)
- `.mx-auto` - Horizontal auto margin (centering)

### Padding Utilities
- `.p-0` ... `.p-9` - All sides
- `.pt-0` ... `.pt-9` - Top
- `.pr-0` ... `.pr-9` - Right
- `.pb-0` ... `.pb-9` - Bottom
- `.pl-0` ... `.pl-9` - Left
- `.px-0` ... `.px-9` - Horizontal (left + right)
- `.py-0` ... `.py-9` - Vertical (top + bottom)

## Offset Utilities
- `.top-0` ... `.top-9`, `.right-0` ... `.right-9`, `.bottom-0` ... `.bottom-9`, `.left-0` ... `.left-9`

## Layout Utilities
### Display
- `.d-block`, `.d-inline`, `.d-inline-block`, `.d-none`
- Responsive: `.d-block-sm/md/lg/xl`, `.d-inline-sm/md/lg/xl`, `.d-inline-block-sm/md/lg/xl`, `.d-none-sm/md/lg/xl`

### Visibility & Position
- `.visibility-hidden`, `.visibility-visible`
- `.static`, `.relative`, `.absolute`, `.fixed`, `.sticky`

### Overflow
- `.overflow-auto`, `.overflow-scroll`, `.overflow-hidden`
- `.overflow-x-auto`, `.overflow-x-scroll`, `.overflow-x-hidden`
- `.overflow-y-auto`, `.overflow-y-scroll`, `.overflow-y-hidden`
- `.scroll-smooth`

### Flexbox
- `.flex`, `.inline-flex`
- `.flex-row`, `.flex-row-reverse`, `.flex-col`, `.flex-col-reverse`
- `.flex-wrap`, `.flex-nowrap`, `.flex-wrap-reverse`
- `.flex-1`, `.flex-auto`, `.flex-initial`, `.flex-none`
- `.grow`, `.grow-0`, `.shrink`, `.shrink-0`
- Responsive: `.flex-sm/md/lg/xl`, `.flex-row-sm/md/lg/xl`, `.flex-col-sm/md/lg/xl`, `.flex-wrap-sm/md/lg/xl`

### Flexbox Alignment
- **Justify Content:** `.justify-start`, `.justify-center`, `.justify-between`, `.justify-end`, `.justify-around`, `.justify-evenly`
- **Align Items:** `.items-start`, `.items-center`, `.items-end`, `.items-baseline`, `.items-stretch`
- **Align Content:** `.content-start`, `.content-center`, `.content-end`, `.content-between`, `.content-around`, `.content-evenly`
- **Align Self:** `.self-auto`, `.self-start`, `.self-center`, `.self-end`, `.self-stretch`, `.self-baseline`
- Responsive: `.items-center-sm/md/lg/xl`, `.justify-center-sm/md/lg/xl`, etc.

### Centering Utility
- `.center-content` - Flexbox centering (both axes)

## Content Utilities
- `.truncate`, `.text-ellipsis`, `.whitespace-nowrap`, `.break-words`

## Filter Utilities
- `.blur-sm`, `.brightness-110`

## Backdrop Filter Utilities
- `.backdrop-blur`, `.backdrop-brightness-125`

## Object Fit/Position Utilities
- `.object-cover`, `.object-contain`, `.object-center`

## Animation Utilities
- `.animate-spin`, `.animate-fade-in`, `.animate-fade-out`, `.animate-slide-up`, `.animate-bounce`
- `.duration-200`, `.duration-500`, `.duration-1000`, `.delay-100`, `.delay-300`, `.ease-in-out`

## Grid Utilities
- `.grid`, `.grid-cols-1` ... `.grid-cols-6`, `.grid-cols-none`, `.grid-rows-1` ... `.grid-rows-6`, `.grid-rows-none`
- `.grid-flow-row`, `.grid-flow-col`, `.grid-flow-dense`
- `.grid-rows-min`, `.grid-rows-max`, `.grid-rows-auto`, `.grid-cols-min`, `.grid-cols-max`, `.grid-cols-auto`

## Typography Utilities
### Font Sizes
- `.fs-xs`, `.fs-sm`, `.fs-base`, `.fs-md`, `.fs-lg`, `.fs-xl`, `.fs-2xl`, `.fs-3xl`, `.fs-4xl`, `.fs-5xl`

### Font Weights
- `.fw-100`, `.fw-200`, `.fw-300`, `.fw-400`, `.fw-500`, `.fw-600`, `.fw-700`, `.fw-800`, `.fw-900`

### Text Alignment
- `.text-left`, `.text-center`, `.text-right`, `.text-justify`
- Responsive: `.text-left-sm/md/lg/xl`, `.text-center-sm/md/lg/xl`, `.text-right-sm/md/lg/xl`, `.text-justify-sm/md/lg/xl`

### Line Height
- `.lh-base`

### Vertical Alignment
- `.align-baseline`, `.align-top`, `.align-middle`, `.align-bottom`, `.align-text-top`, `.align-text-bottom`

## Color Utilities
### Natural Color Backgrounds
- `.bg-red`, `.bg-red-light`, `.bg-red-dark`
- `.bg-pink`, `.bg-pink-light`, `.bg-pink-dark`
- `.bg-orange`, `.bg-orange-light`, `.bg-orange-dark`
- `.bg-yellow`, `.bg-yellow-light`, `.bg-yellow-dark`
- `.bg-green`, `.bg-green-light`, `.bg-green-dark`
- `.bg-teal`, `.bg-teal-light`, `.bg-teal-dark`
- `.bg-blue`, `.bg-blue-light`, `.bg-blue-dark`
- `.bg-indigo`, `.bg-indigo-light`, `.bg-indigo-dark`
- `.bg-purple`, `.bg-purple-light`, `.bg-purple-dark`
- `.bg-brown`, `.bg-brown-light`, `.bg-brown-dark`
- `.bg-gray`, `.bg-gray-light`, `.bg-gray-dark`
- `.bg-black`, `.bg-black-light`, `.bg-black-dark`
- `.bg-white`, `.bg-white-light`
- `.bg-muted`

### Semantic Color Backgrounds
- `.bg-primary`, `.bg-primary-light`, `.bg-primary-lighter`, `.bg-primary-dark`
- `.bg-secondary`, `.bg-secondary-light`, `.bg-secondary-lighter`, `.bg-secondary-dark`
- `.bg-success`, `.bg-success-light`, `.bg-success-lighter`, `.bg-success-dark`
- `.bg-warning`, `.bg-warning-light`, `.bg-warning-lighter`, `.bg-warning-dark`
- `.bg-danger`, `.bg-danger-light`, `.bg-danger-lighter`, `.bg-danger-dark`
- `.bg-info`, `.bg-info-light`, `.bg-info-lighter`, `.bg-info-dark`
- `.bg-accent`, `.bg-accent-light`, `.bg-accent-lighter`, `.bg-accent-dark`
- `.bg-background`, `.bg-surface`, `.bg-surface-dark`, `.bg-surface-alt`, `.bg-border`, `.bg-border-dark`

### Natural Color Text
- `.text-red`, `.text-red-light`, `.text-red-dark`
- `.text-pink`, `.text-pink-light`, `.text-pink-dark`
- `.text-orange`, `.text-orange-light`, `.text-orange-dark`
- `.text-yellow`, `.text-yellow-light`, `.text-yellow-dark`
- `.text-green`, `.text-green-light`, `.text-green-dark`
- `.text-teal`, `.text-teal-light`, `.text-teal-dark`
- `.text-blue`, `.text-blue-light`, `.text-blue-dark`
- `.text-indigo`, `.text-indigo-light`, `.text-indigo-dark`
- `.text-purple`, `.text-purple-light`, `.text-purple-dark`
- `.text-brown`, `.text-brown-light`, `.text-brown-dark`
- `.text-gray`, `.text-gray-light`, `.text-gray-dark`
- `.text-black`, `.text-black-light`, `.text-black-dark`
- `.text-white`

### Semantic Color Text
- `.text-primary`, `.text-primary-light`, `.text-primary-lighter`, `.text-primary-dark`
- `.text-secondary`, `.text-secondary-light`, `.text-secondary-lighter`, `.text-secondary-dark`
- `.text-success`, `.text-success-light`, `.text-success-lighter`, `.text-success-dark`
- `.text-warning`, `.text-warning-light`, `.text-warning-lighter`, `.text-warning-dark`
- `.text-danger`, `.text-danger-light`, `.text-danger-lighter`, `.text-danger-dark`
- `.text-info`, `.text-info-light`, `.text-info-lighter`, `.text-info-dark`
- `.text-accent`, `.text-accent-light`, `.text-accent-lighter`, `.text-accent-dark`
- `.text`, `.text-muted`, `.text-inverse`

## Border Utilities
### Border Sides
- `.border` - All sides
- `.border-0` - No border
- `.border-top`, `.border-right`, `.border-bottom`, `.border-left`
- `.border-x` - Left + right
- `.border-y` - Top + bottom
- `.border-top-0`, `.border-right-0`, `.border-bottom-0`, `.border-left-0`
- `.border-x-0`, `.border-y-0`

### Border Colors
- `.border-red`, `.border-green`, `.border-blue`, `.border-indigo`, `.border-gray`, `.border-black`, `.border-white`

### Border Radius
- `.radius-sm`, `.radius-md`, `.radius-lg`

## Shadow Utilities
- `.shadow-sm`, `.shadow-md`, `.shadow-lg`

## Width/Height Utilities
### Width
- `.w-1` ... `.w-9` - Fixed widths using gap scale
- `.w-100` - 100% width
- `.w-xs`, `.w-sm`, `.w-md`, `.w-lg` - Container widths
- `.min-w-xs`, `.min-w-sm`, `.min-w-md`, `.min-w-lg` - Min widths
- `.max-w-xs`, `.max-w-sm`, `.max-w-md`, `.max-w-lg` - Max widths

### Height
- `.h-1` ... `.h-9` - Fixed heights using gap scale
- `.h-100` - 100% height
- `.h-100vh` - 100vh height
- `.min-h-100vh` - Min height 100vh
- `.max-h-50`, `.max-h-75` - Max heights

## Opacity Utilities
- `.opacity-100`, `.opacity-80`, `.opacity-50`, `.opacity-25`, `.opacity-disabled`, `.opacity-overlay`

## Z-Index Utilities
- `.z-0`, `.z-10`, `.z-20`, `.z-30`, `.z-40`, `.z-50`

## Transition Utilities
- `.transition-fast`, `.transition-base`, `.transition-slow`

## Container Width Utilities
- `.container-xs`, `.container-sm`, `.container-md`, `.container-lg`, `.container-xl`

## Accessibility Utilities
- `.sr-only`

## Cursor Utilities
- `.cursor-pointer`, `.cursor-disabled`, `.cursor-default`, `.cursor-text`, `.cursor-move`, `.cursor-grab`, `.cursor-grabbing`, `.cursor-wait`, `.cursor-crosshair`, `.cursor-zoom-in`, `.cursor-zoom-out`, `.cursor-help`, `.pointer-events-none`, `.pointer-events-auto`, `.select-none`, `.select-text`, `.select-all`, `.select-auto`

## Scroll Snap Utilities
- `.snap-x`, `.snap-y`, `.snap-mandatory`, `.snap-proximity`, `.snap-start`, `.snap-center`, `.snap-end`

## Aspect Ratio Utilities
- `.aspect-1-1`, `.aspect-16-9`, `.aspect-4-3`

## Text Decoration & Transform Utilities
- `.underline`, `.line-through`, `.uppercase`, `.lowercase`, `.capitalize`

## List Style Utilities
- `.list-none`, `.list-disc`, `.list-decimal`

---

## Usage Examples

### Spacing Utilities

<div class="demo-container" style="display:flex; gap:1rem;">
  <div class="bg-muted p-3 m-2">.p-3 .m-2</div>
  <div class="bg-muted p-1 m-4">.p-1 .m-4</div>
</div>

```html
<div class="bg-muted p-3 m-2">.p-3 .m-2</div>
<div class="bg-muted p-1 m-4">.p-1 .m-4</div>
```

### Layout Utilities

<div class="demo-container" style="display:flex; gap:1rem;">
  <div class="d-inline bg-muted p-2">.d-inline</div>
  <div class="d-block bg-muted p-2">.d-block</div>
  <div class="d-none bg-muted p-2">.d-none (hidden)</div>
</div>

```html
<div class="d-inline bg-muted p-2">.d-inline</div>
<div class="d-block bg-muted p-2">.d-block</div>
<div class="d-none bg-muted p-2">.d-none (hidden)</div>
```

### Flex Utilities

<div class="demo-container" style="display:flex; gap:1rem;">
  <div class="flex flex-row gap-2 p-2">
    <div class="bg-muted p-2">A</div>
    <div class="bg-muted p-2">B</div>
    <div class="bg-muted p-2">C</div>
  </div>
</div>

```html
<div class="flex flex-row gap-2 bg-muted p-2">
  <span class="bg-indigo p-1">1</span>
  <span class="bg-green p-1">2</span>
  <span class="bg-red p-1">3</span>
</div>
```

### Grid Utilities

<div class="demo-container">
  <div class="grid grid-cols-3 gap-2">
    <div class="bg-muted p-2">A</div>
    <div class="bg-muted p-2">B</div>
    <div class="bg-muted p-2">C</div>
  </div>
</div>

```html
<div class="grid grid-cols-3 gap-2">
  <div class="bg-muted p-2">A</div>
  <div class="bg-muted p-2">B</div>
  <div class="bg-muted p-2">C</div>
</div>
```

### Typography Utilities

<div class="demo-container" style="display:flex; flex-direction:column; gap:0.5rem;">
  <span class="fs-xs">.fs-xs</span>
  <span class="fs-lg">.fs-lg</span>
  <span class="fw-700">.fw-700</span>
  <span class="text-center">.text-center (centered text)</span>
</div>

```html
<span class="fs-xs">.fs-xs</span>
<span class="fs-lg">.fs-lg</span>
<span class="fw-700">.fw-700</span>
<span class="text-center">.text-center (centered text)</span>
```

### Color Utilities

<div class="demo-container" style="display:flex; gap:1rem;">
  <span class="bg-indigo text-white p-2">.bg-indigo .text-white</span>
  <span class="bg-green text-white p-2">.bg-green .text-white</span>
  <span class="bg-red text-white p-2">.bg-red .text-white</span>
</div>

```html
<span class="bg-indigo text-white p-2">.bg-indigo .text-white</span>
<span class="bg-green text-white p-2">.bg-green .text-white</span>
<span class="bg-red text-white p-2">.bg-red .text-white</span>
```

### Border & Radius Utilities

<div class="demo-container" style="display:flex; gap:1rem;">
  <span class="border border-indigo radius-sm p-2">.border .border-indigo .radius-sm</span>
  <span class="border border-red radius-lg p-2">.border .border-red .radius-lg</span>
</div>

```html
<span class="border border-indigo radius-sm p-2">.border .border-indigo .radius-sm</span>
<span class="border border-red radius-lg p-2">.border .border-red .radius-lg</span>
```

### Shadow Utilities

<div class="demo-container" style="display:flex; gap:1rem;">
  <span class="shadow-sm p-2">.shadow-sm</span>
  <span class="shadow-md p-2">.shadow-md</span>
  <span class="shadow-lg p-2">.shadow-lg</span>
</div>

```html
<span class="shadow-sm p-2">.shadow-sm</span>
<span class="shadow-md p-2">.shadow-md</span>
<span class="shadow-lg p-2">.shadow-lg</span>
```

### Width/Height Utilities

<div class="demo-container" style="display:flex; gap:1rem; align-items:center;">
  <div class="bg-muted w-xs h-100 p-2">.w-xs .h-100</div>
  <div class="bg-muted w-md h-100 p-2">.w-md .h-100</div>
  <div class="bg-muted w-lg h-100 p-2">.w-lg .h-100</div>
</div>

```html
<div class="bg-muted w-xs h-100 p-2">.w-xs .h-100</div>
<div class="bg-muted w-md h-100 p-2">.w-md .h-100</div>
<div class="bg-muted w-lg h-100 p-2">.w-lg .h-100</div>
```

### Opacity Utilities

<div class="demo-container" style="display:flex; gap:1rem;">
  <span class="bg-indigo text-white p-2 opacity-100">.opacity-100</span>
  <span class="bg-indigo text-white p-2 opacity-50">.opacity-50</span>
  <span class="bg-indigo text-white p-2 opacity-25">.opacity-25</span>
</div>

```html
<span class="bg-indigo text-white p-2 opacity-100">.opacity-100</span>
<span class="bg-indigo text-white p-2 opacity-50">.opacity-50</span>
<span class="bg-indigo text-white p-2 opacity-25">.opacity-25</span>
```

### Animation Utilities

<div class="demo-container" style="display:flex; gap:1rem; align-items:center;">
  <span class="animate-spin bg-indigo text-white p-2">spin</span>
  <span class="animate-bounce bg-green text-white p-2">bounce</span>
</div>

```html
<span class="animate-spin bg-indigo text-white p-2">spin</span>
<span class="animate-bounce bg-green text-white p-2">bounce</span>
```

---
