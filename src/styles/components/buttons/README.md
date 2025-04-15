# Button Component

A versatile button component with multiple variants, states, and modifiers.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Text color for accent buttons
- `--color-bg-secondary`: Secondary button background
- `--color-bg-tertiary`: Default button background
- `--color-text-primary`: Default text color
- `--color-text-secondary`: Ghost button text color
- `--color-accent`: Primary and accent button background
- `--color-accent-rgb`: For shadow and hover effects
- `--color-error`: Danger button background
- `--color-error-rgb`: For danger button effects
- `--border-radius-sm`: Default border radius
- `--border-radius-full`: For badge counter
- `--font-size-xs`: Badge text size
- `--font-size-sm`: Default button text
- `--font-size-base`: Large button text
- `--spacing-xs`: Small button padding
- `--spacing-sm`: Default padding and gap
- `--spacing-md`: Medium button padding
- `--spacing-lg`: Default horizontal padding
- `--spacing-xl`: Large button padding
- `--shadow-sm`: Button shadow
- `--transition-fast`: Hover and click animations

## Classes

### Base Class
- `.btn`: Main button class

### Variants
- `.btn--primary`: Main call-to-action
- `.btn--secondary`: Less prominent actions
- `.btn--accent`: Gradient accent style
- `.btn--outline`: Bordered style
- `.btn--ghost`: Minimal style
- `.btn--danger`: Destructive actions

### Sizes
- `.btn--sm`: Small size
- `.btn--lg`: Large size
- `.btn--block`: Full width

### States
- `:disabled`: Disabled state
- `.btn--loading`: Loading state with spinner

### Modifiers
- `.btn--icon`: Square icon button
- `.btn-badge`: Button with counter badge
- `.btn-group`: Button group container

## Usage Examples

```html
<!-- Basic Buttons -->
<button class="btn">Default</button>
<button class="btn btn--primary">Primary</button>
<button class="btn btn--secondary">Secondary</button>
<button class="btn btn--accent">Accent</button>
<button class="btn btn--outline">Outline</button>
<button class="btn btn--ghost">Ghost</button>
<button class="btn btn--danger">Danger</button>

<!-- Sizes -->
<button class="btn btn--sm">Small</button>
<button class="btn btn--lg">Large</button>
<button class="btn btn--block">Full Width</button>

<!-- States -->
<button class="btn" disabled>Disabled</button>
<button class="btn btn--loading">Loading</button>

<!-- With Icon -->
<button class="btn btn--icon">
  <svg><!-- icon svg --></svg>
</button>

<!-- With Badge -->
<button class="btn btn-badge" data-count="5">
  Notifications
</button>

<!-- Button Group -->
<div class="btn-group">
  <button class="btn">Left</button>
  <button class="btn">Middle</button>
  <button class="btn">Right</button>
</div>
```

## Features
- Multiple semantic variants
- Three size options
- Loading state with spinner
- Icon button support
- Badge counter support
- Button grouping
- Disabled state styling
- Hover and active effects
- Focus state with ring
- Ripple effect on click
- Full width option
- Consistent spacing and alignment
- Accessible states and focus

## Interactive Effects
- Hover: Slight lift and shadow
- Active: Returns to position
- Focus: Accent-colored ring
- Click: Ripple effect
- Loading: Spinning animation