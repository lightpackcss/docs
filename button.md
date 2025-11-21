# Button Component

**Classes:** `.btn`, `.btn-primary`, `.btn-secondary`, `.btn-success`, `.btn-danger`, `.btn-warning`, `.btn-info`, `.btn-outline`, `.btn-ghost`, `.btn-sm`, `.btn-lg`, `.btn-icon`, `.btn:disabled`, `.btn.disabled`

**Features:**
- Multiple color and style variants
- Outline and ghost styles
- Disabled state support
- Icon-only and size modifiers
- Uses design tokens for all styles

**Example**

<div class="demo-container">
    <div class="mb-3">
        <button class="btn btn-primary">Primary</button>
        <button class="btn btn-secondary">Secondary</button>
        <button class="btn btn-success">Success</button>
        <button class="btn btn-danger">Danger</button>
    </div>
    <button class="btn btn-warning">Warning</button>
    <button class="btn btn-info">Info</button>
</div>

**Usage**
```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-danger">Danger</button>
<button class="btn btn-warning">Warning</button>
<button class="btn btn-info">Info</button>
```

**Ghost Buttons**

<div class="demo-container">
    <div class="mb-3">
        <button class="btn btn-primary btn-ghost">Primary Ghost</button>
        <button class="btn btn-success btn-ghost">Success Ghost</button>
        <button class="btn btn-danger btn-ghost">Danger Ghost</button>
    </div>
    <button class="btn btn-warning btn-ghost">Warning Ghost</button>
    <button class="btn btn-info btn-ghost">Info Ghost</button>
</div>

```html
<button class="btn btn-primary btn-ghost">Primary Ghost</button>
<button class="btn btn-success btn-ghost">Success Ghost</button>
<button class="btn btn-danger btn-ghost">Danger Ghost</button>
```

**Disabled State**

<div class="demo-container">
    <button class="btn btn-primary" disabled>Primary</button>
    <button class="btn btn-secondary" disabled>Secondary</button>
    <button class="btn btn-danger" disabled>Danger</button>
</div>

**Usage**
```html
<button class="btn btn-primary disabled">Primary</button>
<button class="btn btn-secondary disabled">Secondary</button>
<button class="btn btn-danger disabled">Danger</button>
<button class="btn btn-success disabled">Success</button>
<button class="btn btn-info disabled">Info</button>
<button class="btn btn-ghost disabled">Ghost</button>
```

**Example**

<div class="demo-container">
    <div class="mb-3">
        <button class="btn btn-primary btn-outline">Primary</button>
        <button class="btn btn-secondary btn-outline">Secondary</button>
        <button class="btn btn-danger btn-outline">Danger</button>
        <button class="btn btn-success btn-outline">Success</button>
    </div>
    <button class="btn btn-info btn-outline">Info</button>
    <button class="btn btn-ghost btn-outline">Ghost</button>
</div>

**Usage:**
```html
<button class="btn btn-primary btn-outline">Primary</button>
<button class="btn btn-secondary btn-outline">Secondary</button>
<button class="btn btn-danger btn-outline">Danger</button>
<button class="btn btn-success btn-outline">Success</button>
<button class="btn btn-warning btn-outline">Warning</button>
<button class="btn btn-info btn-outline">Info</button>
```

**Button Sizes**

<div class="demo-container">
    <button class="btn btn-primary btn-sm">Small</button>
    <button class="btn btn-primary">Default</button>
    <button class="btn btn-primary btn-lg">Large</button>
</div>

```html
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary">Default</button>
<button class="btn btn-primary btn-lg">Large</button>
```

**Icon Button**

<div class="demo-container">
    <button class="btn btn-primary btn-icon">×</button>
    <button class="btn btn-secondary btn-icon">+</button>
</div>

```html
<button class="btn btn-primary btn-icon">×</button>
<button class="btn btn-secondary btn-icon">+</button>
```

**Customization:**
- Add more color variants by extending variables
- Combine with utility classes for spacing/layout

---