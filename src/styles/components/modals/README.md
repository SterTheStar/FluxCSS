# Modal Component

A flexible modal dialog system with backdrop, multiple sizes, and fullscreen option.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Modal background
- `--color-bg-tertiary`: Border color
- `--color-text-primary`: Title color
- `--color-text-muted`: Close button color
- `--border-radius-lg`: Modal corners
- `--spacing-xs`: Close button padding
- `--spacing-sm`: Footer gap
- `--spacing-md`: Section padding
- `--shadow-lg`: Modal shadow
- `--transition-normal`: Show/hide animations
- `--transition-fast`: Button animations

## Classes

### Base Classes
- `.modal-backdrop`: Overlay background
- `.modal`: Main container
- `.modal__header`: Title section
- `.modal__title`: Modal title
- `.modal__close`: Close button
- `.modal__body`: Content area
- `.modal__footer`: Actions area

### Size Variants
- `.modal--sm`: Small (300px)
- `.modal--lg`: Large (800px)
- `.modal--xl`: Extra large (1140px)
- `.modal--fullscreen`: Full viewport

### States
- `.is-active`: Visible state

## Usage Example

```html
<div class="modal-backdrop">
  <div class="modal">
    <!-- Header -->
    <div class="modal__header">
      <h2 class="modal__title">Modal Title</h2>
      <button class="modal__close">×</button>
    </div>

    <!-- Body -->
    <div class="modal__body">
      Modal content goes here...
    </div>

    <!-- Footer -->
    <div class="modal__footer">
      <button class="btn">Cancel</button>
      <button class="btn btn--primary">Confirm</button>
    </div>
  </div>
</div>
```

## Features
- Darkened backdrop
- Multiple size options
- Fullscreen mode
- Header with close button
- Scrollable content area
- Action footer
- Smooth animations
- Responsive design
- Focus trapping
- Keyboard navigation

## Animations
- Fade in/out backdrop
- Slide up/down modal
- Button hover effects
- Smooth transitions

## Best Practices
- Clear titles
- Close button
- Action buttons
- Scroll overflow
- Focus management
- Keyboard support
- Click outside
- ESC to close
- Prevent background scroll
- Mobile considerations

## Responsive Behavior
- Maximum width constraint
- Viewport height limit
- Mobile padding
- Touch-friendly targets
- Fullscreen option