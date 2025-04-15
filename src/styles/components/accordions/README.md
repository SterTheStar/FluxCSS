# Accordion Component

The Accordion component provides collapsible content sections that can be expanded or collapsed.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Background color of the accordion
- `--color-bg-tertiary`: Border and hover background color
- `--color-text-primary`: Text color for accordion titles
- `--border-radius-md`: Border radius for the accordion container
- `--border-radius-sm`: Border radius for spaced variant items
- `--spacing-md`: Default padding for header and content
- `--spacing-sm`: Padding for small variant and spacing between items
- `--transition-fast`: Quick transitions for icons and interactions
- `--transition-normal`: Normal speed transitions for content expansion

## Classes

### Base Classes
- `.accordion`: Main container
- `.accordion__item`: Individual accordion section
- `.accordion__header`: Clickable header area
- `.accordion__title`: Title text
- `.accordion__content`: Collapsible content area
- `.is-active`: State class for expanded items

### Variants
- `.accordion--bordered`: Adds border to the accordion
- `.accordion--spaced`: Adds spacing between items
- `.accordion--sm`: Smaller sized variant

## Usage Example

```html
<div class="accordion">
  <div class="accordion__item">
    <div class="accordion__header">
      <span class="accordion__title">Section Title</span>
    </div>
    <div class="accordion__content">
      Content goes here...
    </div>
  </div>
</div>
```

## Modifiers

You can combine different modifiers:
- Use `accordion--bordered` for bordered style
- Use `accordion--spaced` for separated items
- Use `accordion--sm` for smaller size
- Add `is-active` to `accordion__item` to expand a section