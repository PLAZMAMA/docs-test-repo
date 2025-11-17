# Images Documentation

This document demonstrates various ways to include and reference images in Markdown.

## Basic Image Syntax

### Inline Image Reference

![Alt text for image](https://via.placeholder.com/400x200/0066cc/ffffff?text=Sample+Image)

### Image with Title

![Sample Image](https://via.placeholder.com/300x150/ff6600/ffffff?text=With+Title "This is a title tooltip")

## Different Image Sizes

### Small Image

![Small](https://via.placeholder.com/150x100/00cc66/ffffff?text=Small)

### Medium Image

![Medium](https://via.placeholder.com/400x250/cc0066/ffffff?text=Medium)

### Large Image

![Large](https://via.placeholder.com/800x400/6600cc/ffffff?text=Large)

## Reference-Style Images

Here's an image using reference style: ![Reference Image][logo]

And another one: ![Another Reference][banner]

[logo]: https://via.placeholder.com/200x200/333333/ffffff?text=Logo
[banner]: https://via.placeholder.com/600x150/666666/ffffff?text=Banner

## Images with Links

### Clickable Images

[![Clickable Image](https://via.placeholder.com/300x200/009688/ffffff?text=Click+Me)](https://example.com)

Click the image above to visit example.com!

### Multiple Linked Images

[![Image 1](https://via.placeholder.com/150x150/e91e63/ffffff?text=1)](https://example.com/1)
[![Image 2](https://via.placeholder.com/150x150/9c27b0/ffffff?text=2)](https://example.com/2)
[![Image 3](https://via.placeholder.com/150x150/3f51b5/ffffff?text=3)](https://example.com/3)

## Local Image References

These reference images that would be stored locally:

### Relative Path

![Local Image](./images/sample1.png)

### Absolute Path

![Absolute Path Image](/docs/images/sample2.png)

## Images in Lists

1. First item with image:
   ![List Image 1](https://via.placeholder.com/200x100/ff5722/ffffff?text=Item+1)

2. Second item with image:
   ![List Image 2](https://via.placeholder.com/200x100/ff9800/ffffff?text=Item+2)

3. Third item with image:
   ![List Image 3](https://via.placeholder.com/200x100/ffc107/ffffff?text=Item+3)

## Images in Tables

| Product | Preview | Price |
|---------|---------|-------|
| Widget A | ![Widget A](https://via.placeholder.com/100x100/4caf50/ffffff?text=A) | $29.99 |
| Widget B | ![Widget B](https://via.placeholder.com/100x100/8bc34a/ffffff?text=B) | $39.99 |
| Widget C | ![Widget C](https://via.placeholder.com/100x100/cddc39/ffffff?text=C) | $49.99 |

## Images in Blockquotes

> Here's an important visual reference:
>
> ![Quoted Image](https://via.placeholder.com/350x150/607d8b/ffffff?text=Important+Visual)
>
> This image illustrates a key concept.

## Complex Image Scenarios

### Image with Special Characters in Alt Text

![Image with "quotes" and 'apostrophes' & special chars](https://via.placeholder.com/300x150/795548/ffffff?text=Special+Chars)

### Multiple Images in Sequence

![Seq 1](https://via.placeholder.com/150x100/f44336/ffffff?text=1)
![Seq 2](https://via.placeholder.com/150x100/e91e63/ffffff?text=2)
![Seq 3](https://via.placeholder.com/150x100/9c27b0/ffffff?text=3)
![Seq 4](https://via.placeholder.com/150x100/673ab7/ffffff?text=4)

### Image Gallery Layout

Here's a grid of images:

![Gallery 1](https://via.placeholder.com/200x200/3f51b5/ffffff?text=1) ![Gallery 2](https://via.placeholder.com/200x200/2196f3/ffffff?text=2) ![Gallery 3](https://via.placeholder.com/200x200/03a9f4/ffffff?text=3)

![Gallery 4](https://via.placeholder.com/200x200/00bcd4/ffffff?text=4) ![Gallery 5](https://via.placeholder.com/200x200/009688/ffffff?text=5) ![Gallery 6](https://via.placeholder.com/200x200/4caf50/ffffff?text=6)

## Image Format Variations

### Different Image Formats (URLs)

**JPEG**: ![JPEG](https://via.placeholder.com/250x150.jpg/8bc34a/ffffff?text=JPEG)

**PNG**: ![PNG](https://via.placeholder.com/250x150.png/cddc39/ffffff?text=PNG)

**WebP**: ![WebP](https://via.placeholder.com/250x150.webp/ffeb3b/ffffff?text=WebP)

## Animated Images

### GIF Example

![Animated GIF](https://via.placeholder.com/300x200/ffc107/ffffff?text=GIF+Animation)

## SVG Images

### SVG Reference

![SVG Image](https://via.placeholder.com/300x150.svg/ff9800/ffffff?text=SVG+Format)

## Base64 Encoded Images

### Inline Base64 (Small Icon)

![Base64 Icon](data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNTAiIGhlaWdodD0iNTAiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHJlY3Qgd2lkdGg9IjUwIiBoZWlnaHQ9IjUwIiBmaWxsPSIjZmY1NzIyIi8+PHRleHQgeD0iMjUiIHk9IjI1IiBmb250LXNpemU9IjI0IiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSJ3aGl0ZSI+8J+WvjwvdGV4dD48L3N2Zz4=)

## Image Error Handling

### Missing Image

![This image doesn't exist](./missing-image.png)

### Broken URL

![Broken URL](https://this-domain-definitely-does-not-exist-12345.com/image.png)

---

**Note**: Some images use placeholder services. In production, these would be replaced with actual assets.
