# Tree Component

A hierarchical tree view component with selection, actions, and drag-and-drop capabilities.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Action backgrounds
- `--color-bg-tertiary`: Hover state
- `--color-text-primary`: Node text
- `--color-text-muted`: Icons and actions
- `--color-accent`: Selection and checkbox
- `--border-radius-sm`: Node and checkbox
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Default gaps
- `--spacing-lg`: Branch indent
- `--transition-fast`: Hover effects

## Classes

### Base Classes
- `.tree`: Main container
- `.tree__list`: Node container
- `.tree__item`: Tree item wrapper
- `.tree__branch`: Child nodes
- `.tree__node`: Individual node
- `.tree__toggle`: Expand button
- `.tree__icon`: Node icon
- `.tree__label`: Node text

### Checkboxes
- `.tree__checkbox`: Checkbox wrapper
- `.tree__checkbox-input`: Custom checkbox

### Actions
- `.tree__actions`: Actions container
- `.tree__action`: Action button

### States
- `.tree__node--selected`: Selected node
- `.tree__item--expanded`: Open branch
- `.tree__node--loading`: Loading state
- `.tree__node--dragging`: During drag
- `.tree__node--drop-target`: Drop zone

### Variants
- `.tree--connected`: With branch lines

## Usage Example

```html
<div class="tree tree--connected">
  <ul class="tree__list">
    <!-- Node with Children -->
    <li class="tree__item tree__item--expanded">
      <div class="tree__node">
        <button class="tree__toggle">›</button>
        <span class="tree__icon">📁</span>
        <span class="tree__label">Folder</span>
        <div class="tree__actions">
          <button class="tree__action">+</button>
          <button class="tree__action">⋮</button>
        </div>
      </div>
      
      <ul class="tree__branch">
        <!-- Child Node -->
        <li class="tree__item">
          <div class="tree__node">
            <span class="tree__icon">📄</span>
            <span class="tree__label">File</span>
          </div>
        </li>
      </ul>
    </li>

    <!-- Selectable Node -->
    <li class="tree__item">
      <div class="tree__node">
        <label class="tree__checkbox">
          <input type="checkbox" class="tree__checkbox-input">
        </label>
        <span class="tree__icon">📄</span>
        <span class="tree__label">Selectable Item</span>
      </div>
    </li>
  </ul>
</div>
```

## Features
- Nested hierarchy
- Branch expansion
- Node selection
- Checkbox support
- Action buttons
- Loading states
- Connecting lines
- Hover effects
- Drag and drop
- Custom icons

## Interactions
- Click to select
- Toggle expansion
- Checkbox states
- Action triggers
- Drag to move
- Drop to place
- Show/hide actions
- Loading feedback

## Best Practices
- Clear hierarchy
- Consistent icons
- Proper indentation
- Action visibility
- Loading indicators
- Selection states
- Touch targets
- Keyboard support
- Drag feedback
- Mobile handling