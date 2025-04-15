# Badge Component

A lightweight component for status indicators, labels, and counters.

## Variables Used

### Core Variables Used
- `--color-bg-tertiary`: Default background color
- `--color-text-primary`: Default text color
- `--color-bg-primary`: Text color for primary variant
- `--color-accent`: Background for primary variant
- `--border-radius-sm`: Default border radius
- `--spacing-xs`: Spacing for icon gap

### Status Colors
- Primary: Uses `--color-accent`
- Success: `#4caf50`
- Warning: `#ff9800`
- Error: `#ff4d4d`

## Classes

### Base Class
- `.badge`: Main container with base styles

### Variants
- `.badge--primary`: Primary themed badge
- `.badge--success`: Success themed badge
- `.badge--warning`: Warning themed badge
- `.badge--error`: Error themed badge

### Modifiers
- `.badge--outline`: Outlined style with transparent background
- `.badge--rounded`: Fully rounded corners
- `.badge--icon`: Support for icons with proper spacing

## Usage Example

```html
<!-- Basic Badge -->
<span class="badge">Default</span>

<!-- Variant Badges -->
<span class="badge badge--primary">Primary</span>
<span class="badge badge--success">Success</span>
<span class="badge badge--warning">Warning</span>
<span class="badge badge--error">Error</span>

<!-- Outlined Badge -->
<span class="badge badge--outline">Outlined</span>

<!-- Rounded Badge -->
<span class="badge badge--rounded">Rounded</span>

<!-- Badge with Icon -->
<span class="badge badge--icon">
  <svg><!-- icon svg --></svg>
  With Icon
</span>
```

## Features
- Multiple semantic variants (primary, success, warning, error)
- Outline style option
- Rounded corners variant
- Icon support with proper spacing
- Consistent sizing and padding
- Flexible display with inline-flex
- Proper text alignment and centering