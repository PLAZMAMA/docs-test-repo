# Blockquotes and Special Containers

This document demonstrates various blockquote styles and special container formats in Markdown.

## Basic Blockquotes

### Simple Blockquote

> This is a simple blockquote.

> This is another blockquote on a separate line.

### Multi-line Blockquote

> This is a multi-line blockquote.
> It continues on the second line.
> And even has a third line.

### Blockquote with Multiple Paragraphs

> This is the first paragraph in a blockquote.
>
> This is the second paragraph in the same blockquote.
>
> And here's a third paragraph.

## Nested Blockquotes

### Single Level Nesting

> This is the outer blockquote.
>
> > This is a nested blockquote.
>
> Back to the outer level.

### Multiple Level Nesting

> Level 1 blockquote
>
> > Level 2 blockquote
> >
> > > Level 3 blockquote
> > >
> > > > Level 4 blockquote
> > > >
> > > > Going deep!
> > >
> > > Back to level 3
> >
> > Back to level 2
>
> Back to level 1

## Blockquotes with Other Elements

### Blockquote with Headers

> ## Header in Blockquote
>
> ### Subheader in Blockquote
>
> Content under the headers.

### Blockquote with Lists

> Unordered list in blockquote:
>
> * Item 1
> * Item 2
> * Item 3

> Ordered list in blockquote:
>
> 1. First item
> 2. Second item
> 3. Third item

### Blockquote with Code

> Here's some inline code: `const x = 42;`
>
> And a code block:
>
> ```javascript
> function example() {
>     return "Hello from blockquote";
> }
> ```

### Blockquote with Links

> Check out [this link](https://example.com) for more information.
>
> Also see [this documentation](https://docs.example.com).

### Blockquote with Images

> Here's an image in a blockquote:
>
> ![Example Image](https://placehold.co/300x150/666666/ffffff?text=Blockquote+Image)

### Blockquote with Tables

> | Column 1 | Column 2 |
> |----------|----------|
> | Data 1   | Data 2   |
> | Data 3   | Data 4   |

## Formatting in Blockquotes

### Bold and Italic

> This text is **bold**.
>
> This text is *italic*.
>
> This text is ***bold and italic***.

### Strikethrough

> This is ~~struck through~~ text.

### Mixed Formatting

> **Important:** This is a *critical* message with ~~outdated~~ information.
>
> Please review the `configuration` settings carefully.

## Blockquote Styles

### Warning Quote

> ⚠️ **Warning:** This is a warning message.
>
> Proceed with caution.

### Info Quote

> ℹ️ **Info:** This is an informational message.
>
> Additional details are available in the documentation.

### Success Quote

> ✅ **Success:** Operation completed successfully.
>
> All tests passed.

### Error Quote

> ❌ **Error:** Something went wrong.
>
> Please check the logs for details.

### Note Quote

> 📝 **Note:** This is an important note.
>
> Keep this in mind for future reference.

### Tip Quote

> 💡 **Tip:** Here's a helpful suggestion.
>
> This can save you time.

## Long Blockquotes

> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
>
> Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Blockquotes with Attribution

> "The only way to do great work is to love what you do."
>
> — Steve Jobs

> "In the middle of difficulty lies opportunity."
>
> — Albert Einstein

> "Life is what happens when you're busy making other plans."
>
> — John Lennon

## Complex Nested Structures

### Blockquote with List and Nested Blockquote

> Main point:
>
> * First item
>   > Note about first item
> * Second item
>   > Note about second item
>   >
>   > Additional details
> * Third item

### Multiple Elements Combined

> ## Documentation Update
>
> **Version:** 2.0.0
>
> **Release Date:** 2024-01-15
>
> ### Changes:
>
> 1. Added new features
>    * Feature A
>    * Feature B
> 2. Fixed bugs
>    * Bug #123
>    * Bug #456
>
> ### Migration Guide:
>
> > **Important:** Follow these steps carefully:
> >
> > 1. Backup your data
> > 2. Run migration script
> > 3. Verify results
>
> For more information, see the [migration guide](https://docs.example.com/migration).

## Horizontal Rules in and Around Blockquotes

Before blockquote

---

> Blockquote content

---

After blockquote

> Content before rule
>
> ---
>
> Content after rule

## Empty Blockquotes

>

> 

This tests how renderers handle empty blockquotes.

## Blockquote Followed by Other Elements

> This is a blockquote.

Followed by a regular paragraph.

* Followed by a list item
* Another list item

## Consecutive Blockquotes

> First blockquote.

> Second blockquote.

> Third blockquote.

## Alert Callouts (GitHub-style)

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

## HTML Blockquotes

<blockquote>
  <p>This is an HTML blockquote.</p>
  <p>It can contain multiple paragraphs.</p>
</blockquote>

<blockquote cite="https://example.com">
  <p>Blockquote with citation attribute.</p>
  <footer>— Source: <cite>Example</cite></footer>
</blockquote>

## Details and Summary (Collapsible Sections)

<details>
<summary>Click to expand</summary>

This content is hidden by default and can be expanded by clicking the summary.

It can contain:

* Lists
* **Formatted text**
* `Code`
* [Links](https://example.com)

</details>

<details>
<summary>Nested Example</summary>

Outer content

<details>
<summary>Inner collapsible</summary>

Inner content that's doubly nested.

</details>

</details>

## Aside and Figure

<aside>
This is an aside element with supplementary information.
</aside>

<figure>
  <img src="https://placehold.co/300x200/444444/ffffff?text=Figure+Image" alt="Figure image">
  <figcaption>Figure caption describing the image above.</figcaption>
</figure>

## Blockquote Best Practices

> ### Do's
>
> * Keep quotes relevant
> * Attribute sources
> * Format consistently
>
> ### Don'ts
>
> * Don't overuse blockquotes
> * Don't nest too deeply
> * Don't use for regular content

---

**Note**: Different markdown renderers may display blockquotes with different styling. Test your specific renderer for best results.
