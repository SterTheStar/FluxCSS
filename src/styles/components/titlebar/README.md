# Titlebar Component

A versatile titlebar component with native window controls and multiple style variants.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Text color
- `--color-bg-secondary`: Default background
- `--color-bg-tertiary`: Border color
- `--color-text-primary`: Title color
- `--color-text-secondary`: Subtitle color
- `--color-accent`: Primary variant
- `--font-size-sm`: Subtitle size
- `--font-size-md`: Title size
- `--spacing-sm`: Small gap
- `--spacing-md`: Default padding
- `--spacing-lg`: Large padding
- `--spacing-xl`: Extra padding
- `--shadow-sm`: Shadow variant
- `--transition-normal`: Animations
- `--animation-smooth`: Entry timing

## Classes

### Base Classes
- `.titlebar`: Main container
- `.titlebar__title`: Main heading
- `.titlebar__content`: Title wrapper
- `.titlebar__subtitle`: Secondary text
- `.titlebar__actions`: Right side items
- `.titlebar__icon`: Title icon

### Window Controls
- `.titlebar__window-controls`: Controls wrapper
- `.titlebar__window-button`: Control button
- `.titlebar__window-button--close`: Close button
- `.titlebar__window-button--minimize`: Minimize button
- `.titlebar__window-button--maximize`: Maximize button

### Style Variants
- `.titlebar--primary`: Accent colored
- `.titlebar--glass`: Frosted glass effect
- `.titlebar--bordered`: Full border
- `.titlebar--shadow`: Drop shadow
- `.titlebar--macos`: macOS controls
- `.titlebar--windows`: Windows controls

### Size Variants
- `.titlebar--sm`: Compact height (40px)
- `.titlebar`: Default height (48px)
- `.titlebar--lg`: Large height (56px)

### Position Variants
- `.titlebar--fixed`: Fixed to viewport
- `.titlebar--sticky`: Sticks when scrolling

## Usage Example

```html
<!-- macOS Style -->
<div class="titlebar titlebar--macos">
  <!-- Window Controls -->
  <div class="titlebar__window-controls">
    <button class="titlebar__window-button titlebar__window-button--close"></button>
    <button class="titlebar__window-button titlebar__window-button--minimize"></button>
    <button class="titlebar__window-button titlebar__window-button--maximize"></button>
  </div>

  <!-- Title -->
  <div class="titlebar__content">
    <h1 class="titlebar__title">
      <span class="titlebar__icon">
        <svg><!-- icon --></svg>
      </span>
      Window Title
    </h1>
    <p class="titlebar__subtitle">Additional details</p>
  </div>

  <!-- Actions -->
  <div class="titlebar__actions">
    <button class="btn">Action</button>
  </div>
</div>

<!-- Windows Style -->
<div class="titlebar titlebar--windows">
  <!-- Same structure as above but controls on right -->
</div>
```

## Features
- Window controls
- macOS style
- Windows style
- Position variants
- Size options
- Glass effect
- Icon support
- Action buttons
- Subtitles
- Animations

## Window Controls
### macOS Style
- Left-aligned
- Colored circles
- Hover symbols
- Traffic light layout
- Smooth transitions

### Windows Style
- Right-aligned
- Monochrome icons
- Hover backgrounds
- Minimalist design
- Close highlight

## Best Practices
- Match OS style
- Clear title text
- Proper spacing
- Icon alignment
- Action grouping
- Touch targets
- Focus states
- Proper contrast
- Semantic markup
- Responsive design