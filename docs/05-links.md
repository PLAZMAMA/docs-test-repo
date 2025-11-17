# Links Documentation

This document demonstrates various ways to create and use links in Markdown.

## Basic Links

### Inline Links

[Google](https://www.google.com)

[GitHub](https://github.com)

[Example Website](https://example.com)

### Links with Titles

[Google](https://www.google.com "Go to Google")

[GitHub](https://github.com "Visit GitHub")

[Example](https://example.com "Example Website Tooltip")

## Reference-Style Links

Here's a link to [Google][google-link].

Here's another link to [GitHub][github-link].

And one more to [Example][example-link].

[google-link]: https://www.google.com
[github-link]: https://github.com
[example-link]: https://example.com

## Implicit Reference Links

You can also use [Google][] or [GitHub][] style.

[Google]: https://www.google.com
[GitHub]: https://github.com

## URLs and Email Addresses

### Auto-linking

<https://www.example.com>

<https://github.com/user/repo>

<mailto:email@example.com>

### Plain URLs (GitHub Flavored Markdown)

https://www.github.com

www.example.com

## Internal Links

### Linking to Headers

[Jump to Basic Links](#basic-links)

[Go to Reference-Style Links](#reference-style-links)

[See Complex Links section](#complex-link-scenarios)

### Relative Links to Files

[See Tables Documentation](./01-tables.md)

[Check Images Guide](./02-images.md)

[Read Text Formatting](./03-text-formatting.md)

[View Code Examples](./04-code-blocks.md)

## Anchor Links

Jump to [Section 1](#section-1)

Jump to [Section 2](#section-2)

Jump to [Section 3](#section-3)

### Section 1

Content for section 1.

### Section 2

Content for section 2.

### Section 3

Content for section 3.

## Links in Lists

### Unordered List with Links

* [First Link](https://example.com/1)
* [Second Link](https://example.com/2)
* [Third Link](https://example.com/3)
  * [Nested Link](https://example.com/3a)
  * [Another Nested](https://example.com/3b)

### Ordered List with Links

1. [Getting Started](https://docs.example.com/start)
2. [Installation](https://docs.example.com/install)
3. [Configuration](https://docs.example.com/config)
4. [Advanced Topics](https://docs.example.com/advanced)

## Links in Tables

| Resource | Link |
|----------|------|
| Documentation | [Docs](https://docs.example.com) |
| API Reference | [API](https://api.example.com) |
| GitHub Repo | [Code](https://github.com/example/repo) |
| Support | [Help](https://support.example.com) |

## Links with Images

### Linked Image

[![Click me](https://via.placeholder.com/200x100/007bff/ffffff?text=Click+Here)](https://example.com)

### Multiple Linked Images

[![Logo 1](https://via.placeholder.com/100x100/ff6600/ffffff?text=1)](https://example.com/1)
[![Logo 2](https://via.placeholder.com/100x100/00cc66/ffffff?text=2)](https://example.com/2)
[![Logo 3](https://via.placeholder.com/100x100/cc0066/ffffff?text=3)](https://example.com/3)

## Footnote Links

Here's a sentence with a footnote[^1].

Another sentence with a different footnote[^2].

Multiple references to the same footnote[^1].

[^1]: This is the first footnote.
[^2]: This is the second footnote with more detail.

## Complex Link Scenarios

### Link with Special Characters

[Link with "quotes" and 'apostrophes'](https://example.com/special)

[Link with (parentheses)](https://example.com/parens)

[Link with & ampersand](https://example.com/ampersand)

### Long URLs

[Very long URL example](https://example.com/very/long/path/to/resource/with/many/segments/and/parameters?param1=value1&param2=value2&param3=value3)

### Links in Blockquotes

> This quote contains a [link to example](https://example.com).
> 
> And another [link to documentation](https://docs.example.com).

### Links in Code

In inline code: `[link text](url)` is the syntax.

In a code block:

```markdown
[Example Link](https://example.com)
```

### Escaped Links

\[This is not a link\](https://example.com)

This has escaped brackets: \[text\] but this is a [real link](https://example.com)

## File Protocol Links

[Local File](file:///C:/Users/Documents/file.txt)

[Unix Path](file:///home/user/document.pdf)

## Fragment Links

[Link to specific section](https://example.com/page#section-name)

[GitHub Issue](https://github.com/user/repo/issues/123#issuecomment-456)

## Query Parameter Links

[Search Results](https://example.com/search?q=markdown&sort=date&filter=all)

[API Endpoint](https://api.example.com/v1/users?page=2&limit=50)

## Protocol-Relative URLs

[Protocol Relative](//example.com/resource)

## Link Formatting

**Bold link:** **[Google](https://www.google.com)**

*Italic link:* *[GitHub](https://github.com)*

***Bold and italic:*** ***[Example](https://example.com)***

~~Strikethrough link:~~ ~~[Deprecated](https://old.example.com)~~

## Multiple Links in Paragraph

You can combine multiple links in a paragraph like [Google](https://google.com), [GitHub](https://github.com), and [Example](https://example.com) together seamlessly.

## Broken Link Examples

[Broken Link](https://this-domain-does-not-exist-12345.com)

[Invalid URL](#nonexistent-section)

## Links in Different Contexts

### In Emphasis

This is *emphasized text with a [link](https://example.com) inside*.

This is **bold text with a [link](https://example.com) inside**.

### In Lists with Descriptions

* **[API Documentation](https://api.example.com)** - Complete API reference
* **[User Guide](https://guide.example.com)** - Step-by-step tutorials
* **[FAQ](https://faq.example.com)** - Frequently asked questions

### Nested in Task Lists

- [x] Review [documentation](https://docs.example.com)
- [ ] Check [examples](https://examples.example.com)
- [ ] Read [API guide](https://api.example.com)

## Reference Links with Numbers

Here's link [1][1] and link [2][2].

[1]: https://example.com/first
[2]: https://example.com/second

## Links with HTML

<a href="https://example.com" target="_blank">Open in new tab</a>

<a href="https://example.com" title="Example Site">HTML Link with Title</a>

## Social Media Links

[Twitter](https://twitter.com/username)

[LinkedIn](https://linkedin.com/in/username)

[Facebook](https://facebook.com/username)

[Instagram](https://instagram.com/username)

[YouTube](https://youtube.com/channel/channelid)

## Repository Links

[Repository](https://github.com/user/repo)

[Issues](https://github.com/user/repo/issues)

[Pull Requests](https://github.com/user/repo/pulls)

[Releases](https://github.com/user/repo/releases)

[Wiki](https://github.com/user/repo/wiki)

## Documentation Links

[Introduction](https://docs.example.com/intro)

[Getting Started](https://docs.example.com/getting-started)

[API Reference](https://docs.example.com/api)

[Examples](https://docs.example.com/examples)

[Troubleshooting](https://docs.example.com/troubleshooting)

---

**Note**: Not all link types work in all markdown renderers. Test your specific renderer to ensure compatibility.
