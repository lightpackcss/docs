# Drawer Component

**Classes:** `.drawer`, `.drawer.open`, `.drawer-backdrop`, `.drawer-panel`, `.drawer-left`, `.drawer-left.open`

**Features:**
- Slide-in drawer from right or left
- Backdrop and responsive width

**Example**

<div class="demo-container">
  <button class="btn btn-primary" data-drawer-open="left-drawer">Left Drawer</button>
  <div class="drawer drawer-left" id="left-drawer">
    <div class="drawer-backdrop"></div>
    <div class="drawer-panel">Drawer content here</div>
  </div>
</div>

**Usage:**
```html
<button data-drawer-open="left-drawer">Open Left Drawer</button>
<div class="drawer drawer-left" id="left-drawer">
  <div class="drawer-backdrop"></div>
  <div class="drawer-panel">
    <button data-drawer-close>Close</button>
    <p>Drawer content here</p>
  </div>
</div>
```

**Example**

<div class="demo-container">
  <button class="btn btn-primary" data-drawer-open="right-drawer">Right Drawer</button>
  <div class="drawer drawer-right" id="right-drawer">
    <div class="drawer-backdrop"></div>
    <div class="drawer-panel">Drawer content here</div>
  </div>
</div>

**Usage:**
```html
<button data-drawer-open="right-drawer">Open Right Drawer</button>
<div class="drawer" id="right-drawer">
  <div class="drawer-backdrop"></div>
  <div class="drawer-panel">
    <button data-drawer-close>Close</button>
    <p>Drawer content here</p>
  </div>
</div>
```

**JS Interactivity:**
- Use `data-drawer-open="drawerId"` on trigger buttons
- Use `data-drawer-close` on close buttons inside drawer
- Clicking backdrop or pressing ESC closes the drawer
- Default drawer slides from right; use `.drawer-left` for left side

**JavaScript API:**
```javascript
// Drawers are initialized automatically via Lightpack.initDrawers()
// Called on DOMContentLoaded by Lightpack.initAll()
```

---
