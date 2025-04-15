# Slider Component

A customizable range slider with tooltips, markers, and range selection support.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Thumb background
- `--color-bg-tertiary`: Track background
- `--color-text-secondary`: Label text
- `--color-text-muted`: Marker labels
- `--color-accent`: Active track and thumb
- `--color-accent-rgb`: Focus effects
- `--border-radius-sm`: Tooltip radius
- `--border-radius-full`: Track radius
- `--font-size-xs`: Marker text
- `--font-size-sm`: Value and label text
- `--spacing-xs`: Small padding
- `--spacing-sm`: Label margins
- `--shadow-md`: Thumb shadow
- `--transition-fast`: Hover animations

### Component Variables
- `--thumb-size`: Thumb dimensions (16px - 24px)
- `--track-height`: Track thickness (4px - 8px)
- `--value-percent`: Fill percentage
- `--value-left`: Tooltip position

## Classes

### Base Classes
- `.slider`: Main container
- `.slider__input`: Range input
- `.slider__value`: Value tooltip
- `.slider__labels`: End labels
- `.slider__marker`: Tick marks
- `.slider__marker-label`: Tick labels

### Size Variants
- `.slider--sm`: Small size
- `.slider--lg`: Large size

### Range Variant
- `.slider--range`: Dual thumb mode
- `.slider__track`: Range track
- `.slider__track-fill`: Active range

## Usage Example

```html
<!-- Basic Slider -->
<div class="slider">
  <input type="range" class="slider__input" min="0" max="100">
  <div class="slider__value">50</div>
</div>

<!-- With Markers -->
<div class="slider">
  <input type="range" class="slider__input">
  <div class="slider__marker" style="left: 0%">
    <span class="slider__marker-label">0</span>
  </div>
  <div class="slider__marker" style="left: 50%">
    <span class="slider__marker-label">50</span>
  </div>
  <div class="slider__marker" style="left: 100%">
    <span class="slider__marker-label">100</span>
  </div>
</div>

<!-- Range Slider -->
<div class="slider slider--range">
  <div class="slider__track">
    <div class="slider__track-fill"></div>
  </div>
  <input type="range" class="slider__input" min="0" max="100">
  <input type="range" class="slider__input" min="0" max="100">
</div>
```

## Features
- Value tooltip display
- Custom track colors
- Gradient track fill
- Custom thumb design
- Size variations
- Range selection
- Tick markers
- Value labels
- Disabled state
- Focus styles
- Smooth animations

## Interactions
- Hover effects
- Focus indication
- Drag support
- Value preview
- Scale animation
- Smooth tracking
- Touch support

## Best Practices
- Use appropriate size
- Show value feedback
- Add meaningful markers
- Support keyboard
- Handle touch input
- Consider step values
- Label min/max
- Show current value
- Maintain contrast
- Enable transitions