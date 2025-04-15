# Skeletons Component

A collection of animated loading placeholder components for various content types and layouts.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Container background
- `--color-bg-tertiary`: Skeleton background
- `--border-radius-sm`: Default corners
- `--border-radius-md`: Card and thumbnail radius
- `--spacing-sm`: Small padding
- `--spacing-md`: Default gaps

## Classes

### Base Classes
- `.skeleton`: Base skeleton style
- `.skeleton-text`: Text line placeholder
- `.skeleton-circle`: Circular placeholder
- `.skeleton-avatar`: Profile picture placeholder
- `.skeleton-thumbnail`: Image placeholder

### Layout Classes
#### Card Layout
- `.skeleton-card`: Card container
- `.skeleton-card__header`: Card top section
- `.skeleton-card__content`: Card body area

#### Table Layout
- `.skeleton-table`: Table container
- `.skeleton-table__row`: Table row
- `.skeleton-table__cell`: Table cell

#### List Layout
- `.skeleton-list`: List container
- `.skeleton-list__item`: List row
- `.skeleton-list__content`: List item content

#### Grid Layout
- `.skeleton-grid`: Auto-fill grid layout

## Usage Example

```html
<!-- Text Lines -->
<div class="skeleton-text"></div>
<div class="skeleton-text"></div>
<div class="skeleton-text"></div>

<!-- Card Loading -->
<div class="skeleton-card">
  <div class="skeleton-card__header">
    <div class="skeleton-avatar"></div>
    <div class="skeleton-text"></div>
  </div>
  <div class="skeleton-card__content">
    <div class="skeleton-text"></div>
    <div class="skeleton-text"></div>
    <div class="skeleton-text"></div>
  </div>
</div>

<!-- List Loading -->
<div class="skeleton-list">
  <div class="skeleton-list__item">
    <div class="skeleton-avatar"></div>
    <div class="skeleton-list__content">
      <div class="skeleton-text"></div>
      <div class="skeleton-text"></div>
    </div>
  </div>
</div>

<!-- Grid Loading -->
<div class="skeleton-grid">
  <div class="skeleton-card">
    <div class="skeleton-thumbnail"></div>
    <div class="skeleton-text"></div>
  </div>
</div>
```

## Features
- Wave animation effect
- Multiple layout options
- Content type variants
- Responsive grid
- Customizable sizes
- Clean aesthetics
- Low-effort implementation
- Performance optimized
- Consistent spacing
- Proper content hints

## Layout Options
- Card layouts
- List views
- Table rows
- Grid systems
- Flexible sizing
- Responsive design

## Animation
- Smooth wave effect
- Continuous animation
- 1.5s duration
- Gradient overlay
- Performance optimized
- Subtle indication

## Best Practices
- Match content structure
- Use appropriate sizes
- Maintain spacing
- Keep animations subtle
- Consider performance
- Provide visual hierarchy
- Indicate content type
- Ensure accessibility
- Handle transitions
- Maintain consistency