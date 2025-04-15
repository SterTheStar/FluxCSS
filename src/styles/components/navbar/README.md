# Navbar Component

A responsive navigation bar with support for branding, menu items, dropdowns, and mobile toggle.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Navbar background
- `--color-bg-tertiary`: Link hover background
- `--color-text-primary`: Brand and toggle color
- `--color-text-secondary`: Link color
- `--color-accent`: Active link color
- `--border-radius-sm`: Link and submenu radius
- `--spacing-xs`: Link padding
- `--spacing-sm`: Horizontal link padding
- `--spacing-md`: Container padding
- `--shadow-sm`: Navbar shadow
- `--shadow-md`: Mobile menu shadow
- `--transition-fast`: Link animations

## Classes

### Base Classes
- `.navbar`: Main container
- `.navbar__container`: Content wrapper
- `.navbar__brand`: Logo/site name
- `.navbar__menu`: Navigation list
- `.navbar__item`: Menu item wrapper
- `.navbar__link`: Navigation link
- `.navbar__toggle`: Mobile menu button
- `.navbar__submenu`: Dropdown menu

### Variants
- `.navbar--transparent`: No background
- `.navbar--fixed`: Sticky to top
- `.navbar__link--active`: Current page

### States
- `.is-active`: Mobile menu visible

## Usage Example

```html
<nav class="navbar">
  <div class="navbar__container">
    <!-- Brand -->
    <a href="/" class="navbar__brand">Logo</a>

    <!-- Mobile Toggle -->
    <button class="navbar__toggle">☰</button>

    <!-- Navigation -->
    <ul class="navbar__menu">
      <li class="navbar__item">
        <a href="/" class="navbar__link navbar__link--active">Home</a>
      </li>
      
      <!-- Dropdown -->
      <li class="navbar__item">
        <a href="#" class="navbar__link">Products</a>
        <ul class="navbar__submenu">
          <li><a href="#" class="navbar__link">Category 1</a></li>
          <li><a href="#" class="navbar__link">Category 2</a></li>
        </ul>
      </li>
      
      <li class="navbar__item">
        <a href="/about" class="navbar__link">About</a>
      </li>
    </ul>
  </div>
</nav>
```

## Features
- Responsive design
- Mobile hamburger menu
- Dropdown support
- Active state styling
- Hover effects
- Fixed position option
- Transparent variant
- Container width limit
- Smooth transitions
- Nested navigation

## Mobile Behavior
- Hamburger menu toggle
- Vertical menu layout
- Full-width dropdown
- Touch-friendly targets
- Maintained hierarchy
- Proper spacing
- Shadow elevation

## Best Practices
- Clear navigation labels
- Consistent spacing
- Mobile-first approach
- Accessible markup
- Keyboard navigation
- Dropdown indicators
- Active state feedback
- Touch target sizing
- Proper heading structure
- Semantic HTML use

## Responsive Design
- Breakpoint: 768px
- Collapsible menu
- Preserved functionality
- Maintained readability
- Adapted layout
- Proper spacing
- Touch optimization