---
title: "CSS Align horizontal vertical"
description: "CSS align, align element, align horizontal vertical."
publishDate: "20 Nov 2023"
tags: ["CSS"]
---

## Align Horizontal Vertical

In this lesson, we'll study how to align elements horizontally, vertically and both horizontally, vertically and both horizontally and vertically.

Horizontally

Here is how to horizontally align elements:

Horizontally centering text and inline elements

To center inline elements and/or text we need to wet the text-align CSS property to center.

Code

Horizontally centering Block-level elements

To horizontally center a block-level  element, ser the left and right margins to auto.

It makes the left and right margins of an element be equally divided on each side.

Don't forget to set the element's width property so it will not stretch to the edges of its container.

Code

Horizontally centering an image

To center an image we can simply use the same method as centering a block level element.

Since the <img> HTML element is an inline element by default we need to first set its display CSS property to block.

Code

Left and Right Align Text

We can either left or right align text by setting the text-align CSS property.

Code

Left and Right Align Elements

To left or right align elements use the position CSS property together qith the left or right properties.

Code

Note! If the element is wrapped in a container the container should have a position: relative declaration.

Another method is to use the float CSS property.

Code

Vertically

Here is how to vertically align elements:
Vertically centering using Padding

To vertically center a text or element inside a container set the top and bottom paaddings of the container with the same value.

Here is how to vertically center a text using padding:

Code

You can set the trxt-align CSS property to center to both horizontally and vertically center the text:

Code

On the example bellow we will vertically center a <div> inside a <div> using padding.

Code

Top and bottom align elements

To top or bottom align elements use the position  CSS property together with the top or bottom properties.

Code

Note! If the element is wrapped in a container the container should have a position: relative declaration.

Both Horizontally and vertically centering a Text

To center a text both horizontally and vertically inside an element (or container) we simply need to: define tur line-height property and set the text-align property to center.

Code

Both horizontally and vertically centering - usigb position

To both horizontally and vertically center and element or text in a container we need to:

1) set the position property of the container to relative.
2) set the posigion property of the container to absolute.
3) position the element using the top and left properties.
4) use the transform CSS property.

Here is how to exactly do it:

Code

Note you'll learn about the  transform css property in our 2d transforms leasson.

[[CSS]]
