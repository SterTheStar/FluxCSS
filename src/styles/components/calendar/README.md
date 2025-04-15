# Calendar Component

A comprehensive date and time picker component with multiple selection modes and navigation features.

## Variables Used

### Core Variables Used
- `--color-bg-primary`: Text color for selected states
- `--color-bg-secondary`: Calendar background
- `--color-bg-tertiary`: Button backgrounds and borders
- `--color-text-primary`: Main text color
- `--color-text-secondary`: Day number colors
- `--color-text-muted`: Weekday labels and disabled states
- `--color-accent`: Selected dates and hover states
- `--border-radius-sm`: Small elements radius
- `--border-radius-lg`: Calendar container radius
- `--border-radius-full`: Circular buttons and days
- `--font-size-sm`: Day and button text size
- `--spacing-xs`: Grid and small element gaps
- `--spacing-sm`: Internal padding
- `--spacing-md`: Header and section padding
- `--shadow-lg`: Calendar container shadow
- `--transition-fast`: Hover and interaction animations
- `--animation-smooth`: Slide animation timing

## Classes

### Base Classes
- `.calendar`: Main container
- `.calendar__header`: Month/year display and navigation
- `.calendar__grid`: Days grid container
- `.calendar__weekdays`: Weekday labels row
- `.calendar__days`: Days grid
- `.calendar__time`: Time picker section
- `.calendar__footer`: Actions footer

### Interactive Elements
- `.calendar__nav-button`: Navigation buttons
- `.calendar__day`: Individual day button
- `.calendar__time-input`: Time input fields
- `.calendar__select-item`: Month/year selection items
- `.calendar__footer-button`: Footer action buttons

### States and Variants
- `.calendar__day--today`: Current day
- `.calendar__day--selected`: Selected day
- `.calendar__day--range-start`: Range selection start
- `.calendar__day--range-end`: Range selection end
- `.calendar__day--in-range`: Days within selected range
- `.calendar--multi`: Multiple calendar view
- `.calendar--animate-in`: Entry animation

## Usage Example

```html
<!-- Basic Calendar -->
<div class="calendar">
  <div class="calendar__header">
    <span class="calendar__title">September 2023</span>
    <div class="calendar__nav">
      <button class="calendar__nav-button">←</button>
      <button class="calendar__nav-button">→</button>
    </div>
  </div>
  
  <div class="calendar__grid">
    <div class="calendar__weekdays">
      <span class="calendar__weekday">Su</span>
      <!-- ...other weekdays... -->
    </div>
    
    <div class="calendar__days">
      <!-- Calendar days -->
    </div>
  </div>
  
  <!-- Optional Time Picker -->
  <div class="calendar__time">
    <div class="calendar__time-inputs">
      <input type="text" class="calendar__time-input" placeholder="HH">
      <span class="calendar__time-separator">:</span>
      <input type="text" class="calendar__time-input" placeholder="MM">
    </div>
  </div>
  
  <!-- Optional Footer -->
  <div class="calendar__footer">
    <button class="calendar__footer-button">Cancel</button>
    <button class="calendar__footer-button">Apply</button>
  </div>
</div>
```

## Features
- Date selection with current day highlight
- Date range selection
- Time picker integration
- Month and year navigation
- Multiple calendar view for range selection
- Responsive design
- Entry animation
- Disabled dates support
- Month/Year selection interface
- Footer with action buttons
- Customizable through CSS variables

## Responsive Behavior
- Single calendar view on mobile
- Stacked layout for multiple calendars on small screens
- Touch-friendly sizing for interactive elements

## Animations
- Smooth hover transitions
- Slide-down entry animation
- Interactive state transitions