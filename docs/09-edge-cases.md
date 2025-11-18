# Edge Cases and Stress Tests

This document contains edge cases, unusual patterns, and stress tests for markdown renderers.

## Empty Elements

### Empty Headers

#

##

###

### Empty Lists

*
-
+

1.
2.

### Empty Table Cells

| A | B | C |
|---|---|---|
|   |   |   |
|   | X |   |
|   |   |   |

### Empty Blockquote

>

### Empty Code Block

```

```

## Extreme Nesting

### Deeply Nested Lists

* Level 1
  * Level 2
    * Level 3
      * Level 4
        * Level 5
          * Level 6
            * Level 7
              * Level 8
                * Level 9
                  * Level 10

### Deeply Nested Blockquotes

> Level 1
> > Level 2
> > > Level 3
> > > > Level 4
> > > > > Level 5
> > > > > > Level 6
> > > > > > > Level 7
> > > > > > > > Level 8

### Mixed Deep Nesting

> Blockquote level 1
> * List item 1
>   * Nested list 1
>     > Nested blockquote
>     > * List in blockquote
>     >   1. Ordered in list in blockquote
>     >      * Even deeper

## Special Characters

### Markdown Special Characters

\\ \` \* \_ \{ \} \[ \] \( \) \# \+ \- \. \! \| \~

### Multiple Consecutive Special Characters

*****

_____

~~~~~

`````

#####

### Special Characters in Content

Text with * asterisks * and _ underscores _ and ` backticks `.

Text with [brackets] and (parentheses) and {braces}.

### Unicode Edge Cases

Zero-width space:​ (between these words)

Right-to-left mark: ‏Text‏

Combining characters: e̊ å ñ

Emoji with modifiers: 👋🏻 👋🏿 👨‍👩‍👧‍👦

Unusual emoji: 🫠 🫥 🫡 🫢 🫣

## Very Long Content

### Long Line Without Breaks

ThisIsAVeryLongWordThatDoesNotContainAnySpacesOrBreakingCharactersAndIsDesignedToTestHowMarkdownRenderersHandleExtremelyLongContinuousTextWithoutAnyNaturalBreakingPointsWhichMightCauseLayoutIssuesOrOverflowProblemsInSomeRenderers

### Long URL

https://example.com/very/long/path/with/many/segments/that/goes/on/and/on/and/continues/for/a/very/long/time/to/test/how/renderers/handle/extremely/long/urls/that/might/overflow/their/containers?parameter1=value1&parameter2=value2&parameter3=value3&parameter4=value4

### Extremely Long Table Row

| A | B | C | D | E | F | G | H | I | J | K | L | M | N | O | P | Q | R | S | T | U | V | W | X | Y | Z |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 | 23 | 24 | 25 | 26 |

## Ambiguous Syntax

### Asterisk Ambiguity

***text***

** text**

* *text*

*text *

### Underscore Ambiguity

___text___

__ text__

_ _text_

_text _

### Mixed Emphasis

*__text__*

_**text**_

**_text_**

***bold and italic***

### Code Ambiguity

`code with ` backtick`

``code with ` backtick``

```code with ``` backticks```

## Invalid or Malformed Syntax

### Unclosed Elements

**Bold without closing

*Italic without closing

[Link without closing paren](url

![Image without closing](url

### Mismatched Elements

**Bold with italic close*

*Italic with bold close**

### Incorrect Nesting

**Bold *italic** mixed*

## Duplicate IDs

### Duplicate Headers

#### Same Header
#### Same Header
#### Same Header

### Headers with Same ID

#### header
#### Header
#### HEADER
#### header

## Whitespace Edge Cases

### Leading/Trailing Whitespace

**  bold with spaces  **

*  italic with spaces  *

`  code with spaces  `

### Multiple Spaces

Multiple     spaces     between     words

### Tabs vs Spaces

	Tab-indented line
    Space-indented line
	    Mixed indentation

## Number Edge Cases

### Lists with Unusual Numbering

0. Starting at zero
1. One
2. Two

10. Starting at ten
11. Eleven
12. Twelve

999. Large number
1000. Larger number

### Lists with Wrong Order

1. First
5. Fifth (marked as 5)
3. Third (marked as 3)

## Link Edge Cases

### Link with No URL

[Text]()

[Text]( )

### Link with No Text

[](https://example.com)

[ ](https://example.com)

### Nested Links (Invalid)

[[Nested]](url1)(url2)

### Links with Special Characters

[Link with spaces](https://example.com/path with spaces)

[Link<with>special](https://example.com)

## Image Edge Cases

### Image with No URL

![Alt text]()

### Image with No Alt Text

![](https://placehold.co/150)

### Very Long Alt Text

![This is an extremely long alt text that goes on and on and continues to provide excessive description that might cause issues in some renderers especially if they try to display this text in tooltips or other constrained spaces](https://placehold.co/150)

## Code Block Edge Cases

### Code Block with Triple Backticks Inside

````
```
Code with backticks
```
````

### Code Block with Language and Extra Text

```javascript this is extra text
console.log("test");
```

### Empty Code Block with Language

```javascript
```

## Table Edge Cases

### Table with Missing Cells

| A | B | C |
|---|---|---|
| 1 | 2 |
| 3 |
| 4 | 5 | 6 |

### Table with Extra Cells

| A | B |
|---|---|
| 1 | 2 | 3 | 4 |

### Misaligned Table

| A | B | C |
|---|
| 1 | 2 | 3 |

### Table with No Header

|---|---|---|
| 1 | 2 | 3 |
| 4 | 5 | 6 |

## Horizontal Rule Variations

***
* * *
*****
- - -
-------
___
_ _ _
_______

Mixed:
* - *
- * -

## Escaping Edge Cases

### Escaped Escapes

\\**not bold\\**

\\*not italic\\*

### Partially Escaped

\**half bold**

*\*half italic*

## HTML Edge Cases

### Unclosed HTML Tags

<div>
<span>
<p>

### Invalid HTML

<notarealtag>content</notarealtag>

<div style="invalid css: !!;">content</div>

### Mixed Case HTML

<DIV>Capital div</DIV>

<SpAn>Mixed case span</SpAn>

## Reference Link Edge Cases

### Undefined Reference

[Undefined reference][nonexistent]

### Duplicate References

[Link1][ref]
[Link2][ref]

[ref]: https://example.com

### Reference with No Definition

[Link][ref-with-no-def]

## Character Encoding

### Different Quotes

"Double quotes"
'Single quotes'
"Curly double quotes"
'Curly single quotes'
„German quotes"
«French quotes»

### Dashes and Hyphens

Hyphen: -
En dash: –
Em dash: —
Minus: −

### Mathematical Symbols

≠ ≤ ≥ ± × ÷ √ ∞ ∑ ∏ ∫

### Currency Symbols

$ € £ ¥ ₹ ₽ ₩ ₪ ₦

## Performance Stress Tests

### Many Paragraphs

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris.

Nisi ut aliquip ex ea commodo consequat.

Duis aute irure dolor in reprehenderit in voluptate velit.

Esse cillum dolore eu fugiat nulla pariatur.

Excepteur sint occaecat cupidatat non proident.

Sunt in culpa qui officia deserunt mollit anim id est laborum.

### Many Links

[Link1](url) [Link2](url) [Link3](url) [Link4](url) [Link5](url) [Link6](url) [Link7](url) [Link8](url) [Link9](url) [Link10](url) [Link11](url) [Link12](url) [Link13](url) [Link14](url) [Link15](url) [Link16](url) [Link17](url) [Link18](url) [Link19](url) [Link20](url)

### Many Images

![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50) ![](https://placehold.co/50)

## Corner Cases

### Just a Header

# Nothing Else

### Just a List

* Only
* A
* List

### Just a Table

| A | B |
|---|---|
| 1 | 2 |

### Just Code

```
Only code here
```

### Just a Quote

> Only a quote

---

**Note**: Many of these edge cases may cause unexpected behavior or errors in markdown renderers. They are intentionally included to test robustness and error handling.
