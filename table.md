# Table Component

**Classes:** `.table`, `.table-hover`, `.table-bordered`, `.table-responsive`, `.table-responsive-sm`, `.table-responsive-md`, `.table-responsive-lg`, `.table-responsive-xl`

**Features:**
- Modern, responsive tables
- Hover, bordered variants
- Responsive wrappers for horizontal scrolling on small screens
- Breakpoint-specific responsive behavior

**Example**

<div class="demo-container">
  <table class="table table-bordered table-hover">
    <thead>
      <tr>
        <th>Name</th>
        <th>Position</th>
        <th>Email</th>
        <th>Status</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Alice Smith</td>
        <td>Designer</td>
        <td>alice@example.com</td>
        <td>Active</td>
      </tr>
      <tr>
        <td>Bob Lee</td>
        <td>Developer</td>
        <td>bob@example.com</td>
        <td>Inactive</td>
      </tr>
      <tr>
        <td>Charlie Kim</td>
        <td>PM</td>
        <td>charlie@example.com</td>
        <td>Active</td>
      </tr>
    </tbody>
  </table>
</div>

**Usage:**
```html
<table class="table table-bordered table-hover">
  <thead>
    <tr>
      <th>Name</th>
      <th>Position</th>
      <th>Email</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alice Smith</td>
      <td>Designer</td>
      <td>alice@example.com</td>
      <td>Active</td>
    </tr>
    <tr>
      <td>Bob Lee</td>
      <td>Developer</td>
      <td>bob@example.com</td>
      <td>Inactive</td>
    </tr>
    <tr>
      <td>Charlie Kim</td>
      <td>PM</td>
      <td>charlie@example.com</td>
      <td>Active</td>
    </tr>
  </tbody>
</table>
```

**Responsive Tables**

Wrap tables in responsive containers to enable horizontal scrolling on smaller screens:

```html
<!-- Always responsive -->
<div class="table-responsive">
  <table class="table">...</table>
</div>

<!-- Responsive only below sm breakpoint (640px) -->
<div class="table-responsive-sm">
  <table class="table">...</table>
</div>

<!-- Responsive only below md breakpoint (768px) -->
<div class="table-responsive-md">
  <table class="table">...</table>
</div>

<!-- Responsive only below lg breakpoint (1024px) -->
<div class="table-responsive-lg">
  <table class="table">...</table>
</div>

<!-- Responsive only below xl breakpoint (1280px) -->
<div class="table-responsive-xl">
  <table class="table">...</table>
</div>
```

**Customization:**
- Add utility classes for custom color, spacing, or typography
- Use `.table-hover` for row hover effects
- Use `.table-bordered` for borders on all cells

---
