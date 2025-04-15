# Inputs Component

A flexible input component with validation states and grouping capabilities.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Input background
- `--color-bg-tertiary`: Border color
- `--color-text-primary`: Input text color
- `--color-text-secondary`: Label text color
- `--color-text-muted`: Placeholder text
- `--color-accent`: Focus border color
- `--border-radius-sm`: Input corners
- `--spacing-xs`: Group gaps
- `--spacing-sm`: Vertical padding
- `--spacing-md`: Horizontal padding
- `--shadow-sm`: Focus shadow
- `--transition-normal`: State transitions

## Classes

### Base Classes
- `.input`: Main input class
- `.input-group`: Input wrapper with label
- `.input-label`: Input label
- `.input-error`: Error message

### States
- `.input--error`: Error state
- `.input--success`: Success state

## Usage Example

```html
<!-- Basic Input -->
<input type="text" class="input" placeholder="Enter text">

<!-- Input with Label -->
<div class="input-group">
  <label class="input-label">Username</label>
  <input type="text" class="input">
</div>

<!-- Input with Error -->
<div class="input-group">
  <label class="input-label">Email</label>
  <input type="email" class="input input--error">
  <span class="input-error">Please enter a valid email address</span>
</div>

<!-- Input with Success -->
<div class="input-group">
  <label class="input-label">Password</label>
  <input type="password" class="input input--success">
</div>
```

## Features
- Clean, minimal design
- Validation states
- Label support
- Error messaging
- Consistent spacing
- Focus states
- Placeholder styling
- Smooth transitions

## States
- Default
- Focus
- Error
- Success
- Disabled
- Read-only

## Best Practices
- Use clear labels
- Show validation feedback
- Maintain consistent spacing
- Include placeholder text
- Handle focus states
- Provide error messages
- Use semantic HTML
- Support keyboard navigation
- Follow accessibility guidelines
- Consider mobile input types

## Responsive Behavior
- Full width by default
- Consistent touch targets
- Clear focus indicators
- Readable text size
- Mobile-friendly padding