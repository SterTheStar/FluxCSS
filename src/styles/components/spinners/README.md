# Spinners Component

A collection of loading indicators with multiple variants and sizes.

## Variables Used

### Core Variables Used
- `--color-bg-tertiary`: Spinner track color
- `--color-accent`: Active spinner color

## Classes

### Base Classes
- `.spinner`: Basic circular loader

### Size Variants
- `.spinner--sm`: Small (1rem)
- `.spinner`: Default (2rem)
- `.spinner--lg`: Large (3rem)

### Style Variants
- `.spinner--dots`: Dual dot animation
- `.spinner--pulse`: Expanding circle effect

## Usage Example

```html
<!-- Basic Spinner -->
<div class="spinner"></div>

<!-- Size Variants -->
<div class="spinner spinner--sm"></div>
<div class="spinner spinner--lg"></div>

<!-- Dots Animation -->
<div class="spinner spinner--dots"></div>

<!-- Pulse Effect -->
<div class="spinner spinner--pulse"></div>
```

## Features
- Multiple animation styles
- Three size options
- Smooth animations
- Minimal markup
- Customizable colors
- Performance optimized
- Clean aesthetics

## Animations
### Circular Spinner
- 360° rotation
- 0.75s duration
- Linear timing
- Infinite loop

### Dots Animation
- Scale and fade
- 1s duration
- Ease-in-out timing
- Alternating dots

### Pulse Effect
- Scale and fade
- 1.5s duration
- Ease-out timing
- Expanding ripple

## Best Practices
- Use appropriate size
- Maintain contrast
- Consider context
- Avoid multiple spinners
- Keep animations subtle
- Ensure accessibility
- Provide loading text
- Handle timeouts
- Consider fallbacks
- Match theme colors