<!---
title: Kaveh - Markdown Website Generator
description: A simple, powerful static site generator built with pure POSIX shell that converts Markdown to HTML
--->

# Kaveh - Markdown Website Generator

Kaveh is a **lightweight** and *powerful* static site generator written entirely in pure POSIX shell. It transforms your Markdown files into beautiful, responsive HTML pages without any external dependencies. This page showcases all the markdown features Kaveh supports, demonstrating how you can create rich content with simple, readable syntax.

## Rich Text Formatting

Kaveh supports comprehensive text formatting options to make your content expressive and readable.

### Bold Text

Emphasize important content with **bold text** using `**text**` or `__text__`.

- **This is bold with asterisks**
- __This is bold with underscores__

### Italic Text

Add subtle emphasis with *italic text* using `*text*` or `_text_`.

- *This is italic with asterisks*
- _This is italic with underscores_

### Combined Formatting

You can combine formatting styles: ***bold and italic*** using `***text***` or `___text___`.

### Strikethrough

Mark text as removed or outdated with ~~strikethrough~~ using `~~text~~`.

### Inline Code

Highlight code snippets inline with `backticks` like this: `const x = 42;`

### Highlighted Text

Draw attention to important passages with ==highlighted text== using `==text==`.

### Scientific Notation

Kaveh supports subscript and superscript for scientific and mathematical expressions:

- Chemical formulas: H~2~O using `H~2~O`
- Mathematical equations: E=mc^2^ using `E=mc^2^`

## Links and Media

Create hyperlinks and embed images effortlessly in your Kaveh-powered site.

### Hyperlinks

Link to external sites, pages, or email addresses with the syntax `[text](url)`:

- External link: [Visit GitHub](https://github.com)
- Email link: [Contact us](mailto:example@example.com)
- Internal link: [Jump to headings](#headings)

### Images

Embed images using `![alt text](image-url)` syntax:

![Sample Image](https://raw.githubusercontent.com/MahdiMirzadeh/kaveh/refs/heads/master/iran.webp)

### Clickable Images

Combine links and images to create clickable graphics: `[![alt](image-url)](link-url)`

[![Clickable Image](https://raw.githubusercontent.com/MahdiMirzadeh/kaveh/refs/heads/master/iran.webp)](https://example.com)

## Organizing Content with Lists

Kaveh provides flexible list formatting to structure your content clearly.

### Bullet Lists

Create unordered lists with `-`, `*`, or `+`:

- Documentation pages
- Blog posts
  - Technical tutorials
  - Release notes
- Project notes

### Numbered Lists

Ordered lists use numbers followed by periods:

1. Install Kaveh
2. Create markdown files
3. Generate your site
   1. Run the converter
   2. Deploy the output

### Task Lists

Track progress with interactive checkboxes using `- [ ]` and `- [x]`:

- [x] Set up Kaveh
- [x] Write content
- [ ] Deploy website
  - [x] Configure server
  - [ ] Set up domain

### Flexible List Mixing

Combine different list styles as needed:

1. Plan your website structure
2. Write content in Markdown
   - Create pages
   - Add images and links
3. Generate with Kaveh

## Code Highlighting

Kaveh excels at displaying code with fenced code blocks and syntax highlighting.

### Multi-Language Support

Use triple backticks with language identifiers:

```bash
#!/bin/sh
echo "Hello, World!"
```

```python
def hello():
    print("Hello from Python!")
```

```javascript
const greeting = () => {
    console.log('Hello from JavaScript!');
};
```

```c
#include <stdio.h>

int main() {
    printf("Hello from C!\n");
    return 0;
}
```

## Blockquotes and Callouts

Highlight important information or quotations with blockquotes using `>`:

> Kaveh generates clean, semantic HTML from your Markdown files.
> No JavaScript frameworks or build tools required.

> **Tip**: Blockquotes are perfect for tips, warnings, or highlighting key points.

> Blockquotes support **formatting**, *emphasis*, and `inline code`.

## Data Tables

Present structured data beautifully with Markdown tables using pipes `|` and hyphens `-`:

| Name    | Age | City      |
|---------|-----|----------|
| John    | 25  | NYC      |
| Jane    | 30  | LA       |
| Bob     | 35  | Chicago  |

### Formatted Tables

Tables fully support inline formatting to make data more readable:

| Feature         | Status | Syntax                   |
|-----------------|--------|-------------------------|
| **Bold**        | ✓      | `**text**`              |
| *Italic*        | ✓      | `*text*`                |
| `Code`          | ✓      | `` `code` ``            |
| ~~Strike~~      | ✓      | `~~text~~`              |

## Visual Separators

Divide content sections with horizontal rules using three or more hyphens, asterisks, or underscores:

---

Content above the separator.

***

Content between separators.

___

## Headings with Auto-Generated Anchors {#headings}

Kaveh automatically generates anchor links for all headings (H1 through H6), making it easy to create a table of contents or link to specific sections:

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

### Custom Heading IDs

You can add custom IDs to headings:

## Custom Heading Example {#my-custom-id}

You can also provide custom IDs using the syntax `{#custom-id}`. [Click here to jump back](#headings)

## Advanced Features

### Footnotes and References

Add scholarly footnotes[^1] to provide additional context. They automatically appear at the bottom[^2] of the page with return links.

[^1]: Footnotes are perfect for citations, additional explanations, or references.
[^2]: Kaveh automatically numbers and links footnotes for you.

Example syntax:
```
Add footnotes[^1] to your text.

[^1]: This is a footnote definition.
```

### Definition Lists

Create glossaries or define terms with definition lists:

Static Site Generator
: A tool that generates a complete static website from source files

Markdown
: A lightweight markup language with plain text formatting syntax

### Manual Line Breaks

End any line with two or more spaces to insert a line break.  
The text continues on a new line without starting a new paragraph.

## HTML Passthrough

When you need more control, Kaveh passes raw HTML directly to the output:

<div style="padding: 10px; border: 2px solid #0066cc; border-radius: 5px;">
This <strong>custom HTML</strong> is rendered exactly as written.
</div>

Example:
```html
<div style="padding: 10px; border: 2px solid #0066cc;">
Custom HTML content here.
</div>
```

## Escaping Special Characters

Use backslashes to display Markdown syntax literally:

- \* This won't be italic \*
- \_ This won't be italic \_
- \` This won't be code \`
- \[ This won't be a link \]
- \# This won't be a heading

## Why Choose Kaveh?

Kaveh brings simplicity and power together for static site generation:

- ✓ **Zero Dependencies** - Pure POSIX shell script
- ✓ **Fast** - Instant compilation, no build tools
- ✓ **Complete** - Full Markdown support with extensions
- ✓ **Semantic HTML** - Clean, accessible output
- ✓ **Dark Mode** - Built-in responsive dark theme
- ✓ **Portable** - Runs on any POSIX-compliant system

### Supported Features

- Rich text formatting (bold, italic, strikethrough, highlight)
- Headings (H1-H6) with automatic anchor generation
- Links, images, and clickable images
- Lists (bullet, numbered, task lists, nested)
- Syntax-highlighted code blocks
- Tables with formatting support
- Blockquotes and callouts
- Footnotes with auto-linking
- Definition lists
- Scientific notation (subscript/superscript)
- Raw HTML passthrough
- Character escaping
- Horizontal rules

