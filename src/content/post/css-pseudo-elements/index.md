---
title: "CSS Pseudo-elements"
description: "CSS Pseudo-elements, Child combinator, Descendant combinator, Adjacent zibiling combinator, General sibling combinator."
publishDate: "23 Oct 2023"
tags: ["CSS"]
---

## CSS pseudo-elements

A CSS pseudo-element is a keyword added to a selector that lets you style a specific part of the selected element(s).

## Syntax

```CSS
selector::pseudo-element {
   property: value;
}
```

In this lesson we'll study following CSS pseudo elements:

- ::after
- ::before
- ::first-letter
- ::first-line
- ::selection

## The ::after Pseudo-element

The ::after CSS pseudo-elemnt creates a pseudo-element that is the last child of the selected element.

It is commonly used with the content CSS property to add cosmetics to the selected element.

The creared element is inline by default.

```CSS
.true::after {
   content: "-> True";
   color: green;
}
.false::after {
   content: "-> False";
   color: red;
}
```

## The ::before pseudo-element

The ::before CSS pseudo-element creates a pseudo-element that is the first child of the selected element.

It is commontly used with the content CSS property to add cosmetics to the selected element.

The created element is inline by default.

```CSS
.true::before {
   content: "-> True";
   color: green;
}
.false::befofe {
   content: "-> False";
   color: red;
}
```

We can also use it on HTML lists to add custom bullets:

```CSS
ul {
   list-style-type: none;
}
li:before {
   content: "->";
  color: blue;
}
```

## The ::first-letter Pseudo-element

The ::first-letter CSS pseudo-element applies styles to the first letter of the first line of the selected block-level element.

Allowed CSS properties:

- All font properties
- All background properties
- All margin properties
- All padding properties
- All border properties
- All color property
- word-spacing, letter-spacing, text-decoration, text-transform, line-height, text-shadow, text-decoration-style, vertical-align

```CSS
p::first-letter {
   text-decoration: overline;
   font-size: 250%;
   color: red;
}
```

## The forst-line Pseudo-elemnt

The ::first-line CSS pseudo-element applies styles to the first line of the selected block-level element.

Allowed CSS Properties:

- All font properties
- All background properties
- The color property
- word-spacing, letter-spacing, text-decoration, text-transform, line-height, text-shadow, text-decoration, text-decoration-color, text-decoration-line, text-decoration-style, vertical-align.

```CSS
p::first-line {
   color: #f8f9f9;
   background-color: #173459;
}
```

## The ::selection Pseudo-element

The ::selection CSS pseudo-element applies styles to the part of a document that has been hijhlighted or selected by the user.

Allowed CSS Properties:

- color
- background-color
- cursor
- caret-color
- outline css properties
- text-decoration and its associated properties
- text-emphasis-color
- text-shadow

```CSS
p::selection, textarea::selection {
   color: green;
   background-color: red;
}
```
