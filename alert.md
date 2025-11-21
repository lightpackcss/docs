# Alert Component

**Classes:** `.alert`, `.alert-content`, `.alert-title`, `.alert-close`, `.alert-success`, `.alert-warning`, `.alert-danger`, `.alert-info`

**Features:**
- Dismissible alerts
- Color/status variants: success, warning, danger, info
- Includes close button: `.alert-close`
- Accessible markup

**Example**

<div class="demo-container">
  <div class="alert alert-success">
    <div class="alert-content">
      <div class="alert-title">Success!</div>
      <div>Your action was completed successfully.</div>
    </div>
    <button class="alert-close">&times;</button>
  </div>
  <div class="alert alert-danger">
    <div class="alert-content">
      <div class="alert-title">Error!</div>
      <div>Something went wrong. Please try again.</div>
    </div>
    <button class="alert-close">&times;</button>
  </div>
  <div class="alert alert-warning">
    <div class="alert-content">
      <div class="alert-title">Warning!</div>
      <div>Please review your input before proceeding.</div>
    </div>
    <button class="alert-close">&times;</button>
  </div>
  <div class="alert alert-info">
    <div class="alert-content">
      <div class="alert-title">Info</div>
      <div>Here's some helpful information.</div>
    </div>
    <button class="alert-close">&times;</button>
  </div>
</div>

**Usage:**
```html
<!-- Simple alert -->
<div class="alert alert-success">
  <span>Success message!</span>
  <button class="alert-close">&times;</button>
</div>

<!-- Alert with title and content -->
<div class="alert alert-success">
  <div class="alert-content">
    <div class="alert-title">Success!</div>
    <div>Your action was completed successfully.</div>
  </div>
  <button class="alert-close">&times;</button>
</div>

<div class="alert alert-danger">
  <div class="alert-content">
    <div class="alert-title">Error!</div>
    <div>Something went wrong.</div>
  </div>
  <button class="alert-close">&times;</button>
</div>
```

**JS Interactivity:**
- Clicking `.alert-close` removes the alert

**Customization:**
- Override colors via variables or utility classes
- Add icons or extra content as needed

---