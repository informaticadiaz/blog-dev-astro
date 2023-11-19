---
title: "CSS Float Clear"
description: "CSS Float Clear, CSS Float Clear, clear float, css properties."
publishDate: "24 Oct 2023"
tags: ["CSS"]

---

## CSS Float Clear

The float and clear properties the float CSS property places and element on the left or right side of its container  (containing block).

It allows inline elements to wrap arround it.

Valid Values:
None: default; the element does not float
Left: the element floats on the left side of its container.
Right: the element floats on the left side of its container.

Here is an example of an element that does not float:

Here is an example of an element that float on the left side:

Here is an example of an element that floats on the right side:

CSS clear property
The cleae CSS property sets whether an element can have floating elements around it.

It can be applied to floating and non-floating elements.

Valid Values:
none: default; elements are allowed to float on both sides
left: elements are not allowed to float on the left side.
right: elements are not allowed to float on the right side.
both: elements are not allowed to float on both sides

An element will fit horizontally to the space next to an element which is floated.

Unless we set the clear property to the same side as the float. For example if an element is floatrd left and we don't.want the next element to take up the sapace next to it then we can set the clear property to left as well.

If we do this, the cleared element will be renderrd below the floated element instead of taking the horizontal space around the floating element.

Problem with CSS floats
A floated element is removed from the normal flow of the page.

If a floating element is taller than its container it will overflow outside the container. Because the container will not contain the height of a floated element.

To make a container be able to resizd so that it contains the floating elements inside it we need to self-clear its children.

To do that we need to use the clearfix hack:

Learn about the ::after pseudo-element here

Example:

Grid Layout using CSS Floats
With CSS floats we can create a grid of boxes with equal sizes. This approach is ideal for organizing web contents.

To achieve it, we simply need a container with the clearfix hack that will contain the boxes.

We also need to set all elements box-sizing property to border-box so that the padding and borders do not enlarge the total width and height of the boxes. If we don't do this the padding and border will not stay inside the box instead its size will be added and produxe unexpected results. Learn more here.

Then we need to divide 100% to the number of boxes we need.

For example, to creare a two-column layout then simply divide 100% to two: 100% / 2 = 50%.

As you may notice, we also removed the default padding and margins of the body using the following code:

Code

This is a good practice in CSS layouting as it maximizes the space and appeals more to the eyes.

Moreover, it is also useful to create grid layout with unequal size of boxes.

The example below shows a grid of boxes where the first box is 25% wide and the second is 75%.

Code

Note! If one column js larger or has more content, it can grow bigger than the other. To prevent this from happening we could simply define a fixed height for the boxes.

Code

[[CSS]]
