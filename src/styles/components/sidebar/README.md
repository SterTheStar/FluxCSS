# Sidebar Component

A modern sidebar navigation with glass-morphism effect, search functionality, and responsive behavior.

## Variables Used

### Core Variables Used
- `--color-bg-secondary-rgb`: Glass background
- `--color-bg-tertiary-rgb`: Border and hover effects
- `--color-text-primary`: Main text color
- `--color-text-secondary`: Link color
- `--color-text-muted`: Section titles
- `--color-accent`: Active states
- `--color-accent-rgb`: Active backgrounds
- `--border-radius-lg`: Link radius
- `--border-radius-full`: Close button/scrollbar
- `--font-size-sm`: Small text
- `--font-size-lg`: Header text
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Default gaps
- `--spacing-md`: Section padding
- `--spacing-lg`: Section margins
- `--shadow-lg`: Active state
- `--z-sidebar`: Stack order
- `--transition-normal`: Show/hide
- `--transition-fast`: Hover effects
- `--animation-smooth`: Motion timing

## Classes

### Base Classes
- `.sidebar`: Main container
- `.sidebar__header`: Top section
- `.sidebar__search`: Search area
- `.sidebar__content`: Navigation area
- `.sidebar__footer`: Bottom section
- `.sidebar-overlay`: Mobile backdrop

### Navigation
- `.sidebar__section`: Group container
- `.sidebar__section-header`: Group title
- `.sidebar__section-title`: Group heading
- `.sidebar__link`: Navigation link
- `.sidebar__title`: Sidebar heading
- `.sidebar__close`: Close button

### States
- `.is-active`: Visible state
- `.sidebar__link.is-active`: Current page

## Usage Example

```html
<div class="sidebar">
  <!-- Header -->
  <div class="sidebar__header">
    <h1 class="sidebar__title">Dashboard</h1>
    <button class="sidebar__close">×</button>
  </div>

  <!-- Search -->
  <div class="sidebar__search">
    <div class="input-group">
      <span class="input-group-prepend">
        <svg><!-- search icon --></svg>
      </span>
      <input class="input" placeholder="Search...">
    </div>
  </div>

  <!-- Content -->
  <div class="sidebar__content">
    <div class="sidebar__section">
      <div class="sidebar__section-header">
        <h2 class="sidebar__section-title">Main Menu</h2>
      </div>

      <a href="#" class="sidebar__link is-active">
        <svg><!-- icon --></svg>
        Dashboard
        <span class="badge">3</span>
      </a>
    </div>
  </div>

  <!-- Footer -->
  <div class="sidebar__footer">
    <div class="sidebar__theme-toggle">
      <!-- Theme toggle content -->
    </div>
  </div>
</div>

<!-- Mobile Overlay -->
<div class="sidebar-overlay"></div>
```

## Features
- Glass-morphism design
- Search functionality
- Grouped navigation
- Active state indicators
- Badge support
- Sticky header/footer
- Custom scrollbar
- Mobile responsive
- Smooth animations
- Icon integration

## Responsive Behavior
- Desktop: Fixed open (≥1024px)
  - Content margin adjustment
  - Hidden close button
  - No overlay
- Mobile: Slide-in (<1024px)
  - Full height
  - Max width: 320px
  - Backdrop overlay
  - Close button
  - Glass effect header/footer

## Glass-morphism Effects
- Background blur
- Semi-transparent background
- Frosted glass appearance
- Layered blur effects
- Smooth transitions

## Best Practices
- Clear hierarchy
- Visible active states
- Smooth transitions
- Touch targets
- Keyboard navigation
- Proper spacing
- Icon consistency
- Mobile optimization
- Performance consideration
- Accessibility support