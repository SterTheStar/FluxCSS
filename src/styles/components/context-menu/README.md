# Context Menu Component

A customizable right-click menu component with support for submenus, icons, and various states.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Menu background
- `--color-bg-tertiary`: Hover background and dividers
- `--color-text-primary`: Item text color
- `--border-radius-md`: Menu container radius
- `--spacing-xs`: Vertical padding and divider margin
- `--spacing-sm`: Item padding and icon gap
- `--spacing-md`: Horizontal item padding
- `--shadow-lg`: Menu shadow
- `--transition-fast`: Show/hide and hover animations

## Classes

### Base Classes
- `.context-menu`: Main container
- `.context-menu__item`: Menu item
- `.context-menu__item-icon`: Item icon
- `.context-menu__divider`: Separator line
- `.context-menu__submenu`: Nested menu container

### States and Variants
- `.is-active`: Visible state
- `.context-menu__item--disabled`: Disabled item
- `.context-menu__item--danger`: Destructive action
- `.context-menu__item--has-submenu`: Item with submenu

## Usage Example

```html
<div class="context-menu">
  <!-- Basic Item -->
  <div class="context-menu__item">
    <svg class="context-menu__item-icon"><!-- icon svg --></svg>
    Edit
  </div>

  <!-- Divider -->
  <div class="context-menu__divider"></div>

  <!-- Disabled Item -->
  <div class="context-menu__item context-menu__item--disabled">
    <svg class="context-menu__item-icon"><!-- icon svg --></svg>
    Share
  </div>

  <!-- Danger Item -->
  <div class="context-menu__item context-menu__item--danger">
    <svg class="context-menu__item-icon"><!-- icon svg --></svg>
    Delete
  </div>

  <!-- Item with Submenu -->
  <div class="context-menu__item context-menu__item--has-submenu">
    More Options
    <div class="context-menu__submenu">
      <!-- Submenu items -->
      <div class="context-menu__item">Option 1</div>
      <div class="context-menu__item">Option 2</div>
    </div>
  </div>
</div>
```

## Features
- Right-click activation
- Nested submenus
- Icon support
- Divider elements
- Disabled state
- Danger actions
- Smooth animations
- Keyboard navigation
- Position auto-adjustment
- User selection prevention

## Interactions
- Shows on right-click
- Hides on outside click
- Submenu on hover
- Hover highlighting
- Disabled item handling

## Animations
- Scale and fade in/out
- Smooth hover transitions
- Submenu slide effect

## Best Practices
- Keep menus concise
- Group related items
- Use clear icons
- Include keyboard shortcuts
- Provide visual feedback
- Handle edge positions
- Support keyboard navigation
- Ensure proper focus management