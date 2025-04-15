# Notifications Component

A flexible notification system with multiple positions, animations, and status variants.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Notification background
- `--color-text-primary`: Title text
- `--color-text-secondary`: Message text
- `--color-text-muted`: Close button color
- `--color-accent`: Progress bar color
- `--color-success`: Success variant
- `--color-error`: Error variant
- `--color-warning`: Warning variant
- `--color-info`: Info variant
- `--border-radius-md`: Notification corners
- `--font-size-sm`: Message text size
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Container gap
- `--spacing-md`: Container padding
- `--shadow-lg`: Notification shadow
- `--z-toast`: Stack order
- `--transition-fast`: Button animations
- `--animation-smooth`: Enter/exit timing

## Classes

### Container Classes
- `.notifications-container`: Main wrapper
- `.notifications-container--top-right`: Top right position
- `.notifications-container--top-left`: Top left position
- `.notifications-container--bottom-right`: Bottom right position
- `.notifications-container--bottom-left`: Bottom left position

### Notification Classes
- `.notification`: Individual notification
- `.notification__icon`: Status icon
- `.notification__content`: Text wrapper
- `.notification__title`: Notification title
- `.notification__message`: Notification text
- `.notification__close`: Close button
- `.notification__progress`: Timer bar

### Animation Variants
- `.notification--slide-right`: Slide from right
- `.notification--slide-left`: Slide from left
- `.notification--fade`: Fade and scale
- `.notification--closing`: Exit animation

### Status Variants
- `.notification--success`: Success message
- `.notification--error`: Error message
- `.notification--warning`: Warning message
- `.notification--info`: Info message

## Usage Example

```html
<div class="notifications-container notifications-container--top-right">
  <!-- Success Notification -->
  <div class="notification notification--success notification--slide-right">
    <svg class="notification__icon"><!-- success icon --></svg>
    <div class="notification__content">
      <div class="notification__title">Success</div>
      <div class="notification__message">Operation completed successfully!</div>
    </div>
    <button class="notification__close">×</button>
    <div class="notification__progress notification__progress--animated"></div>
  </div>

  <!-- Error Notification -->
  <div class="notification notification--error notification--slide-right">
    <svg class="notification__icon"><!-- error icon --></svg>
    <div class="notification__content">
      <div class="notification__title">Error</div>
      <div class="notification__message">Something went wrong!</div>
    </div>
    <button class="notification__close">×</button>
  </div>
</div>
```

## Features
- Multiple positions
- Animation options
- Auto-dismiss timer
- Progress indicator
- Status variants
- Close button
- Icon support
- Stacked layout
- Smooth transitions
- Responsive design

## Animations
- Slide right/left
- Fade with scale
- Progress bar
- Close transitions
- Smooth stacking

## Best Practices
- Clear messages
- Appropriate timing
- Consistent positioning
- Status indication
- Progress feedback
- Easy dismissal
- Stack management
- Animation performance
- Touch consideration
- Screen reader support

## Position Options
- Top right
- Top left
- Bottom right
- Bottom left
- Proper stacking
- Gap management