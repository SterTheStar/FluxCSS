# Terminal Component

A highly customizable terminal/log viewer component with multiple themes, sizes, and style variants.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Terminal background
- `--color-bg-tertiary`: Header and borders
- `--color-bg-tertiary-rgb`: Action hover effect
- `--color-text-primary`: Main text color
- `--color-text-secondary`: Output text color
- `--color-text-muted`: Action button color
- `--color-accent`: Prompt color
- `--color-error`: Error messages
- `--color-warning`: Warning messages
- `--color-success`: Success messages
- `--color-info`: Info messages

### Component Variables
- `--terminal-height`: Container height (default: 300px)
- `--terminal-opacity`: Content opacity (default: 1)
- `--terminal-header-height`: Header size (default: 40px)
- `--terminal-font`: Custom monospace font (default: 'Fira Code', 'Cascadia Code', monospace)
- `--terminal-blur`: Glass effect strength (default: 10px)
- `--terminal-prompt`: Custom prompt symbol (default: '$')

## Classes

### Base Classes
- `.terminal`: Main container
- `.terminal__header`: Top bar area
- `.terminal__title`: Window title
- `.terminal__icon`: Title icon
- `.terminal__actions`: Header buttons
- `.terminal__action`: Individual button
- `.terminal__content`: Output area

### Line Types
- `.terminal__line`: Base line wrapper
- `.terminal__prompt`: Command prefix (uses --terminal-prompt)
- `.terminal__command`: Input command with '>' prefix
- `.terminal__output`: Command result with padding
- `.terminal__input-line`: Active input line
- `.terminal__input`: Command input field

### Status Variants
- `.terminal__line--error`: Error message
- `.terminal__line--warning`: Warning message
- `.terminal__line--success`: Success output
- `.terminal__line--info`: Info message

### Theme Variants
- `.terminal--dark`: Dark theme with reduced opacity
- `.terminal--transparent`: Modern glass effect with blur
- `.terminal--minimal`: No header version
- `.terminal--matrix`: Matrix-style with green glow
- `.terminal--retro`: Pixel-style retro look with bold borders

### Size Variants
- `.terminal--sm`: Small height (200px)
- `.terminal--lg`: Large height (500px)
- `.terminal--xl`: Extra large (700px)
- `.terminal--fullscreen`: Full viewport with z-index

### State Classes
- `.terminal--loading`: Shows blinking cursor animation
- `.terminal--minimal`: Hides the header completely

## Usage Example

```html
<!-- Matrix Theme Terminal -->
<div class="terminal terminal--matrix">
  <div class="terminal__header">
    <div class="terminal__title">
      <svg class="terminal__icon"><!-- terminal icon --></svg>
      Matrix Terminal
    </div>
    <div class="terminal__actions">
      <button class="terminal__action">
        <svg><!-- minimize icon --></svg>
      </button>
      <button class="terminal__action">
        <svg><!-- maximize icon --></svg>
      </button>
      <button class="terminal__action">
        <svg><!-- close icon --></svg>
      </button>
    </div>
  </div>

  <div class="terminal__content">
    <!-- Success Output -->
    <div class="terminal__line terminal__line--success">
      Connection established
    </div>
    
    <!-- Command Line -->
    <div class="terminal__line">
      <span class="terminal__prompt"></span>
      <span class="terminal__command">access mainframe</span>
    </div>
    <div class="terminal__output">Decrypting security protocols...</div>

    <!-- Active Input -->
    <div class="terminal__input-line">
      <span class="terminal__prompt"></span>
      <input class="terminal__input" type="text" placeholder="Enter command...">
    </div>
  </div>
</div>

<!-- Retro Terminal -->
<div class="terminal terminal--retro terminal--lg">
  <!-- Same structure as above -->
</div>
```

## Features
- Multiple themes
- Custom prompt
- Size variants
- Status indicators
- Glass effect
- Loading state
- Custom scrollbar
- Command history
- Active input
- Fullscreen mode

## Theme Details

### Dark Theme
- Background: #1e1e1e
- Reduced opacity (0.9)
- Semi-transparent header

### Glass Effect (Transparent)
- Background with 0.8 opacity
- Backdrop blur effect
- Modern floating appearance

### Matrix Theme
- Black background
- Neon green text (#0f0)
- Text glow effects
- Custom prompt styling

### Retro Theme
- Pixel-style font (VT323)
- Bold borders
- Box shadow effect
- High contrast colors

## Responsive Behavior
- Adapts to viewport on mobile (<640px)
- Adjustable height on smaller screens
- Reduced padding in content area
- Fullscreen option available

## Best Practices
- Choose appropriate theme
- Set custom prompt
- Use status indicators
- Show loading states
- Enable fullscreen
- Handle overflow
- Support keyboard
- Match brand style
- Consider mobile
- Maintain contrast
- Use loading state for operations
- Consider adding keyboard shortcuts
- Implement command history
- Test on mobile devices
- Ensure proper contrast ratios
- Use appropriate theme for context