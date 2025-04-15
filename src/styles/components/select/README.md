# Select Component

A feature-rich select component with search functionality, multi-select support, and grouped options.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Background colors
- `--color-bg-tertiary`: Borders and hover states
- `--color-text-primary`: Main text color
- `--color-text-secondary`: Option text color
- `--color-text-muted`: Placeholder and group labels
- `--color-accent`: Selected item and focus
- `--border-radius-sm`: Input corners
- `--border-radius-md`: Dropdown corners
- `--border-radius-full`: Tag and scrollbar radius
- `--font-size-sm`: Small text elements
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Default padding
- `--spacing-md`: Large padding
- `--shadow-lg`: Dropdown shadow
- `--z-dropdown`: Stack order
- `--transition-fast`: Hover animations
- `--transition-normal`: Dropdown animation

## Classes

### Base Classes
- `.select`: Main container
- `.select__trigger`: Dropdown button
- `.select__dropdown`: Options container
- `.select__options`: Options wrapper
- `.select__option`: Individual option

### Search
- `.select__search`: Search container
- `.select__search-input`: Search input

### Multi-select
- `.select__tags`: Selected items wrapper
- `.select__tag`: Selected item tag
- `.select__tag-remove`: Tag remove button

### States
- `.is-open`: Dropdown visible
- `.select__option--selected`: Selected option
- `.select__option--disabled`: Disabled option

### Groups
- `.select__group-label`: Option group header

## Usage Example

```html
<!-- Basic Select -->
<div class="select">
  <button class="select__trigger">
    Select an option
    <svg class="select__trigger-icon"><!-- arrow icon --></svg>
  </button>
  
  <div class="select__dropdown">
    <!-- Search -->
    <div class="select__search">
      <input class="select__search-input" placeholder="Search...">
    </div>
    
    <!-- Options -->
    <div class="select__options">
      <!-- Group -->
      <div class="select__group">
        <div class="select__group-label">Category</div>
        <div class="select__option">Option 1</div>
        <div class="select__option select__option--selected">Option 2</div>
        <div class="select__option select__option--disabled">Option 3</div>
      </div>
    </div>
  </div>
</div>

<!-- Multi-select -->
<div class="select">
  <div class="select__tags">
    <div class="select__tag">
      Selected Item
      <button class="select__tag-remove">×</button>
    </div>
  </div>
  <!-- Same structure as above -->
</div>
```

## Features
- Searchable options
- Multi-select support
- Option grouping
- Disabled states
- Custom scrollbar
- Selected indicators
- Removable tags
- Smooth animations
- Keyboard navigation
- Empty state handling

## Interactions
- Click to open/close
- Search filtering
- Option selection
- Tag removal
- Keyboard support
- Focus management
- Scroll within dropdown

## Best Practices
- Clear option labels
- Group related options
- Show selected state
- Handle empty states
- Enable keyboard use
- Support screen readers
- Maintain focus
- Proper ARIA labels
- Touch-friendly targets
- Performance optimization