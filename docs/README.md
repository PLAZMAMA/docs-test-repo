# Markdown Stress Test Documentation Suite

A comprehensive collection of markdown files designed to test and stress-test markdown rendering engines, parsers, and tools.

## 🎯 Overview

This documentation suite contains **10 markdown files** with extensive examples of markdown features, edge cases, and stress tests. It's perfect for:

- **Testing** markdown parsers and renderers
- **Validating** markdown tool implementations
- **Learning** markdown syntax and capabilities
- **Benchmarking** rendering performance
- **Quality assurance** for documentation platforms

## 📂 Files Included

| File | Description | Features |
|------|-------------|----------|
| [00-index.md](./00-index.md) | Main index and overview | Navigation, feature matrix, testing guide |
| [01-tables.md](./01-tables.md) | Table demonstrations | Simple, aligned, complex, nested, Unicode tables |
| [02-images.md](./02-images.md) | Image examples | Inline, reference, linked, base64, various formats |
| [03-text-formatting.md](./03-text-formatting.md) | Text formatting | Headers, emphasis, lists, Unicode, emoji |
| [04-code-blocks.md](./04-code-blocks.md) | Code examples | 15+ languages, inline code, syntax highlighting |
| [05-links.md](./05-links.md) | Link types | Internal, external, reference, anchors, footnotes |
| [06-blockquotes.md](./06-blockquotes.md) | Blockquotes | Nested, with elements, styled, collapsible |
| [07-github-features.md](./07-github-features.md) | GitHub-specific | Task lists, emoji, Mermaid diagrams, alerts, LaTeX |
| [08-html-elements.md](./08-html-elements.md) | HTML in markdown | Forms, tables, media, SVG, mixed HTML/MD |
| [09-edge-cases.md](./09-edge-cases.md) | Edge cases | Malformed syntax, extremes, performance tests |

## 🚀 Quick Start

### View All Documentation

Start with the [index file](./00-index.md) for a complete overview and navigation.

### Test a Specific Feature

Jump directly to the relevant file:

```bash
# Test tables
open 01-tables.md

# Test code syntax highlighting
open 04-code-blocks.md

# Test GitHub features
open 07-github-features.md
```

### Run Automated Tests

Use these files as input for your markdown renderer tests:

```bash
# Example with a markdown CLI tool
markdown-tool render 01-tables.md > output.html

# Example with a parser
node test-parser.js docs/*.md
```

## 📊 Feature Coverage

### ✅ Standard Markdown (CommonMark)

- [x] Headers (ATX and Setext style)
- [x] Paragraphs and line breaks
- [x] Emphasis (bold, italic)
- [x] Lists (ordered, unordered, nested)
- [x] Links (inline, reference, automatic)
- [x] Images
- [x] Code (inline and fenced blocks)
- [x] Blockquotes
- [x] Horizontal rules
- [x] Escaping

### ✅ Extended Syntax

- [x] Tables
- [x] Fenced code blocks with syntax highlighting
- [x] Strikethrough
- [x] Task lists
- [x] Automatic URL linking
- [x] Emoji (shortcodes and Unicode)
- [x] Footnotes
- [x] Definition lists
- [x] Abbreviations

### ✅ GitHub-Flavored Markdown

- [x] Task lists with checkboxes
- [x] Emoji shortcodes (:smile:)
- [x] @mentions
- [x] Issue/PR references (#123)
- [x] Commit references (SHA)
- [x] Strikethrough (~~text~~)
- [x] Tables
- [x] Automatic linking
- [x] Mermaid diagrams
- [x] Alerts/callouts
- [x] Mathematical expressions (LaTeX)

### ✅ HTML Elements

- [x] Text formatting tags
- [x] Lists and tables
- [x] Forms and inputs
- [x] Media (audio, video, iframe)
- [x] SVG and canvas
- [x] Details/summary (collapsible)
- [x] Semantic HTML5 elements

### ✅ Advanced Features

- [x] Nested structures (5+ levels)
- [x] Unicode characters
- [x] Special characters
- [x] Long content (performance)
- [x] Edge cases and malformed syntax
- [x] Mixed HTML and Markdown

## 🧪 Test Scenarios

### 1. Feature Completeness

Test if your renderer supports all standard and extended markdown features.

```bash
# Check each file for proper rendering
for file in *.md; do
    echo "Testing $file"
    your-renderer "$file"
done
```

### 2. Performance Testing

Measure rendering time for documents with different characteristics:

- **01-tables.md**: Large tables
- **04-code-blocks.md**: Many code blocks
- **09-edge-cases.md**: Extreme nesting and long lines

### 3. Edge Case Handling

Test robustness with malformed or unusual markdown:

- Empty elements
- Unclosed tags
- Deeply nested structures
- Very long lines
- Special character sequences

### 4. Compatibility Testing

Compare output across different renderers:

- GitHub
- GitLab
- Static site generators (Jekyll, Hugo, etc.)
- Documentation platforms (Read the Docs, GitBook, etc.)
- IDE markdown previewers (VS Code, etc.)

## 💻 Usage Examples

### As Test Input

```python
# Python example
import markdown

with open('docs/01-tables.md', 'r') as f:
    content = f.read()
    html = markdown.markdown(content, extensions=['tables', 'fenced_code'])
    print(html)
```

```javascript
// JavaScript example
const fs = require('fs');
const marked = require('marked');

const content = fs.readFileSync('docs/02-images.md', 'utf8');
const html = marked.parse(content);
console.log(html);
```

### For Documentation

Include these files in your documentation project to test rendering:

```yaml
# mkdocs.yml example
nav:
  - Home: index.md
  - Tests:
    - Tables: 01-tables.md
    - Images: 02-images.md
    - Code: 04-code-blocks.md
```

### For Benchmarking

```bash
# Measure rendering time
time markdown-tool render 09-edge-cases.md

# Compare multiple renderers
for renderer in pandoc markdown-it marked; do
    echo "Testing $renderer"
    time $renderer 04-code-blocks.md
done
```

## 📈 Expected Results

### Rendering

All features should render correctly without:

- Layout breaks
- Escaped characters visible
- Missing images or links
- Broken tables
- Syntax highlighting failures

### Performance

Reasonable rendering times:

- Small files (< 5KB): < 10ms
- Medium files (5-10KB): < 50ms
- Large files (> 10KB): < 100ms

### Compatibility

Consistent rendering across:

- Desktop browsers
- Mobile devices
- Different markdown renderers
- Light and dark themes

## 🐛 Known Issues

Some features may not work in all environments:

- **Mermaid diagrams**: Require JavaScript support
- **LaTeX math**: Require specific renderer support
- **HTML elements**: May be sanitized for security
- **Base64 images**: May have size limits
- **Emoji shortcodes**: Renderer-specific

## 🤝 Contributing

Found an edge case we missed? Want to add more tests?

1. Add examples to existing files
2. Create new test files for specific features
3. Document expected vs actual behavior
4. Share your test results

## 📝 Test Results Template

Document your test results:

```markdown
## Test Results

**Renderer**: [Name and Version]
**Date**: [YYYY-MM-DD]
**Platform**: [OS/Browser]

### Feature Support
- Tables: ✅ / ⚠️ / ❌
- Images: ✅ / ⚠️ / ❌
- Code Highlighting: ✅ / ⚠️ / ❌
- GitHub Features: ✅ / ⚠️ / ❌
- HTML Elements: ✅ / ⚠️ / ❌

### Performance
- Average render time: XXms
- Largest file render time: XXms
- Memory usage: XXMB

### Issues Found
1. [Description of issue]
2. [Description of issue]

### Notes
[Any additional observations]
```

## 🔗 Resources

### Specifications

- [CommonMark Spec](https://commonmark.org/)
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Markdown Guide](https://www.markdownguide.org/)

### Tools

- **Parsers**: marked, markdown-it, commonmark.js
- **Renderers**: Pandoc, kramdown, goldmark
- **Validators**: markdownlint, remark-lint
- **Editors**: Typora, MarkText, VS Code

### Testing Frameworks

- [Markdown Test Suite](https://github.com/karlcow/markdown-testsuite)
- [CommonMark Test Suite](https://github.com/commonmark/commonmark-spec)

## 📊 Statistics

- **Total Files**: 10
- **Total Lines**: ~2000+
- **Total Characters**: ~80,000+
- **Code Examples**: 30+ languages
- **Tables**: 50+ examples
- **Images**: 100+ references
- **Links**: 200+ examples

## 📄 License

MIT License - Feel free to use these files for testing, learning, or any other purpose.

## 🙏 Acknowledgments

Created for the markdown community to help improve tools and ensure compatibility across platforms.

---

**Last Updated**: January 2024

**Version**: 1.0.0

**Repository**: [PLAZMAMA/docs-test-repo](https://github.com/PLAZMAMA/docs-test-repo)

---

Happy Testing! 🚀
