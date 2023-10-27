---
title: "CSS Attribute Selectors"
description: "CSS Attribute Selectors, CSS Attribute Selectors attribute selectors target elements,"
publishDate: "10 Sept 2023"
tags: ["CSS"]
draft: true
---

## CSS Attribute Selectors

The CSS attribute selectors target elements based on the presence or value of a given attribute.

### `[attr]`

Selects elements with selectors target elements based on the presence or value of a given attribute.

The example below selects `<a>` elements with the title attribute.

```CSS
a[title] {
   color: red;
}
```

### `[attr=value]`

Selects elements with an attribute name of attr whose value is axactly value.

The example below selects `<a>` elements whose title attribute's value is exactly codeliber.

```CSS
a[title="codeliber"] {
   color:red;
}
```

### [attr~=value]

Selects elements with an attribute name of `attr` whose value is exactly `value`.

It can select elements with the attribute name `attr` that has multiple values (separated by white-spaces) including `value`.

The example below selects `<a>` elements whose `title` attribute's values are `codeliber`, `codeliber css`, `css codeliber`, `html codeliber css` but NOT `codelibers` and `codeliber-css`.

```CSS
a[title~="codeliber"] {
   color: red;
}
```

### [attr|=value]

Selects elements with an attribute name of `attr` whose value can be exactly `value` or can begin with `value` immediately followed by a hyphen, `(-)`.

It is often used for language subcode matches.

The example below selects `div` elements whose lang attribute values start with `en-`.

```CSS
div[lang|="en"] {
   color: green;
}
```

The example below selects `<div>` elements whose lang attribute values start with `zh-`.

```CSS
div[lang="zh"] {
   color: red;
}
```

### `[attr^=value]`

Selects elements with an attribute name of attr whose value is prefixed (preceded) by `value`.

The example below selects internal links(`<a>` elements whose `href` value starts with a hash `#`).

```CSS
a[href^="#"] {
   color:fuchsia;
}
```

### `[attr$=value]`

Select elements with an attribute name of `attr` whose value is prefixed (preceded) by `value`.

The example below selects `<a>` elements whose `href` value ends with `.org`.

```CSS
a[href*="exam"] {
   color: red;
}
```

Note! All attribute selectors values are cased sensitive by default.

To make the value be compared case-insesitively, simply add an `i` or `I` before the closing bracket.

```CSS
a[title="codeliber" i] {
 color: red;
}
```
