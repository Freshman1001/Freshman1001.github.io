---
title: Easy CSS
date: 2023-11-05 09:05:06
tags: web
categories:
- web
- [html, css]
cover: https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQuXXqnhoPvHQ9kWgT-CuvhO1DJDMM4Bj3WkA&usqp=CAU
---

So many tutor there are for css , so this article just for review and quick look through. It can be used as a simple hand book.
<!-- more -->



## Q&A

### CSS Core?

Box model.

### What can CSS Do?

Box and in the box.

### How?

Selector and declaration(attribution and value).

### How to Add a CSS?

1. `<link>` in `<head>`: herf, type, ref
2. `<style>`: type

### How Selector Works?

1. \* {}

2. tag {}

3. .class {} h1.class {}

4. #id {}

5. parenttag > subtag {}

6. parenttag nestedtag {}

7. tag+nexttag {}

8. tag~siblingtag{}

   Border and background-color will not be inherited beside designated inherited.

9. []

10. [=]

11. [~=]

12. [^=]

13. [$=]

14. [*=]



## Color

Know color mechanism and representation.

1. color: usually refers to the text color
2. backgroung-color
3. opacity and rgba
4. hsl and hsla



## Text and Font

Know font design and mechanism.

font-family

font-size: px, %, em

@font-face

font-weight

font-style

font-transform

text-decoration

line-height: better use em as the unit

letter-spacing, word-spacing

text-align

vertical-align

text-indent

text-shadow: {down, right, size, color}

:first-letter, :first-line : pseudo element

:link, :visited :pseudo element

:hover, :active, :focus :respond to users



## Box Model

width, min-width, max-width

height, min-height, max-height

overflow: hidden/scroll

padding: inside. top, right, bottom, left(has order)

border: thin, medium, thick. or just (width, style, color)

​	border-style: solid, dotted, double, dashed, groove, ridge, inset, outset, hidden/none

​	border-color

margin: outside

all 3 above included in width and height

display: inline, block, inline-block, none

​		visibility: hidden, visible

boarder-image/-moz-boarder-image/-webkit-boarder-iamge: url() stretch, repeat, round

box-shadow

border-radius: radius width, radius height



## List Table and Form

list-style:

​	list-style-type

​	list-style-image

​	list-style-position

empty-cells

border-spacing, border-collapse

**layout of form**

​	float

cursor

​	auto

​	crosshair

​	default

​	pointer

​	move

​	text

​	wait

​	help

​	url(“”)





## Layout and Position

### Streaming(static)

block and inline

### Relative

Relative to the position it should be if there is position designation

### Absolute

Absolute to the page, just as if the element doesn't exist.

#### Absolute

Scroll with the page

#### Fixed position

Not scroll

#### Float Position

z-index

clear



## Image

size

align

background

background-repeat

background-attachment

linear-gradient

:hover :active
