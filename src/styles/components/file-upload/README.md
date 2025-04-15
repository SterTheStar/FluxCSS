# File Upload Component

A comprehensive file upload component with drag-and-drop support, file preview, and progress tracking.

## Variables Used

### Core Variables Used
- `--color-bg-secondary`: Upload area background
- `--color-bg-tertiary`: Border and document preview
- `--color-text-primary`: Filename text
- `--color-text-secondary`: Drop zone text
- `--color-text-muted`: Icons and secondary text
- `--color-accent`: Hover border and progress
- `--color-error`: Error states
- `--border-radius-sm`: Preview border radius
- `--border-radius-md`: File item radius
- `--border-radius-lg`: Drop zone radius
- `--border-radius-full`: Progress bar radius
- `--font-size-sm`: Secondary text size
- `--spacing-xs`: Small gaps
- `--spacing-sm`: Default gaps
- `--spacing-md`: Medium spacing
- `--spacing-lg`: Mobile padding
- `--spacing-xl`: Drop zone padding
- `--transition-fast`: Hover animations

## Classes

### Base Classes
- `.file-upload`: Main container
- `.file-upload__dropzone`: Drag-and-drop area
- `.file-upload__icon`: Upload icon
- `.file-upload__text`: Instruction text
- `.file-upload__browse`: Browse button

### File List
- `.file-upload__list`: Files container
- `.file-upload__item`: Individual file
- `.file-upload__preview`: File thumbnail
- `.file-upload__info`: File details
- `.file-upload__filename`: File name
- `.file-upload__size`: File size
- `.file-upload__actions`: Action buttons

### Progress
- `.file-upload__progress`: Progress container
- `.file-upload__progress-bar`: Progress indicator

### States
- `.is-dragging`: Active drop state
- `.file-upload__item--error`: Error state
- `.file-upload__preview--document`: Document icon

## Usage Example

```html
<div class="file-upload">
  <!-- Drop Zone -->
  <div class="file-upload__dropzone">
    <svg class="file-upload__icon"><!-- upload icon --></svg>
    <p class="file-upload__text">
      Drag and drop files here or
      <a href="#" class="file-upload__browse">browse</a>
    </p>
    <p class="file-upload__restrictions">
      Maximum file size: 10MB
    </p>
  </div>

  <!-- File List -->
  <div class="file-upload__list">
    <!-- File Item -->
    <div class="file-upload__item">
      <div class="file-upload__preview">
        <img src="preview.jpg" alt="File preview">
      </div>
      
      <div class="file-upload__info">
        <div class="file-upload__filename">document.pdf</div>
        <div class="file-upload__size">2.5 MB</div>
        
        <div class="file-upload__progress">
          <div class="file-upload__progress-bar" style="width: 70%"></div>
        </div>
      </div>

      <div class="file-upload__actions">
        <button class="file-upload__remove">×</button>
      </div>
    </div>
  </div>
</div>
```

## Features
- Drag and drop support
- File preview thumbnails
- Upload progress tracking
- Error state handling
- File size display
- Remove functionality
- Multiple file support
- File restrictions
- Responsive design
- Browse button option

## Interactions
- Drag enter/leave effects
- Hover state feedback
- Progress animation
- Remove confirmation
- Error highlighting
- Browse trigger

## Responsive Behavior
- Stack layout on mobile
- Full-width previews
- Adjusted spacing
- Touch-friendly targets
- Maintains usability

## Best Practices
- Show file restrictions
- Provide clear feedback
- Include progress indication
- Handle errors gracefully
- Support keyboard interaction
- Enable file removal
- Show file previews
- Display file sizes
- Validate file types
- Maintain accessibility