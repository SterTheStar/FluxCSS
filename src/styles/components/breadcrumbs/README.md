# Breadcrumb Component

A navigation component that indicates the current page's location within a navigational hierarchy.

## Variables Used

### Core Variables Used
- `--color-text-secondary`: Color for breadcrumb items
- `--color-text-primary`: Color for active/current item
- `--color-text-muted`: Color for separators
- `--color-text-inverse`: Color for text on accent backgrounds
- `--color-accent`: Hover color for links and theme accents
- `--color-accent-light`: Used in gradient theme
- `--color-bg-primary`: Background for modern theme
- `--color-bg-secondary`: Background for variants
- `--color-border`: Border color for bordered theme
- `--border-radius-sm`: Small border radius
- `--border-radius-lg`: Large border radius for modern theme
- `--shadow-sm`: Shadow for modern theme
- `--spacing-xs`: Extra small spacing
- `--spacing-sm`: Default spacing
- `--spacing-md`: Medium spacing
- `--transition-fast`: Animation speed

## Classes

### Base Classes
- `.breadcrumb`: Main container
- `.breadcrumb__item`: Individual breadcrumb item
- `.breadcrumb__link`: Clickable link within item
- `.breadcrumb__separator`: Divider between items
- `.breadcrumb__icon`: Icon element

### Theme Variants
- `.breadcrumb--bg`: Classic background variant
- `.breadcrumb--modern`: Elevated design with shadow
- `.breadcrumb--pill`: Pill-shaped items without separators
- `.breadcrumb--bordered`: Simple border outline
- `.breadcrumb--gradient`: Gradient background for current item

### Separator Styles
- `.breadcrumb--chevron`: Uses › as separator
- `.breadcrumb--arrow`: Uses → as separator
- `.breadcrumb--dot`: Uses • as separator

### Enhanced Features
- `.breadcrumb--animated`: Adds underline animation on hover
- `.breadcrumb--responsive`: Collapses on mobile screens
- `.breadcrumb--with-icons`: Support for icons in items

## Usage Examples

```html
<!-- Modern Theme -->
<nav class="breadcrumb breadcrumb--modern">
  <div class="breadcrumb__item">
    <a href="/" class="breadcrumb__link">Home</a>
    <span class="breadcrumb__separator">/</span>
  </div>
  <div class="breadcrumb__item">Current Page</div>
</nav>

<!-- Pill Style with Icons -->
<nav class="breadcrumb breadcrumb--pill breadcrumb--with-icons">
  <div class="breadcrumb__item">
    <svg class="breadcrumb__icon"><!-- icon svg --></svg>
    <a href="/" class="breadcrumb__link">Home</a>
  </div>
  <div class="breadcrumb__item">Products</div>
</nav>

<!-- Animated with Custom Separator -->
<nav class="breadcrumb breadcrumb--animated breadcrumb--chevron">
  <div class="breadcrumb__item">
    <a href="/" class="breadcrumb__link">Home</a>
    <span class="breadcrumb__separator"></span>
  </div>
  <div class="breadcrumb__item">Current Page</div>
</nav>
```

## Features
- Multiple theme variants (modern, pill, bordered, gradient)
- Custom separator options (chevron, arrow, dot)
- Animated hover effects
- Responsive design with mobile optimization
- Icon support
- Clean and minimal base design
- Accessible navigation structure
- Easy theme combinations (can mix different variants)

## Best Practices
- Choose separators that match your theme's style
- Use icons consistently if implementing the with-icons variant
- Consider using animations for interactive websites
- Implement the responsive variant for better mobile experience
- Match the theme variant to your overall site design
- Use appropriate color variables for maximum theme compatibility

## Responsive Behavior
On screens smaller than 640px, the responsive variant:
- Shows only first and last items
- Replaces middle items with ellipsis
- Reduces gaps between elements
- Maintains theme styling while simplifying layout