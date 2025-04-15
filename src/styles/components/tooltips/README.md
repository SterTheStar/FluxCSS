# Tooltips Component

An attribute-driven tooltip system with multiple positions and size options.

## Variables Used

### Core Variables Used
- `--color-bg-tertiary`: Tooltip background
- `--color-text-primary`: Tooltip text
- `--border-radius-sm`: Tooltip corners
- `--spacing-xs`: Small padding
- `--spacing-sm`: Default padding
- `--transition-fast`: Show/hide animations

## Attributes

### Base Attributes
- `data-tooltip`: Tooltip text content
- `data-tooltip-position`: Placement option
- `data-tooltip-size`: Content width

### Position Options
- Default: Top center
- `right`: Right side
- `left`: Left side

### Size Options
- Default: Auto width
- `large`: Fixed 300px width

## Usage Example

```html
<!-- Basic Tooltip -->
<button data-tooltip="Helpful information">Hover me</button>

<!-- Right Position -->
<button data-tooltip="Right side tooltip" data-tooltip-position="right">
  Right tooltip
</button>

<!-- Left Position -->
<button data-tooltip="Left side tooltip" data-tooltip-position="left">
  Left tooltip
</button>

<!-- Large Size -->
<button data-tooltip="A longer tooltip with multiple words that wrap to multiple lines" data-tooltip-size="large">
  Large tooltip
</button>
```

## Features
- Attribute-based setup
- Multiple positions
- Size variations
- Arrow indicators
- Hover activation
- Smooth animations
- Text wrapping
- Clean design

## Positioning
### Top (Default)
- Above target
- Centered alignment
- Downward arrow

### Right
- Right of target
- Middle alignment
- Leftward arrow

### Left
- Left of target
- Middle alignment
- Rightward arrow

## Best Practices
- Keep text concise
- Clear descriptions
- Consider position
- Handle overflow
- Maintain spacing
- Ensure contrast
- Support keyboard
- Proper triggers
- Screen reader text
- Mobile handling