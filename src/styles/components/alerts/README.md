# Alert Component

The Alert component provides contextual feedback messages for typical user actions with support for multiple types of alerts.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Base background color
- `--color-text-secondary`: Text color for alert messages
- `--border-radius-md`: Border radius for the alert container
- `--spacing-xs`: Small spacing for title margin
- `--spacing-sm`: Spacing for close button positioning
- `--spacing-md`: Padding and margin for the alert container
- `--transition-fast`: Animation speed for hover effects
- `--color-accent`: Color for info variant

### Status Colors
- Info: `var(--color-accent)`
- Success: `#4caf50`
- Warning: `#ff9800`
- Error: `#ff4d4d`

## Classes

### Base Classes
- `.alert`: Main container
- `.alert__title`: Alert heading
- `.alert__message`: Alert content text
- `.alert__close`: Close button

### Variants
- `.alert--info`: Information style alert
- `.alert--success`: Success style alert
- `.alert--warning`: Warning style alert
- `.alert--error`: Error style alert
- `.alert--icon`: Adds an icon to the alert

## Usage Example

```html
<!-- Basic Alert -->
<div class="alert">
  <div class="alert__title">Alert Title</div>
  <div class="alert__message">Alert content goes here</div>
</div>

<!-- Alert with Icon -->
<div class="alert alert--success alert--icon">
  Success message with icon
</div>

<!-- Alert with Close Button -->
<div class="alert alert--warning">
  <button class="alert__close">×</button>
  Warning message with close button
</div>
```

## Features
- Four contextual variations (info, success, warning, error)
- Optional icons for each variant
- Support for titles and messages
- Closeable alerts
- Left border accent
- Semi-transparent background that matches the theme