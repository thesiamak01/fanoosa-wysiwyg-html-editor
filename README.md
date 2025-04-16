# Fanoosa WYSIWYG HTML Editor

A lightweight, RTL-supported WYSIWYG HTML editor with Persian (Farsi) and English language support.

![Editor Screenshot](https://raw.githubusercontent.com/thesiamak01/fanoosa-wysiwyg-html-editor/refs/heads/main/cover.png)

## Features

- **RTL Support**: Fully compatible with right-to-left languages like Persian/Farsi
- **Bilingual UI**: Persian and English language support
- **Customizable Toolbar**: Enable/disable toolbar buttons as needed
- **Responsive Design**: Works on desktop and mobile devices
- **Common Formatting Options**:
    - Text styles (bold, italic, underline, strikethrough)
    - Paragraph formatting (headings, alignment)
    - Lists (ordered/unordered)
    - Links and images
    - Text and background colors
    - HTML source editing

## Installation

Include the necessary files in your HTML:

```html
<link href="fanoosa-wysiwyg-html-editor.min.css" rel="stylesheet">
<script src="fanoosa-wysiwyg-html-editor.min.js"></script>
```
Don't forget to include Bootstrap Icons for the toolbar icons:
```html
<!-- Bootstrap Icons -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">
```
## Usage
Basic initialization:
```html
document.addEventListener('DOMContentLoaded', function() {
    const editor = new FanoosaWysiwygHtmlEditor({
        textareaId: 'myEditor',
        language: 'fa', // or 'en' for English
        toolbarButtons: {
            undoRedo: true,
            formatBlock: true,
            textStyles: true,
            alignment: true,
            lists: true,
            links: true,
            colors: true,
            misc: true
        }
    });
});
```

## Toolbar Buttons Configuration
All toolbar buttons are enabled by default. You can disable specific groups:
```html
toolbarButtons: {
    undoRedo: false,    // Disable undo/redo buttons
    formatBlock: false, // Disable paragraph formatting
    textStyles: false,  // Disable bold/italic/underline
    alignment: false,   // Disable text alignment
    lists: false,       // Disable lists
    links: false,       // Disable links/images
    colors: false,      // Disable color pickers
    misc: false         // Disable other tools
}
```
## Methods
- getContent(): Get the HTML content of the editor


- setContent(html): Set the editor content


- syncTextarea(): Sync editor content with the original textarea

## Browser Support
The editor works in all modern browsers (Chrome, Firefox, Safari, Edge).

## License
MIT License. See LICENSE file for details.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.