# Toast Component

A notification system for temporary messages with status variants and positioning options.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Toast background
- `--color-text-primary`: Title text
- `--color-text-secondary`: Message text
- `--color-text-muted`: Close button
- `--color-accent`: Info variant/progress
- `--border-radius-md`: Toast corners
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Item spacing
- `--spacing-md`: Container padding
- `--shadow-lg`: Toast shadow
- `--transition-fast`: Button animation

## Classes

### Container Classes
- `.toast-container`: Position wrapper
- `.toast-container--top-right`: Top right position
- `.toast-container--top-left`: Top left position
- `.toast-container--bottom-right`: Bottom right position
- `.toast-container--bottom-left`: Bottom left position

### Toast Classes
- `.toast`: Individual message
- `.toast__icon`: Status icon
- `.toast__content`: Text wrapper
- `.toast__title`: Message title
- `.toast__message`: Message text
- `.toast__close`: Close button
- `.toast__progress`: Timer bar

### Status Variants
- `.toast--success`: Success message
- `.toast--error`: Error message
- `.toast--warning`: Warning message
- `.toast--info`: Info message
- `.toast--progress`: With progress bar
- `.toast--closing`: Exit animation

## Usage Example

```html
<div class="toast-container toast-container--top-right">
  <!-- Success Toast -->
  <div class="toast toast--success">
    <svg class="toast__icon"><!-- success icon --></svg>
    <div class="toast__content">
      <div class="toast__title">Success</div>
      <div class="toast__message">Operation completed successfully!</div>
    </div>
    <button class="toast__close">×</button>
    <div class="toast__progress"></div>
  </div>

  <!-- Error Toast -->
  <div class="toast toast--error">
    <svg class="toast__icon"><!-- error icon --></svg>
    <div class="toast__content">
      <div class="toast__title">Error</div>
      <div class="toast__message">Something went wrong!</div>
    </div>
    <button class="toast__close">×</button>
  </div>
</div>
```

## Features
- Multiple positions
- Status variants
- Auto-dismiss
- Progress indicator
- Close button
- Smooth animations
- Stack management
- Icon support
- Clean design

## Animations
- Slide in/out
- Progress bar
- Close transitions
- Stack reflow
- 0.3s duration
- Smooth timing

## Best Practices
- Clear messages
- Appropriate timing
- Consistent position
- Status indication
- Progress feedback
- Easy dismissal
- Stack handling
- Animation performance
- Screen reader support
- Touch consideration