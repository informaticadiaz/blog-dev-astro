---
title: "CSS Align"
description: "CSS Layout - Horizontal and Vertical Align. how to align elements horizontally, vertically. Alinear vertical horizontal."
publishDate: "25 Oct 2023"
tags: ["CSS"]
---

# CSS Layout Horizontal and Vertical Align

In this lesson, we'll study how to align elements horizontally, vertically and both horizontally, vertically and both horizontally and vertically.

## Horizontally

Here is how to horizontally align elements:

### Horizontally centering text and inline elements

To center inline elements and/or text we need to wet the text-align CSS property to center.

```css
.center {
	text-align: center;
	width: 100%;
	border: 3px solid #173459;
}
```

### Horizontally centering Block-level elements

To horizontally center a block-level element, ser the left and right margins to auto.

It makes the left and right margins of an element be equally divided on each side.

Don't forget to set the element's width property so it will not stretch to the edges of its container.

```css
.center {
	margin: 0 auto; /* same as margin-top: 0; margin-right: auto; margin-bottom: 0; margin-left: auto; */
	width: 60%;
	padding: 20px;
	border: 3px solid #173459;
}
```

### Horizontally centering an image

To center an image we can simply use the same method as centering a block level element.

Since the `<img>` HTML element is an inline element by default we need to first set its display CSS property to
block.

```css
.img {
	display: block;
	margin: 0 auto;
	width: 60%;
	height: auto;
}
```

### Left and Right Align Text

We can either left or right align text by setting the
text-align CSS property.

```css
.left {
	text-align: left;
}
.right {
	text-align: right;
}
p {
	background: lightgrey;
}
```

### Left and Right Align Elements

To left or right align elements use the position CSS property together qith the left or right properties.

```css
.right {
	float: right;
	width: 60%;
	padding: 10px;
	border: 3px solid #173459;
}
```

Note! If the element is wrapped in a container the container should have a position: relative declaration.

Another method is to use the float CSS property.

```css
.right {
	float: right;
	width: 60%;
	padding: 10px;
	border: 3px solid #173459;
}
```

## Vertically

Here is how to vertically align elements

### Vertically centering using Padding

To vertically center a text or element inside a container set the top and bottom paaddings of the container with the same value.

Here is how to vertically center atext using padding:

```css
div {
	padding-top: 40px;
	padding-bottom: 40px;
	border: 3px solid #173459;
}
```

You can set the text-align CSS property to center to both horizontally and
vertically center the text:

```css
div {
	padding-top: 40px;
	padding-bottom: 40px;
	text-align: center;
	border: 3px solid #173459;
}
```

On the example bellow we will vertically center a `<div>` inside a `<div>` using padding.

```css
div.container {
	padding-top: 40px;
	padding-bottom: 40px;
	background: #903c56;
}
div.content {
	background: #89c3d0;
}
```

### Top and bottom align elements

To top or bottom align elements use the position CSS property together with the top or bottom properties.

```css
.bottom {
	position: absolute;
	bottom: 0;
	width: 60%;
	padding: 10px;
	border: 3px solid #173459;
}
```

Note! If the element is wrapped in a container the container should have a position: relative declaration.

### Both Horizontally and vertically centering a Text

To center a text both horizontally and vertically inside an element (or container) we simply need to: define tur line-height property and set the text-align property to center.

```css
div {
	width: 250px;
	line-height: 250px;
	text-align: center;
	font-size: 20px;
	background: lightblue;
}
```

### Both horizontally and Vertically Centering - Using Position

To both horizontally and vertically center and element or text in a container we need
to:

1. Set the position property of the container to relative.
2. Set the posigion property of the container to absolute.
3. Position the element using the top and left properties.
4. Use the transform CSS property.

Here is how to exactly do it:

```CSS
.center {
    position: relative;
    height: 500px;
    border: 3px solid #173459;
}
.center > p {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```

Note you'll learn about the transform css property in our 2d transforms leasson.
