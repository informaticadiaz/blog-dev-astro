---
title: "CSS Pseudo Classes"
description: "CSS Pseudo Classes, Pseudo Classes, CSS Pseudo Classes, Pseudo Classes."
publishDate: "21 Nov 2023"
tags: ["CSS"]
---

## Pseudo Clases

A CSS pseudo-class is a keyword added to a selector that specifies a special state for the targeted elements.

Syntax:
selector: pseudo-class {
 property: value;
}

The :hover Pseudo-class

The CSS :hover pseudo-class can be used to change an element's styles when the user's pointer hovers (mouses over) it.

p:hover {
   color: red;
   font-size: 20px;
}
/*optional; specifies the duration of the effect*/
p {
    transition-duration: 2s;
}

CSS Anchor Pseudo-classes
The following pseudo-classes are used for the anchor (<a>) element.

a:link {
   color: orange;
}
a:visited {
   color: red;
}
a:hover {
   color: green;
}
a:active {
   color: pink;
}

Note! In the CSS definition, the :hover pseudo-class should come after the :link and :visited pseudo-classes. And the :active pseudo-class must come after the :hover pseudo-class.

Index of CSS Pseudo-classes

Click the examples to Try it Yourself and see description.
Pseudo-class
:active
:checked
:disabled
:empty
:enabled
:first-child
:first-of-type
:focus
:hover
:in-rangr
:invalid
:lang(language)
:last-child
:last-of-type
:link
:not(selector)
:nth-child(n)
:nth-last-child(n)
:nth-last-of-type(n)
:nth-of-type(n)
:only-of-type
:only-child
:optional
:out-of-range
:read-only
:read-write
:required
:root
:target
:valid
:visited

[[CSS]]
