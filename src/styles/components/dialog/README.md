# Dialog Component

A flexible modal dialog component with multiple variants, animations, and positioning options.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Close button text color
- `--color-bg-secondary`: Dialog background
- `--color-bg-tertiary`: Borders and close button
- `--color-text-primary`: Title text color
- `--color-text-secondary`: Close button color
- `--color-accent`: Close button hover
- `--border-radius-lg`: Dialog container radius
- `--border-radius-full`: Close button radius
- `--font-size-xl`: Dialog title size
- `--spacing-sm`: Button gap
- `--spacing-md`: Backdrop padding
- `--spacing-lg`: Section padding
- `--shadow-lg`: Dialog shadow
- `--z-modal`: Stack order
- `--transition-normal`: Show/hide animations
- `--transition-fast`: Button animations
- `--animation-smooth`: Backdrop timing
- `--animation-bounce`: Dialog timing

## Classes

### Base Classes
- `.dialog-backdrop`: Overlay background
- `.dialog`: Main container
- `.dialog__header`: Title section
- `.dialog__title`: Dialog title
- `.dialog__close`: Close button
- `.dialog__content`: Main content area
- `.dialog__footer`: Actions section

### Size Variants
- `.dialog--sm`: Small dialog (400px)
- `.dialog--lg`: Large dialog (800px)
- `.dialog--xl`: Extra large dialog (1140px)
- `.dialog--fullscreen`: Full viewport size

### Position Variants
- `.dialog--top`: Appears from top
- `.dialog--bottom`: Appears from bottom

### States
- `.is-active`: Visible state
- `.dialog--loading`: Loading state

## Usage Example

```html
<div class="dialog-backdrop">
  <div class="dialog">
    <!-- Header -->
    <div class="dialog__header">
      <h2 class="dialog__title">Dialog Title</h2>
      <button class="dialog__close">×</button>
    </div>
    
    <!-- Content -->
    <div class="dialog__content">
      Dialog content goes here...
    </div>
    
    <!-- Footer -->
    <div class="dialog__footer">
      <button class="btn">Cancel</button>
      <button class="btn btn--primary">Confirm</button>
    </div>
  </div>
</div>
```

## Features
- Backdrop with click-away
- Custom scrollbar styling
- Multiple size options
- Position variants
- Loading state
- Smooth animations
- Responsive design
- Focus trapping
- Keyboard navigation
- Scroll lock
- Custom scroll area

## Animations
- Fade in/out backdrop
- Scale and slide transitions
- Bounce effect on entry
- Smooth button interactions

## Responsive Behavior
- Maximum height constraint
- Mobile-friendly padding
- Scrollable content area
- Fullscreen option
- Maintains readable width

## Best Practices
- Use clear, concise titles
- Include close button
- Provide action buttons
- Handle loading states
- Maintain focus management
- Enable keyboard navigation
- Prevent background scroll
- Consider mobile viewports
- Implement ARIA attributes
- Handle edge cases