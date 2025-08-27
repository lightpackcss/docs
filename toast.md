# Toast Component

Lightpack Toasts provide temporary, stackable notification popups with color variants, close buttons, auto-dismiss, sticky support, and multi-positioning.

**Classes:**
- `.toast` (base)
- `.toast-success`, `.toast-warning`, `.toast-danger`, `.toast-info` (color variants)
- `.toast-close` (dismiss button)
- `.toast-bottom-right`, `.toast-bottom-left`, `.toast-top-right`, `.toast-top-left` (container positions)

**JS API:**
- `Lightpack.showToast(message, variant, sticky, position)`
  - `message` (string): Toast content
  - `variant` (string): `info`, `success`, `danger`, `warning` (optional, default: `info`)
  - `sticky` (bool): If `true`, does not auto-dismiss (optional, default: `false`)
  - `position` (string): `bottom-right`, `bottom-left`, `top-right`, `top-left` (optional, default: `bottom-right`)

---

## Features
- **Color Variants:** Info, Success, Warning, Danger
- **Positions:** Bottom Right, Bottom Left, Top Right, Top Left
- **Sticky Toasts:** Don't auto-dismiss, require manual close
- **Dismiss Button:** `.toast-close` for manual dismiss
- **Stacking:** Multiple toasts stack per position

---

## Examples

<div class="demo-container">
  <div style="display: flex; flex-wrap: wrap; gap: 1em; margin-bottom: 1em;">
    <div>
      <strong>Bottom Right</strong><br>
      <button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'BR info toast', type: 'info', sticky: false, position: 'bottom-right' })">Info</button>
      <button class="btn btn-success" onclick="Lightpack.showToast({ message: 'BR success toast', type: 'success', sticky: false, position: 'bottom-right' })">Success</button>
      <button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'BR error toast', type: 'danger', sticky: false, position: 'bottom-right' })">Error</button>
      <button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'BR warning toast', type: 'warning', sticky: false, position: 'bottom-right' })">Warning</button>
      <button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'BR sticky toast', type: 'info', sticky: true, position: 'bottom-right' })">Sticky</button>
    </div>
    <div>
      <strong>Bottom Left</strong><br>
      <button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'BL info toast', type: 'info', sticky: false, position: 'bottom-left' })">Info</button>
      <button class="btn btn-success" onclick="Lightpack.showToast({ message: 'BL success toast', type: 'success', sticky: false, position: 'bottom-left' })">Success</button>
      <button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'BL error toast', type: 'danger', sticky: false, position: 'bottom-left' })">Error</button>
      <button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'BL warning toast', type: 'warning', sticky: false, position: 'bottom-left' })">Warning</button>
      <button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'BL sticky toast', type: 'info', sticky: true, position: 'bottom-left' })">Sticky</button>
    </div>
    <div>
      <strong>Top Right</strong><br>
      <button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'TR info toast', type: 'info', sticky: false, position: 'top-right' })">Info</button>
      <button class="btn btn-success" onclick="Lightpack.showToast({ message: 'TR success toast', type: 'success', sticky: false, position: 'top-right' })">Success</button>
      <button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'TR error toast', type: 'danger', sticky: false, position: 'top-right' })">Error</button>
      <button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'TR warning toast', type: 'warning', sticky: false, position: 'top-right' })">Warning</button>
      <button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'TR sticky toast', type: 'info', sticky: true, position: 'top-right' })">Sticky</button>
    </div>
    <div>
      <strong>Top Left</strong><br>
      <button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'TL info toast', type: 'info', sticky: false, position: 'top-left' })">Info</button>
      <button class="btn btn-success" onclick="Lightpack.showToast({ message: 'TL success toast', type: 'success', sticky: false, position: 'top-left' })">Success</button>
      <button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'TL error toast', type: 'danger', sticky: false, position: 'top-left' })">Error</button>
      <button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'TL warning toast', type: 'warning', sticky: false, position: 'top-left' })">Warning</button>
      <button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'TL sticky toast', type: 'info', sticky: true, position: 'top-left' })">Sticky</button>
    </div>
  </div>
</div>

**Usage**
```html
<!-- Bottom right -->
<strong>Bottom Right</strong><br>
<button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'BR info toast', type: 'info', sticky: false, position: 'bottom-right' })">Info</button>
<button class="btn btn-success" onclick="Lightpack.showToast({ message: 'BR success toast', type: 'success', sticky: false, position: 'bottom-right' })">Success</button>
<button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'BR error toast', type: 'danger', sticky: false, position: 'bottom-right' })">Error</button>
<button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'BR warning toast', type: 'warning', sticky: false, position: 'bottom-right' })">Warning</button>
<button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'BR sticky toast', type: 'info', sticky: true, position: 'bottom-right' })">Sticky</button>

<!-- Bottom left -->
<strong>Bottom Left</strong><br>
<button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'BL info toast', type: 'info', sticky: false, position: 'bottom-left' })">Info</button>
<button class="btn btn-success" onclick="Lightpack.showToast({ message: 'BL success toast', type: 'success', sticky: false, position: 'bottom-left' })">Success</button>
<button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'BL error toast', type: 'danger', sticky: false, position: 'bottom-left' })">Error</button>
<button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'BL warning toast', type: 'warning', sticky: false, position: 'bottom-left' })">Warning</button>
<button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'BL sticky toast', type: 'info', sticky: true, position: 'bottom-left' })">Sticky</button>

<!-- Top right -->
<strong>Top Right</strong><br>
<button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'TR info toast', type: 'info', sticky: false, position: 'top-right' })">Info</button>
<button class="btn btn-success" onclick="Lightpack.showToast({ message: 'TR success toast', type: 'success', sticky: false, position: 'top-right' })">Success</button>
<button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'TR error toast', type: 'danger', sticky: false, position: 'top-right' })">Error</button>
<button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'TR warning toast', type: 'warning', sticky: false, position: 'top-right' })">Warning</button>
<button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'TR sticky toast', type: 'info', sticky: true, position: 'top-right' })">Sticky</button>

<!-- Top left -->
<strong>Top Left</strong><br>
<button class="btn btn-primary" onclick="Lightpack.showToast({ message: 'TL info toast', type: 'info', sticky: false, position: 'top-left' })">Info</button>
<button class="btn btn-success" onclick="Lightpack.showToast({ message: 'TL success toast', type: 'success', sticky: false, position: 'top-left' })">Success</button>
<button class="btn btn-danger" onclick="Lightpack.showToast({ message: 'TL error toast', type: 'danger', sticky: false, position: 'top-left' })">Error</button>
<button class="btn btn-warning" onclick="Lightpack.showToast({ message: 'TL warning toast', type: 'warning', sticky: false, position: 'top-left' })">Warning</button>
<button class="btn btn-dark" onclick="Lightpack.showToast({ message: 'TL sticky toast', type: 'info', sticky: true, position: 'top-left' })">Sticky</button>
```

---