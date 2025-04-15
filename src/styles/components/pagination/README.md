# Pagination Component

A flexible pagination system with multiple styles, sizes, and responsive behavior.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Active item text color
- `--color-bg-tertiary`: Hover background and borders
- `--color-text-primary`: Hover text color
- `--color-text-secondary`: Default text color
- `--color-accent`: Active item background
- `--border-radius-sm`: Default corners
- `--border-radius-full`: Rounded variant
- `--font-size-sm`: Small size text
- `--font-size-lg`: Large size text
- `--spacing-xs`: Item gaps
- `--spacing-sm`: Horizontal padding
- `--transition-fast`: Hover animations

## Classes

### Base Classes
- `.pagination`: Container
- `.pagination__item`: Page number/control
- `.pagination__icon`: Navigation icons

### States
- `.pagination__item--active`: Current page
- `.pagination__item--disabled`: Disabled control
- `.pagination__item--prev`: Previous button
- `.pagination__item--next`: Next button
- `.pagination__item--dots`: Ellipsis

### Variants
- `.pagination--rounded`: Circular buttons
- `.pagination--bordered`: Outlined style
- `.pagination--responsive`: Mobile-friendly

### Sizes
- `.pagination--sm`: Small size
- `.pagination--lg`: Large size

## Usage Example

```html
<nav class="pagination pagination--bordered">
  <!-- Previous -->
  <a href="#" class="pagination__item pagination__item--prev">
    <svg class="pagination__icon"><!-- prev icon --></svg>
  </a>

  <!-- Numbers -->
  <a href="#" class="pagination__item">1</a>
  <a href="#" class="pagination__item pagination__item--active">2</a>
  <a href="#" class="pagination__item">3</a>
  <span class="pagination__item pagination__item--dots">...</span>
  <a href="#" class="pagination__item">10</a>

  <!-- Next -->
  <a href="#" class="pagination__item pagination__item--next">
    <svg class="pagination__icon"><!-- next icon --></svg>
  </a>
</nav>
```

## Features
- Multiple style variants
- Three size options
- Responsive design
- Icon support
- Disabled states
- Active page indicator
- Hover effects
- Touch-friendly targets
- Keyboard navigation
- Screen reader support

## Size Options
- Default: 2.5rem
- Small: 2rem
- Large: 3rem

## Responsive Behavior
- Shows only active page on mobile
- Maintains prev/next controls
- Keeps ellipsis visible
- Adapts to screen size
- Preserves functionality

## Best Practices
- Clear active state
- Consistent spacing
- Adequate touch targets
- Keyboard accessibility
- Logical navigation
- Visual feedback
- Screen reader labels
- Proper HTML semantics
- Simple mobile view
- Loading state handling