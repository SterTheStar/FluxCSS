# Tabs Component

A flexible tabbed interface with multiple layout variants and styles.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Pill text color
- `--color-bg-tertiary`: Border color
- `--color-text-primary`: Hover text
- `--color-text-secondary`: Default text
- `--color-accent`: Active state
- `--border-radius-sm`: Pill corners
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Button padding
- `--spacing-md`: Section padding
- `--transition-fast`: Hover effects

## Classes

### Base Classes
- `.tabs`: Main container
- `.tabs__list`: Tab buttons wrapper
- `.tabs__button`: Individual tab
- `.tabs__content`: Panels container
- `.tabs__panel`: Content panel

### States
- `.tabs__button--active`: Selected tab
- `.tabs__panel--active`: Visible panel

### Layout Variants
- `.tabs--vertical`: Side navigation
- `.tabs--pills`: Rounded buttons

## Usage Example

```html
<!-- Standard Tabs -->
<div class="tabs">
  <div class="tabs__list" role="tablist">
    <button class="tabs__button tabs__button--active" role="tab">Tab 1</button>
    <button class="tabs__button" role="tab">Tab 2</button>
  </div>
  
  <div class="tabs__content">
    <div class="tabs__panel tabs__panel--active" role="tabpanel">
      Content 1
    </div>
    <div class="tabs__panel" role="tabpanel">
      Content 2
    </div>
  </div>
</div>

<!-- Vertical Tabs -->
<div class="tabs tabs--vertical">
  <!-- Same structure as above -->
</div>

<!-- Pill Tabs -->
<div class="tabs tabs--pills">
  <!-- Same structure as above -->
</div>
```

## Features
- Multiple layouts
- Active state indicators
- Hover effects
- Content panels
- Smooth transitions
- Accessible markup
- Clean aesthetics
- Flexible styling
- Easy implementation

## Layout Options
- Horizontal (default)
- Vertical navigation
- Pill-style buttons
- Flexible sizing
- Consistent spacing

## Best Practices
- Use semantic markup
- Include ARIA roles
- Handle keyboard nav
- Clear active states
- Consistent spacing
- Meaningful labels
- Content organization
- Mobile consideration
- Transition handling
- Focus management