# Dropdown Component

A versatile dropdown menu component with multiple positioning options, animations, and states.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Menu background
- `--color-bg-tertiary`: Hover background
- `--color-text-primary`: Active item text
- `--color-text-secondary`: Default item text
- `--color-text-muted`: Group header text
- `--color-accent`: Active item color
- `--border-radius-md`: Menu border radius
- `--font-size-sm`: Small text size
- `--spacing-xs`: Small gaps and margins
- `--spacing-sm`: Default item gap
- `--spacing-md`: Item padding
- `--shadow-lg`: Menu shadow
- `--z-dropdown`: Stack order
- `--transition-normal`: Show/hide animations
- `--transition-fast`: Item hover animations

## Classes

### Base Classes
- `.dropdown`: Main container
- `.dropdown__trigger`: Click target
- `.dropdown__menu`: Menu container
- `.dropdown__item`: Menu item
- `.dropdown__divider`: Separator line
- `.dropdown__icon`: Item icon
- `.dropdown__arrow`: Trigger arrow icon

### Position Variants
- `.dropdown__menu--right`: Right-aligned menu
- `.dropdown__menu--top`: Opens upward

### Animation Variants
- `.dropdown__menu--fade`: Fade animation
- `.dropdown__menu--scale`: Scale animation

### States
- `.is-active`: Visible state
- `.dropdown__item--active`: Selected item
- `.dropdown__item--disabled`: Disabled item

### Groups
- `.dropdown__group`: Item group
- `.dropdown__group-header`: Group title

## Usage Example

```html
<div class="dropdown">
  <!-- Trigger -->
  <button class="dropdown__trigger">
    Dropdown
    <svg class="dropdown__arrow"><!-- arrow icon --></svg>
  </button>

  <!-- Menu -->
  <div class="dropdown__menu">
    <!-- Group -->
    <div class="dropdown__group">
      <div class="dropdown__group-header">Group Title</div>
      
      <!-- Items -->
      <a class="dropdown__item">
        <svg class="dropdown__icon"><!-- icon --></svg>
        Regular Item
      </a>
      
      <a class="dropdown__item dropdown__item--active">
        Active Item
      </a>
      
      <div class="dropdown__divider"></div>
      
      <a class="dropdown__item dropdown__item--disabled">
        Disabled Item
      </a>
    </div>
  </div>
</div>
```

## Features
- Multiple positioning options
- Customizable animations
- Icon support
- Grouped items
- Active states
- Disabled states
- Divider elements
- Arrow indicator
- Smooth transitions
- Keyboard navigation
- Click-away handling

## Animations
- Fade in/out option
- Scale animation option
- Slide transform default
- Arrow rotation
- Hover transitions

## Best Practices
- Use clear labels
- Group related items
- Include visual feedback
- Support keyboard navigation
- Handle edge positions
- Consider mobile interaction
- Maintain accessibility
- Use consistent icons
- Implement proper focus
- Handle overflow cases

## Responsive Behavior
- Handles edge detection
- Maintains readability
- Preserves touch targets
- Adapts to viewport
- Mobile-friendly interactions