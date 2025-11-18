# HTML Elements in Markdown

This document demonstrates the use of HTML elements within Markdown documents.

## Text Formatting

### Basic HTML Tags

<b>Bold text using HTML</b>

<i>Italic text using HTML</i>

<u>Underlined text</u>

<s>Strikethrough text using HTML</s>

<strong>Strong text</strong>

<em>Emphasized text</em>

<small>Small text</small>

<big>Big text</big>

<mark>Highlighted text</mark>

<del>Deleted text</del>

<ins>Inserted text</ins>

### Subscript and Superscript

H<sub>2</sub>O is water

E = mc<sup>2</sup> is Einstein's equation

The formula is x<sup>2</sup> + y<sup>2</sup> = r<sup>2</sup>

Chemical formula: CH<sub>3</sub>COOH

## Text Styling

### Font and Span

<font color="red">Red text</font>

<font color="#0066cc">Blue text with hex color</font>

<font size="5">Large text</font>

<span style="color: green; font-weight: bold;">Styled span element</span>

<span style="background-color: yellow; padding: 5px;">Highlighted span</span>

### Text Alignment

<div align="left">This text is left-aligned</div>

<div align="center">This text is center-aligned</div>

<div align="right">This text is right-aligned</div>

<div align="justify">This text is justified. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>

## Headings

<h1>HTML H1 Heading</h1>

<h2>HTML H2 Heading</h2>

<h3>HTML H3 Heading</h3>

<h4>HTML H4 Heading</h4>

<h5>HTML H5 Heading</h5>

<h6>HTML H6 Heading</h6>

## Horizontal Rules

<hr>

<hr style="border: 2px solid #000;">

<hr style="border: 1px dashed #666;">

## Line Breaks

This line has a break<br>here.

Multiple<br>line<br>breaks<br>in<br>sequence.

## Preformatted Text

<pre>
Preformatted text
    preserves    spaces
        and line breaks
            exactly as written
</pre>

<pre style="background-color: #f4f4f4; padding: 10px; border: 1px solid #ddd;">
Styled preformatted text
With background and border
</pre>

## Code Elements

<code>inline code element</code>

<kbd>Ctrl</kbd> + <kbd>C</kbd>

<var>variable</var>

<samp>sample output</samp>

## Lists

### Unordered List

<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ul>

### Ordered List

<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>

### Styled Lists

<ul style="list-style-type: square;">
  <li>Square bullets</li>
  <li>Another item</li>
</ul>

<ol type="A">
  <li>Item A</li>
  <li>Item B</li>
  <li>Item C</li>
</ol>

<ol type="I">
  <li>Item I</li>
  <li>Item II</li>
  <li>Item III</li>
</ol>

### Definition List

<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
  
  <dt>JavaScript</dt>
  <dd>A programming language for the web</dd>
</dl>

## Links

<a href="https://example.com">HTML link</a>

<a href="https://example.com" target="_blank">Link opening in new tab</a>

<a href="https://example.com" title="Example Website">Link with title</a>

<a href="#top">Link to anchor</a>

<a href="mailto:email@example.com">Email link</a>

## Images

<img src="https://placehold.co/300x150/007bff/ffffff?text=HTML+Image" alt="HTML Image">

<img src="https://placehold.co/200x200" alt="Image" width="100" height="100">

<img src="https://placehold.co/400x200" alt="Styled" style="border: 2px solid #333; border-radius: 10px;">

## Figures and Captions

<figure>
  <img src="https://placehold.co/400x250/666666/ffffff?text=Figure+Example" alt="Figure">
  <figcaption>This is a figure caption</figcaption>
</figure>

<figure style="text-align: center;">
  <img src="https://placehold.co/300x200/444444/ffffff?text=Centered" alt="Centered">
  <figcaption style="font-style: italic;">Centered figure with styled caption</figcaption>
</figure>

## Tables

### Basic HTML Table

<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
    <th>Header 3</th>
  </tr>
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
    <td>Cell 3</td>
  </tr>
  <tr>
    <td>Cell 4</td>
    <td>Cell 5</td>
    <td>Cell 6</td>
  </tr>
</table>

### Styled Table

<table style="border-collapse: collapse; width: 100%;">
  <tr style="background-color: #f2f2f2;">
    <th style="border: 1px solid #ddd; padding: 8px;">Name</th>
    <th style="border: 1px solid #ddd; padding: 8px;">Age</th>
    <th style="border: 1px solid #ddd; padding: 8px;">City</th>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px;">John</td>
    <td style="border: 1px solid #ddd; padding: 8px;">30</td>
    <td style="border: 1px solid #ddd; padding: 8px;">New York</td>
  </tr>
  <tr style="background-color: #f9f9f9;">
    <td style="border: 1px solid #ddd; padding: 8px;">Jane</td>
    <td style="border: 1px solid #ddd; padding: 8px;">25</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Los Angeles</td>
  </tr>
</table>

### Table with Colspan and Rowspan

<table border="1">
  <tr>
    <th>Header 1</th>
    <th colspan="2">Merged Header</th>
  </tr>
  <tr>
    <td rowspan="2">Merged Cell</td>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
  <tr>
    <td>Cell 3</td>
    <td>Cell 4</td>
  </tr>
</table>

## Blockquotes

<blockquote>
  This is an HTML blockquote.
</blockquote>

<blockquote cite="https://example.com">
  <p>Blockquote with citation.</p>
  <footer>— Source: <cite>Example Source</cite></footer>
</blockquote>

## Divisions and Sections

<div style="background-color: #e7f3ff; padding: 20px; border-left: 5px solid #2196F3;">
  <h3>Info Box</h3>
  <p>This is an information box created with a div.</p>
</div>

<div style="background-color: #fff3cd; padding: 20px; border-left: 5px solid #ffc107; margin-top: 20px;">
  <h3>Warning Box</h3>
  <p>This is a warning box with custom styling.</p>
</div>

<section style="border: 2px solid #ccc; padding: 15px; margin: 10px 0;">
  <h3>Section Element</h3>
  <p>Content within a section element.</p>
</section>

## Details and Summary

<details>
  <summary>Click to expand</summary>
  <p>This content is hidden by default.</p>
  <p>It can contain multiple paragraphs.</p>
</details>

<details open>
  <summary>Expanded by default</summary>
  <p>This details element is open by default.</p>
</details>

<details>
  <summary><strong>Nested Details</strong></summary>
  <p>Outer content</p>
  <details>
    <summary>Inner details</summary>
    <p>Inner content</p>
  </details>
</details>

## Forms

<form>
  <label for="name">Name:</label><br>
  <input type="text" id="name" name="name" placeholder="Enter your name"><br><br>
  
  <label for="email">Email:</label><br>
  <input type="email" id="email" name="email" placeholder="Enter your email"><br><br>
  
  <label for="message">Message:</label><br>
  <textarea id="message" name="message" rows="4" cols="50"></textarea><br><br>
  
  <input type="checkbox" id="agree" name="agree">
  <label for="agree">I agree to the terms</label><br><br>
  
  <input type="radio" id="option1" name="options" value="1">
  <label for="option1">Option 1</label><br>
  <input type="radio" id="option2" name="options" value="2">
  <label for="option2">Option 2</label><br><br>
  
  <select name="country" id="country">
    <option value="usa">USA</option>
    <option value="uk">UK</option>
    <option value="canada">Canada</option>
  </select><br><br>
  
  <button type="submit">Submit</button>
</form>

## Buttons

<button>Default Button</button>

<button style="background-color: #4CAF50; color: white; padding: 10px 20px; border: none; cursor: pointer;">
  Styled Button
</button>

## Progress and Meter

<label for="progress">Progress:</label>
<progress id="progress" value="70" max="100">70%</progress>

<label for="meter">Meter:</label>
<meter id="meter" value="0.6">60%</meter>

## Iframe

<iframe src="https://example.com" width="100%" height="400" style="border: 1px solid #ccc;">
  Your browser doesn't support iframes.
</iframe>

## Audio and Video

### Audio

<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

### Video

<video width="320" height="240" controls>
  <source src="video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Canvas

<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000;">
  Your browser does not support the canvas element.
</canvas>

## SVG

<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>

<svg width="200" height="100">
  <rect width="200" height="100" style="fill:rgb(0,0,255);stroke-width:3;stroke:rgb(0,0,0)" />
</svg>

## Address

<address>
  Written by <a href="mailto:webmaster@example.com">John Doe</a>.<br>
  Visit us at:<br>
  Example.com<br>
  Box 564, Disneyland<br>
  USA
</address>

## Time

<p>The meeting is scheduled for <time datetime="2024-01-15T19:00">January 15, 2024 at 7:00 PM</time>.</p>

<p>Published: <time datetime="2024-01-01">January 1, 2024</time></p>

## Abbreviation

<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>

<p>Use <abbr title="HyperText Markup Language">HTML</abbr> for web pages.</p>

## Comment

<!-- This is an HTML comment -->
<!-- It won't be visible in the rendered output -->

<!-- 
Multi-line
HTML
comment
-->

## Ruby Annotation

<ruby>
  漢 <rp>(</rp><rt>kan</rt><rp>)</rp>
  字 <rp>(</rp><rt>ji</rt><rp>)</rp>
</ruby>

## Dialog

<dialog open>
  <p>This is a dialog element</p>
  <button>Close</button>
</dialog>

## Mixing HTML and Markdown

You can mix **Markdown** with <span style="color: red;">HTML</span>.

* Markdown list item
* <li style="color: blue;">HTML styled list item</li>
* Another markdown item

---

**Note**: Not all HTML elements work in all markdown renderers. Some may be sanitized for security reasons.
