# Carousel Component

A feature-rich slideshow component for cycling through elements like images, with navigation, indicators, and thumbnails.

## Variables Used

### Core Variables Used
- `--color-text-primary`: Navigation buttons and caption text
- `--color-bg-secondary`: Loading state background
- `--color-accent`: Active indicator and thumbnail border
- `--border-radius-sm`: Thumbnail and zoom button radius
- `--spacing-xs`: Small gaps and mobile padding
- `--spacing-sm`: Default gaps and button spacing
- `--spacing-md`: Navigation padding and caption
- `--transition-fast`: Button and indicator animations
- `--transition-normal`: Slide transitions
- `--animation-smooth`: Slide transition timing

## Classes

### Base Classes
- `.carousel`: Main container
- `.carousel__track`: Slides container
- `.carousel__slide`: Individual slide
- `.carousel__image`: Slide image
- `.carousel__caption`: Text overlay for slides

### Navigation
- `.carousel__nav`: Navigation container
- `.carousel__button`: Previous/Next buttons
- `.carousel__indicators`: Dots container
- `.carousel__indicator`: Individual dot
- `.carousel__indicator--active`: Active dot

### Thumbnails
- `.carousel__thumbnails`: Thumbnail strip
- `.carousel__thumbnail`: Individual thumbnail
- `.carousel__thumbnail--active`: Selected thumbnail

### States
- `.carousel__slide--loading`: Loading placeholder
- `.carousel__slide--active`: Currently visible slide

### Variants
- `.carousel--fade`: Fade transition effect

## Usage Example

```html
<!-- Basic Carousel -->
<div class="carousel">
  <div class="carousel__track">
    <div class="carousel__slide">
      <img class="carousel__image" src="slide1.jpg" alt="Slide 1">
      <div class="carousel__caption">Caption Text</div>
    </div>
    <!-- More slides... -->
  </div>
  
  <!-- Navigation -->
  <div class="carousel__nav">
    <button class="carousel__button">←</button>
    <button class="carousel__button">→</button>
  </div>
  
  <!-- Indicators -->
  <div class="carousel__indicators">
    <button class="carousel__indicator carousel__indicator--active"></button>
    <button class="carousel__indicator"></button>
    <!-- More indicators... -->
  </div>
  
  <!-- Thumbnails -->
  <div class="carousel__thumbnails">
    <div class="carousel__thumbnail carousel__thumbnail--active">
      <img src="thumb1.jpg" alt="Thumbnail 1">
    </div>
    <!-- More thumbnails... -->
  </div>
</div>
```

## Features
- Smooth slide transitions
- Fade transition option
- Navigation buttons
- Dot indicators
- Thumbnail navigation
- Touch gesture support
- Loading state
- Image captions
- Zoom functionality
- Responsive design
- Touch-friendly interface

## Touch Interactions
- Supports swipe gestures
- Pan and pinch-zoom enabled
- Touch-optimized thumbnails
- Smooth mobile experience

## Responsive Behavior
- Adapts to screen sizes
- Smaller controls on mobile
- Compact thumbnails on small screens
- Maintains usability across devices

## Animations
- Smooth slide transitions
- Fade effect option
- Interactive button animations
- Active state transitions
- Loading state handling