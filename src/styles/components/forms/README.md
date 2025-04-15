# Forms Component

A comprehensive form system with styled inputs, groups, custom controls, and validation states.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Input and control backgrounds
- `--color-bg-tertiary`: Input group backgrounds
- `--color-text-primary`: Label text
- `--color-text-muted`: Hint text
- `--color-accent`: Checked states and range thumb
- `--border-radius-sm`: Input and checkbox corners
- `--border-radius-full`: Range track radius
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Default padding
- `--spacing-md`: Form groups gap
- `--transition-fast`: Control animations

## Classes

### Base Classes
- `.form`: Form container
- `.form-group`: Input group wrapper
- `.form-label`: Input label
- `.form-hint`: Help text
- `.form-error`: Error message

### Input Groups
- `.input-group`: Combined inputs wrapper
- `.input-group-prepend`: Leading content
- `.input-group-append`: Trailing content

### Custom Controls
- `.form-check`: Checkbox/radio wrapper
- `.form-check-input`: Custom checkbox/radio
- `.form-select`: Custom select
- `.form-range`: Custom range slider

## Usage Example

```html
<form class="form">
  <!-- Text Input -->
  <div class="form-group">
    <label class="form-label required">Username</label>
    <input type="text" class="input">
    <span class="form-hint">Enter your username</span>
  </div>

  <!-- Input Group -->
  <div class="form-group">
    <label class="form-label">Website</label>
    <div class="input-group">
      <div class="input-group-prepend">https://</div>
      <input type="text" class="input">
      <div class="input-group-append">.com</div>
    </div>
  </div>

  <!-- Custom Checkbox -->
  <label class="form-check">
    <input type="checkbox" class="form-check-input">
    Remember me
  </label>

  <!-- Custom Select -->
  <div class="form-group">
    <label class="form-label">Country</label>
    <select class="form-select">
      <option>Select a country</option>
    </select>
  </div>

  <!-- Range Slider -->
  <div class="form-group">
    <label class="form-label">Volume</label>
    <input type="range" class="form-range">
  </div>
</form>
```

## Features
- Consistent form layout
- Input grouping
- Required field marking
- Help text support
- Error state display
- Custom checkboxes
- Custom radio buttons
- Styled select menus
- Range slider styling
- Input groups with add-ons

## Form Controls
- Text inputs
- Checkboxes
- Radio buttons
- Select menus
- Range sliders
- Input groups
- Labels
- Hints
- Error messages

## Customization
- Custom checkbox icon
- Custom radio design
- Custom select arrow
- Range slider thumb
- Input group combinations
- Required field indicator
- Error text color
- Help text styling

## Best Practices
- Use clear labels
- Indicate required fields
- Provide help text
- Show validation errors
- Group related inputs
- Maintain consistency
- Support keyboard navigation
- Include proper ARIA
- Use semantic markup
- Handle focus states