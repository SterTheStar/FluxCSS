# Tables Component

A comprehensive table system with sorting, filtering, selection, and responsive features.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Header border
- `--color-bg-secondary`: Table background
- `--color-bg-tertiary`: Header and hover
- `--color-text-primary`: Header text
- `--color-text-secondary`: Cell text
- `--color-text-muted`: Empty state
- `--color-accent`: Checkbox and actions
- `--border-radius-md`: Container radius
- `--border-radius-sm`: Input and checkbox
- `--font-size-sm`: Small text
- `--spacing-xs`: Tight padding
- `--spacing-sm`: Small padding
- `--spacing-md`: Default padding
- `--spacing-xl`: Empty state padding
- `--transition-fast`: Hover effects
- `--transition-normal`: Batch actions

## Classes

### Container Classes
- `.table-container`: Scrollable wrapper
- `.table`: Main table element
- `.table__header`: Sticky header
- `.table__row`: Table row
- `.table__cell`: Table cell

### Header Elements
- `.table__header-cell`: Column header
- `.table__header-content`: Header layout
- `.table__sort-icon`: Sort indicator
- `.table__header-cell--sorted`: Sort active
- `.table__header-cell--sorted-desc`: Descending

### Filters
- `.table__filters`: Filter container
- `.table__filter`: Filter group
- `.table__filter-label`: Filter name
- `.table__filter-input`: Filter input

### Selection
- `.table__row--selectable`: Clickable row
- `.table__row--selected`: Selected state
- `.table__checkbox`: Selection box
- `.table__batch-actions`: Multi-select tools
- `.table__selected-count`: Selection counter

### States
- `.table__row--loading`: Loading state
- `.table__cell--loading`: Loading cell
- `.table__empty`: No data state
- `.is-visible`: Show batch actions

### Alignment
- `.table__cell--right`: Right align
- `.table__cell--center`: Center align

## Usage Example

```html
<div class="table-container">
  <!-- Filters -->
  <div class="table__filters">
    <div class="table__filter">
      <label class="table__filter-label">Search:</label>
      <input class="table__filter-input" type="text">
    </div>
  </div>

  <!-- Table -->
  <table class="table">
    <!-- Header -->
    <thead class="table__header">
      <tr>
        <th class="table__header-cell">
          <div class="table__header-content">
            Name
            <svg class="table__sort-icon"><!-- sort icon --></svg>
          </div>
        </th>
      </tr>
    </thead>

    <!-- Body -->
    <tbody>
      <!-- Regular Row -->
      <tr class="table__row">
        <td class="table__cell">Content</td>
      </tr>

      <!-- Selectable Row -->
      <tr class="table__row table__row--selectable">
        <td class="table__cell">
          <input type="checkbox" class="table__checkbox">
          Selectable Content
        </td>
      </tr>

      <!-- Loading Row -->
      <tr class="table__row table__row--loading">
        <td class="table__cell table__cell--loading"></td>
      </tr>
    </tbody>
  </table>

  <!-- Batch Actions -->
  <div class="table__batch-actions">
    <span class="table__selected-count">2 items selected</span>
    <button class="btn">Delete</button>
  </div>
</div>
```

## Features
- Column sorting
- Data filtering
- Row selection
- Batch actions
- Loading states
- Empty states
- Sticky header
- Custom scrolling
- Responsive layout
- Cell alignment

## Responsive Behavior
- Horizontal scrolling
- Stack layout on mobile
- Label/value pairs
- Preserved data
- Touch friendly
- Maintained hierarchy

## Best Practices
- Clear column headers
- Consistent alignment
- Loading indicators
- Empty state handling
- Touch targets
- Sort indicators
- Filter accessibility
- Batch action feedback
- Mobile optimization
- Performance handling