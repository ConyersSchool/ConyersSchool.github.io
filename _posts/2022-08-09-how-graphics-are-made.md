---
title: How Graphics Are Made 
author: Nikky Leone
date: 2022-08-09 20:55:00 +0800
categories: [Year 9, Photoshop]
tags: [how graphics are made]
---

# Bitmaps

A **bitmap** or raster graphic, if you will, **is created from rows of different colored pixels that together form an image. In their simplest form, bitmaps have only two colors, with each pixel being either black or white.** With increasing complexity, an image can include more colors; **photograph-quality images may have millions of pixels.** **Examples of bitmap graphic formats include `GIF`, `JPEG`, `PNG`, `TIFF`, `XBM`, `BMP`, and `PCX` as well as bitmap fonts.** The image displayed on a computer monitor is also a bitmap, as are the outputs of printers, scanners, and similar devices. They are created using paint programs like [**Adobe Photoshop.**](https://www.adobe.com/uk/products/photoshop.html)

# Vector

**Vector** graphics are constructed using mathematical formulas describing shapes, colors, and placement. Rather than a grid of pixels, **a vector graphic consists of shapes, curves, lines, and text which together make a picture.** While a bitmap image contains information about the color of each pixel, **a vector graphic contains instructions about where to place each of the components.** It is even possible to embed a bitmap graphic within a vector graphic, which is how vector-bitmap hybrid graphics work. It is not possible, however, to embed vector information within a bitmap. **Examples of vector graphic formats are `PICT`, `EPS`, and `WMF` as well as `PostScript` and `TrueType` fonts.** These are created with `GIS` and `CAD` applications as well as drawing programs like FreeHand.  

> If you did not quite understand some of the terms used in the last few paragraphs, I  strongly advise you to read this [**article**](https://pediaa.com/what-is-the-difference-between-bitmap-and-vector/) where every term is described in depth
{: .prompt-tip }

# Bonus: SVG

SVG, or **Scalable Vector Graphics, is a language for describing vector graphics in XML** (dead language (¬_¬) ). With SVG, you can code graphics directly into an XML document. For more information about SVG, see:

> http://www.wdvl.com/Authoring/Languages/XML/SVG/
  
  
# Bitmap and Vectors: strengths and weaknesses 

- In general, a **bitmap graphic is much larger than a similar vector graphic.**
- **Bitmap graphics are affected by resolution. If you enlarge a bitmap graphic, it will look jagged. When shrunk, its features become indistinct and fuzzy.** This does not happen with vector graphics as their shapes are redrawn to compensate for changes in resolution.
- **Altering vector graphics is easy because the shapes within them can be ungrouped and edited individually.** However, vector graphics are difficult to modify or even display when they are not opened in programs that understand their rendering languages. For example, while many `Mac OS` drawing programs easily display and edit `PICT` files, few are able to do anything at all with `WMF` files. Most paint applications, however, are capable of opening many different kinds of bitmap graphic formats.
- **You can easily convert one kind of bitmap file into another. You can also convert a vector graphic into a bitmap. However, it is very difficult to convert a bitmap graphic into a true vector graphic.** It is even difficult to convert one kind of vector graphic into another (e.g. `PICT` to `WMF`).
- **Vector graphics are not appropriate for complex images** (e.g. digitized photographs).
