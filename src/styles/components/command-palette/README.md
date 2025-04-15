# Command Palette Component

A keyboard-driven command interface inspired by popular IDE and application command palettes.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Palette background
- `--color-bg-tertiary`: Borders and hover states
- `--color-text-primary`: Main text color
- `--color-text-muted`: Icons and secondary text
- `--border-radius-lg`: Container radius
- `--border-radius-sm`: Shortcut keys radius
- `--border-radius-full`: Scrollbar radius
- `--font-size-sm`: Subtitle and shortcut text
- `--font-size-lg`: Search input text
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Default padding
- `--spacing-md`: Section padding
- `--spacing-lg`: Empty state padding
- `--shadow-lg`: Container shadow
- `--z-modal`: Stack order
- `--transition-normal`: Show/hide animations
- `--transition-fast`: Hover transitions

## Classes

### Base Classes
- `.command-palette`: Overlay container
- `.command-palette__container`: Main palette window
- `.command-palette__input-wrapper`: Search input container
- `.command-palette__results`: Results list container
- `.command-palette__input`: Search input field

### Search Elements
- `.command-palette__search-icon`: Search icon
- `.command-palette__shortcuts`: Keyboard shortcuts
- `.command-palette__shortcut`: Individual shortcut key

### Results
- `.command-palette__group-title`: Category headers
- `.command-palette__item`: Result item
- `.command-palette__item-icon`: Item icon
- `.command-palette__item-content`: Item text container
- `.command-palette__item-title`: Item main text
- `.command-palette__item-subtitle`: Item description
- `.command-palette__empty`: No results state

### States
- `.is-active`: Visible state
- `.command-palette__item--active`: Selected item

## Usage Example

```html
<div class="command-palette">
  <div class="command-palette__container">
    <!-- Search Input -->
    <div class="command-palette__input-wrapper">
      <svg class="command-palette__search-icon"><!-- icon svg --></svg>
      <input class="command-palette__input" type="text" placeholder="Search commands...">
      <div class="command-palette__shortcuts">
        <span class="command-palette__shortcut">⌘</span>
        <span class="command-palette__shortcut">K</span>
      </div>
    </div>

    <!-- Results -->
    <div class="command-palette__results">
      <div class="command-palette__group-title">Actions</div>
      
      <div class="command-palette__item">
        <svg class="command-palette__item-icon"><!-- icon svg --></svg>
        <div class="command-palette__item-content">
          <span class="command-palette__item-title">New File</span>
          <span class="command-palette__item-subtitle">Create a new file</span>
        </div>
        <div class="command-palette__shortcuts">
          <span class="command-palette__shortcut">⌘N</span>
        </div>
      </div>
      
      <!-- More items... -->
    </div>
  </div>
</div>
```

## Features
- Keyboard-driven interface
- Search functionality
- Grouped results
- Keyboard shortcuts display
- Active item highlighting
- Empty state handling
- Smooth animations
- Custom scrollbar styling
- Responsive design
- Accessible navigation

## Interactions
- Shows/hides with transition
- Keyboard navigation support
- Search filtering
- Shortcut key hints
- Hover and active states
- Scroll with custom styling

## Animations
- Fade in/out overlay
- Slide up/down container
- Smooth hover transitions
- Focus transitions

## Best Practices
- Use clear, descriptive titles
- Include keyboard shortcuts
- Group related items
- Provide helpful subtitles
- Support keyboard navigation
- Maintain consistent icons