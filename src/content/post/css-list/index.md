---
title: "CSS List"
description: "CSS List, CSS <ul>, CSS <li>, CSS List, CSS <ul>, CSS <li>."
publishDate: "21 Nov 2023"
tags: ["CSS"]
---

## CSS List

In CSS, there are a lot of options for styling HTML lists. We can change its bullets, colors, positions etc.

If you're unfamiliar with HTML Lists you can install this Learn HTML app for free!

Let's have a quick review. In HTML there are two types of lists:
`<ul>` an unordered list; list items are marked with numbers or letters.

And then we have the ``<li>`` element which defines the list items for both unordered and ordered lists.

CSS List Bullet Styles/Types
The list-style-type CSS property sets the bullet type or marker to use.

Valid Values:
`none:` no bullet type
`disc:` a filled circle; default value.
`circle:` a hollow circle
`square:` a filled square
`decimal:` decimal numbers e.g. 1, 2, 3
`decimal-leading-zero:` decimal numbers with leading zeros e.g. 01, 02, 03
lower-roman: uppercase roman numerals e.g. I, II, III
`lower-alpha:` lowercase letters e.g. A, B, C
`lower-greek:` lowercase classical greek e.g.
`arabic-indic:` traditional Arabic-indic numbering
`georgian:` traditional Georgian numbering
`armenian:` traditional Armenian numbering

Here is an example of an unordered list bullet types

Here is an example of an ordered list bullet types.

CSS List Bullet Position
The `list-style-position` CSS property sets the position (whether it's outside or inside) of the bullets.

Valid Values:
outside: sets the bullets to sit outside the list items ( default)
inside: sets the bullets to sit inside the list items.

CSS List Bullet Images.

In CSS, it's possible to have inages as list bullets.

The list-style-image CSS property sets an image as bullets. Example:

Howerver, this property is very limited in terms of controlling the position, size, etc, of the bullets.

For that reason, we better use CSS background properties.

CSS List with Padding Margin and Colors
To make list look interesting we can add paddings, margins and colors.

Note! Any style to the ``<ul>`` and `<ol>`elements affects the entire list while any style added to the ``<li>`` element only affects list items.

[[CSS]]
