# Accordion Component

**Classes:** `.collapsible`, `.collapse-item`, `.collapse-toggle`, `.collapse-content`, `.collapse-icon`, `collapse-indicator`

**Features:**
- Fully customizable UI
- Single or multiple open panels at a time (by default)

**Example**

<div class="demo-container">
  <div class="collapsible">
    <div class="collapse-item">
        <a class="collapse-toggle">Section 1</a>
        <div class="collapse-content">Content 1</div>
    </div>

    <div class="collapse-item">
        <a class="collapse-toggle">Section 2</a>
        <div class="collapse-content">Content 2</div>
    </div>

    <div class="collapse-item">
        <a class="collapse-toggle">
            <span>Section 3</span>
            <span class="collapse-indicator">+</span>
        </a>
        <div class="collapse-content">Content 3</div>
    </div>

    <div class="collapse-item">
        <a class="collapse-toggle">
            <span>Section 3</span>
            <span class="collapse-indicator" data-open="▼" data-closed="►">►</span>
        </a>
        <div class="collapse-content">Content 3</div>
    </div>

    <div class="collapse-item">
        <a class="collapse-toggle">
            <span>Section 3</span>
            <span class="collapse-indicator" data-open="Hide" data-closed="Show">Show</span>
        </a>
        <div class="collapse-content">Content 3</div>
    </div>

    <div class="collapse-item">
        <a class="collapse-toggle">
            <span>Section 3</span>
            <span class="collapse-indicator">
                <svg class="collapse-icon" width="1em" height="1em" viewBox="0 0 20 20" fill="none" aria-hidden="true" focusable="false">
                    <path d="M7 5l5 5-5 5" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
            </span>
        </a>
        <div class="collapse-content">Content 3</div>
    </div>
  </div>
</div>

**Usage**
```html
<div class="collapsible">
  <div class="collapse-item">
      <a class="collapse-toggle">Section 1</a>
      <div class="collapse-content">Content 1</div>
  </div>

  <div class="collapse-item">
      <a class="collapse-toggle">Section 2</a>
      <div class="collapse-content">Content 2</div>
  </div>

  <div class="collapse-item">
      <a class="collapse-toggle">
          <span>Section 3</span>
          <span class="collapse-indicator">+</span>
      </a>
      <div class="collapse-content">Content 3</div>
  </div>

  <div class="collapse-item">
      <a class="collapse-toggle">
          <span>Section 3</span>
          <span class="collapse-indicator" data-open="▼" data-closed="►">►</span>
      </a>
      <div class="collapse-content">Content 3</div>
  </div>

  <div class="collapse-item">
      <a class="collapse-toggle">
          <span>Section 3</span>
          <span class="collapse-indicator" data-open="Hide" data-closed="Show">Show</span>
      </a>
      <div class="collapse-content">Content 3</div>
  </div>

  <div class="collapse-item">
      <a class="collapse-toggle">
          <span>Section 3</span>
          <span class="collapse-indicator">
              <svg class="collapse-icon" width="1em" height="1em" viewBox="0 0 20 20" fill="none" aria-hidden="true" focusable="false">
                  <path d="M7 5l5 5-5 5" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
          </span>
      </a>
      <div class="collapse-content">Content 3</div>
  </div>
</div>
```

To restrict only one open content at a time, declare <code>data-collapse="accordion"</code>.

```html
<div class="collapsible" data-collapse="accordion">
```

---