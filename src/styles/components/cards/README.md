# Card Component

A versatile card component for displaying content in a contained format with multiple variants and layouts.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Text color for primary variant
- `--color-bg-secondary`: Default card background
- `--color-bg-secondary-rgb`: For overlay effects
- `--color-bg-tertiary`: Border colors
- `--color-text-primary`: Title text color
- `--color-text-secondary`: Body text color
- `--color-accent`: Hover border and primary variant
- `--border-radius-lg`: Card container radius
- `--font-size-sm`: Small text size
- `--font-size-lg`: Title size
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Small padding
- `--spacing-md`: Default padding
- `--spacing-lg`: Large padding
- `--spacing-xl`: Extra large padding
- `--shadow-md`: Default shadow
- `--shadow-lg`: Hover shadow
- `--transition-normal`: Hover animations
- `--animation-smooth`: Entry animation timing

## Classes

### Base Classes
- `.card`: Main container
- `.card__header`: Header section
- `.card__title`: Card title
- `.card__subtitle`: Secondary title
- `.card__body`: Main content area
- `.card__footer`: Footer section
- `.card__image`: Card image
- `.card__actions`: Action buttons container

### Variants
- `.card--interactive`: Clickable card
- `.card--hover-accent`: Accent border on hover
- `.card--bordered`: With border
- `.card--primary`: Accent colored header
- `.card--outline`: Transparent background
- `.card--glass`: Glassmorphism effect
- `.card--horizontal`: Side-by-side layout
- `.card--overlay`: Image overlay with gradient

### Sizes
- `.card--sm`: Smaller padding
- `.card--lg`: Larger padding

### States
- `.card--loading`: Loading state with animation
- `.card--hover-reveal`: Reveals content on hover

### Layout
- `.card-grid`: Grid container for cards

## Usage Examples

```html
<!-- Basic Card -->
<div class="card">
  <div class="card__header">
    <h3 class="card__title">Card Title</h3>
    <p class="card__subtitle">Subtitle</p>
  </div>
  <div class="card__body">
    Content goes here
  </div>
  <div class="card__footer">
    <button class="btn">Action</button>
  </div>
</div>

<!-- Card with Image -->
<div class="card">
  <img class="card__image" src="image.jpg" alt="Card image">
  <div class="card__body">
    Content with image
  </div>
</div>

<!-- Horizontal Card -->
<div class="card card--horizontal">
  <img class="card__image" src="image.jpg" alt="Side image">
  <div class="card__content">
    <div class="card__body">Side by side content</div>
  </div>
</div>

<!-- Card Grid -->
<div class="card-grid">
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
</div>
```

## Features
- Multiple layout options (vertical, horizontal, overlay)
- Various style variants (bordered, outline, glass)
- Interactive states and animations
- Loading state with shimmer effect
- Responsive design
- Grid layout system
- Action buttons support
- Image integration
- Hover effects
- Entry animations

## Responsive Behavior
- Grid adjusts columns based on viewport
- Actions move to bottom on mobile
- Padding reduces on smaller screens
- Maintains readability across devices

## Animations
- Smooth hover transitions
- Loading state shimmer
- Entry animation
- Content reveal effects