# Customization Guide

Lightpack is built with customization in mind. Every aspect of the framework can be tailored to match your brand and design requirements using CSS variables, utility classes, and component overrides.

---

## CSS Variables (Design Tokens)

Lightpack uses CSS custom properties (variables) for all design tokens. This means you can customize the entire framework by simply overriding these variables.

**In your CSS file**
```css
:root {
  --color-primary: #6366f1;
  --font-family: 'Inter', sans-serif;
  --radius-md: 8px;
}
```

---

## Customizing Colors

### Brand Colors

Override the primary and secondary colors to match your brand:

```css
:root {
  /* Primary brand color */
  --color-primary: #6366f1;
  --color-primary-light: #818cf8;
  --color-primary-lighter: #a5b4fc;
  --color-primary-dark: #4f46e5;
  
  /* Secondary brand color */
  --color-secondary: #8b5cf6;
  --color-secondary-light: #a78bfa;
  --color-secondary-lighter: #c4b5fd;
  --color-secondary-dark: #7c3aed;
}
```

**Example:**
```html
<button class="btn btn-primary">Branded Button</button>
```

### Semantic Colors

Customize feedback colors for your application:

```css
:root {
  /* Success - green by default */
  --color-success: #10b981;
  --color-success-light: #34d399;
  --color-success-lighter: #6ee7b7;
  --color-success-dark: #059669;
  
  /* Danger - red by default */
  --color-danger: #ef4444;
  --color-danger-light: #f87171;
  --color-danger-lighter: #fca5a5;
  --color-danger-dark: #dc2626;
  
  /* Warning - yellow/orange by default */
  --color-warning: #f59e0b;
  --color-warning-light: #fbbf24;
  --color-warning-lighter: #fcd34d;
  --color-warning-dark: #d97706;
  
  /* Info - blue by default */
  --color-info: #3b82f6;
  --color-info-light: #60a5fa;
  --color-info-lighter: #93c5fd;
  --color-info-dark: #2563eb;
}
```

### Surface & Background Colors

Control the overall look and feel:

```css
:root {
  --color-background: #ffffff;
  --color-surface: #f9fafb;
  --color-surface-dark: #f3f4f6;
  --color-surface-alt: #e5e7eb;
  --color-border: #d1d5db;
  --color-border-dark: #9ca3af;
}
```

### Text Colors

```css
:root {
  --color-text: #1f2937;
  --color-text-muted: #6b7280;
  --color-text-inverse: #ffffff;
}
```

### Complete Brand Example

```css
/* Acme Corp Brand */
:root {
  --color-primary: #ff6b35;
  --color-primary-light: #ff8c61;
  --color-primary-lighter: #ffad8d;
  --color-primary-dark: #e55a2b;
  
  --color-secondary: #004e89;
  --color-secondary-light: #1a6ba8;
  --color-secondary-lighter: #3388c7;
  --color-secondary-dark: #003a6a;
  
  --font-family: 'Poppins', sans-serif;
  --radius-md: 12px;
}
```

---

## Customizing Typography

### Font Families

```css
:root {
  /* Main font stack */
  --font-family-sans: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  --font-family-serif: 'Merriweather', Georgia, serif;
  --font-family-mono: 'Fira Code', 'Courier New', monospace;
  --font-family: var(--font-family-sans);
}
```

**Example: Using Google Fonts**
```html
<head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --font-family: 'Inter', sans-serif;
    }
  </style>
</head>
```

### Font Sizes

Create your own type scale:

```css
:root {
  --fs-xs: 0.75rem;    /* 12px */
  --fs-sm: 0.875rem;   /* 14px */
  --fs-base: 1rem;     /* 16px */
  --fs-md: 1.125rem;   /* 18px */
  --fs-lg: 1.25rem;    /* 20px */
  --fs-xl: 1.5rem;     /* 24px */
  --fs-2xl: 1.875rem;  /* 30px */
  --fs-3xl: 2.25rem;   /* 36px */
  --fs-4xl: 3rem;      /* 48px */
  --fs-5xl: 3.75rem;   /* 60px */
}
```

**Larger Type Scale Example:**
```css
:root {
  --fs-base: 1.125rem;  /* 18px base instead of 16px */
  --fs-xl: 1.75rem;     /* 28px */
  --fs-2xl: 2.25rem;    /* 36px */
  --fs-3xl: 3rem;       /* 48px */
  --fs-4xl: 4rem;       /* 64px */
  --fs-5xl: 5rem;       /* 80px */
}
```

### Line Heights

```css
:root {
  --line-height-tight: 1.25;
  --line-height-snug: 1.375;
  --line-height-normal: 1.5;
  --line-height-relaxed: 1.625;
  --line-height-loose: 2;
}
```

### Letter Spacing

```css
:root {
  --letter-spacing-tighter: -0.05em;
  --letter-spacing-tight: -0.025em;
  --letter-spacing-normal: 0;
  --letter-spacing-wide: 0.025em;
  --letter-spacing-wider: 0.05em;
  --letter-spacing-widest: 0.1em;
}
```

---

## Customizing Spacing

### Gap Scale

Lightpack uses a consistent spacing scale (`--g-1` through `--g-9`):

```css
:root {
  --g-1: 0.25rem;  /* 4px */
  --g-2: 0.5rem;   /* 8px */
  --g-3: 1rem;     /* 16px */
  --g-4: 1.5rem;   /* 24px */
  --g-5: 2rem;     /* 32px */
  --g-6: 3rem;     /* 48px */
  --g-7: 4rem;     /* 64px */
  --g-8: 6rem;     /* 96px */
  --g-9: 8rem;     /* 128px */
}
```

**Custom Spacing Scale:**
```css
/* Tighter spacing */
:root {
  --g-1: 0.125rem;  /* 2px */
  --g-2: 0.25rem;   /* 4px */
  --g-3: 0.5rem;    /* 8px */
  --g-4: 1rem;      /* 16px */
  --g-5: 1.5rem;    /* 24px */
  --g-6: 2rem;      /* 32px */
  --g-7: 3rem;      /* 48px */
  --g-8: 4rem;      /* 64px */
  --g-9: 6rem;      /* 96px */
}
```

---

## Customizing Components

Components don't have their own CSS variables - they use the global design tokens. Customize by overriding component classes directly.

### Example

```css
/* Override button styles */
.btn {
  padding: 0.75rem 1.5rem;
  font-weight: var(--fw-600);
  border-radius: var(--radius-lg);
  text-transform: uppercase;
  letter-spacing: var(--letter-spacing-wide);
}

/* Custom button variant */
.btn-brand {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  border: none;
  box-shadow: var(--shadow-md);
  transition: all var(--transition-base) var(--easing-base);
}

.btn-brand:hover {
  box-shadow: var(--shadow-lg);
  transform: translateY(-2px);
}
```

---

## Creating Custom Themes

### Light & Dark Theme

```css
/* Light theme (default) */
:root {
  --color-background: #ffffff;
  --color-surface: #f9fafb;
  --color-text: #1f2937;
  --color-border: #e5e7eb;
}

/* Dark theme */
.theme-dark {
  --color-background: #111827;
  --color-surface: #1f2937;
  --color-surface-dark: #374151;
  --color-text: #f9fafb;
  --color-text-muted: #9ca3af;
  --color-border: #374151;
  --color-border-dark: #4b5563;
  
  /* Adjust semantic colors for dark mode */
  --color-primary: #818cf8;
  --color-success: #34d399;
  --color-danger: #f87171;
  --color-warning: #fbbf24;
}
```

### Custom Brand Theme

```css
/* Acme Corp Theme */
.theme-acme {
  /* Brand colors - using Lightpack's color palette */
  --color-primary: var(--orange);
  --color-primary-light: var(--orange-light);
  --color-primary-dark: var(--orange-dark);
  
  --color-secondary: var(--blue);
  --color-secondary-light: var(--blue-light);
  --color-secondary-dark: var(--blue-dark);
  
  --color-accent: var(--indigo);
  --color-accent-light: var(--indigo-light);
  --color-accent-dark: var(--indigo-dark);
  
  /* Surfaces */
  --color-background: var(--orange-lighter);
  --color-surface: var(--white);
  --color-border: var(--orange-light);
  
  /* Typography */
  --font-family: 'Poppins', sans-serif;
  
  /* Spacing */
  --radius-md: 12px;
  --radius-lg: 16px;
}
```

**Usage:**
```html
<body class="theme-acme">
  <!-- Your content -->
</body>
```

### High Contrast Theme

```css
.theme-high-contrast {
  --color-background: #000000;
  --color-surface: #1a1a1a;
  --color-text: #ffffff;
  --color-border: #ffffff;
  
  --color-primary: #00d4ff;
  --color-success: #00ff00;
  --color-danger: #ff0000;
  --color-warning: #ffff00;
}
```

---

## Complete Customization Example

```css
/* custom-theme.css */

/* 1. Brand Colors - Use Lightpack's color palette */
:root {
  --color-primary: var(--indigo);
  --color-primary-light: var(--indigo-light);
  --color-primary-lighter: var(--indigo-lighter);
  --color-primary-dark: var(--indigo-dark);
  
  --color-secondary: var(--pink);
  --color-secondary-light: var(--pink-light);
  --color-secondary-lighter: var(--pink-lighter);
  --color-secondary-dark: var(--pink-dark);
}

/* 2. Typography */
:root {
  --font-family: 'Inter', sans-serif;
  --fs-base: 1.125rem;
}

/* 3. Spacing & Layout */
:root {
  --radius-md: 12px;
  --radius-lg: 16px;
  --g-4: 2rem;
}

/* 4. Component Overrides */
.btn {
  text-transform: uppercase;
  letter-spacing: var(--letter-spacing-wide);
  font-weight: var(--fw-600);
}

.card {
  border-radius: var(--radius-lg);
  box-shadow: var(--shadow-md);
  transition: all var(--transition-base) var(--easing-base);
}

.card:hover {
  box-shadow: var(--shadow-lg);
  transform: translateY(-2px);
}

/* 5. Custom Utilities */
.gradient-text {
  background: linear-gradient(135deg, var(--color-primary), var(--color-secondary));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.glass-effect {
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
}
```

**Usage:**
```html
<head>
  <link rel="stylesheet" href="lightpack.min.css">
  <link rel="stylesheet" href="custom-theme.css">
</head>
```

---

## Tips & Best Practices

### ✅ Do's

1. **Use CSS variables** for easy theming
2. **Override at the :root level** for global changes
3. **Scope overrides** to specific sections when needed
4. **Test in dark mode** if you support it
5. **Maintain consistency** with your design system

### ❌ Don'ts

1. **Don't modify the source CSS** - override instead
2. **Don't use !important** unless absolutely necessary
3. **Don't break responsive behavior** when customizing
4. **Don't forget accessibility** (contrast, focus states)
5. **Don't override utility classes** - create new ones instead

---

## Need Help?

- Check [Variables Reference](variables.md) for all available CSS variables
- See [Utilities](utilities.md) for extending with utility classes
- Review [Theming Guide](theming.md) for dark mode customization
- Browse component docs for component-specific customization options
