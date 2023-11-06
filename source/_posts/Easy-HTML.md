---
title: Easy HTML
date: 2023-11-04 16:02:29
tags: web
categories:
- web
- [html, css]
cover: https://austingil.com/wp-content/uploads/HTML-Blog-Cover.png
---



So many tutor there are for html , so this article just for review and quick look through. It can be used as a simple hand book.
<!-- more -->


## Q&A



### **How to visit web?**

1. Browser
2. Web Server
3. Device
4. Monitor/Reader



### **How to Build Web**

What you see: Browser rendering

Mini-web: html and css only

Large project: CMS and so on



### **H5 and Css3?**

The latest.



### **Mechanisms to Visit**

DNS, simply.

More details in computer networking.



## HTML



### Basic Elements

1. `<body>`: show in windows
2. `<head>`: page info
3. `<title>`: tab title



## Text

`<h [1-6]>`: title

`<p>`: paragraph

`<b>`: bold

`<i>`: italic 

`<sup>`: superscript 

`<sub>`: subscript

`<br />`:  break line

`<hr>`: horizontal line

`<em>`: inline element(strong emphasized)

`<blockquote>`: quote

`<q>`: short quote

`<abbr title=“whole word”>ABB</abbr>`: abbreviation

`<cite>`: citation to book or film

`<dfn>`: definition of something 

`<address>`: include the info of author

`<ins>`: insert(underline)

`<del>`: deleted line

`<s>`:  deleted line



### List

`<ol>`: ordered list

`<li>`: list item

`<ul>`: unordered  list

`<dl>`: definition list

`<dt>`: definition term

`<dd>`:definition

lists can be nested.



### Link

`<a herf=""></a></a>`: if point to another site, herf must be absolute url. Can be relative url vice versa.



### Directory Structure

**key words:**

root directory

parent directory

​		subdirectory 

index.html



#### Relative URL

1. *
2. */
3. ../*
4. $*$/$*$/
5. ../../*



#### Email Link

`<a herf="mailto:sombody@example.org"></a></a>`



#### Others Feature

target=“_blank”

`<a herf="#[id]"></a></a>`: to id’s position



## Image

set an image directory

`<img>`:

​	src: :link:

​	alt: alternative 

​	title

​	height: better should be designated for better performance

​	weight: better should be designated for better performance

Image should be measured in pixels.

The storage format of images should be determined by its color distribution to optimize performance

`<figure>`

​	`<img>`

​	`<figcaption>`

`</figure>`



## Table

`<table>`

​	`<tr>` : row

​		`<th>`: heading scope=“row”/“col”

​			`<td>`: data colspan rowspan

`<thead><tbody><tfoot>`



## Form

Understand workflow with SERVER

`<form>`:

​	action

​	method: get/post

​	id

`<input>`:

​	type: text, password, radio, checkbox, file, submit, image(use image for submit button), hidden, date, email, url, search

​	value: use in radio, checkbox

​	checked: use in radio, only one option checked.

​	name: Identify form

​	maxlength

​	placehoder: hint

`<textarea>`

`<select>`: drop-box

​	name

​	`<option>`

​	value

`<button>`: can contain other elements

`<label>`:

​	for: form id

`<fiedlset>`: a set of forms

​	`<legend>`: title of fieldset

form validation: Done by js usually, but easy validation like required can be done by h5.



## Other Tags

`<!DOCTYPE html>`

`<!-- -->`

id

class

`<div>`

`<span>`

`<iframe>`

​	width

​	height

​	src

​	seamless: no scrolling

`<meta>`

​	name=

​		description

​		keywords

​		robots: to search engine, contain `noindex` and `nofollow`

​	http-equiv=

​		author

​		pragma

​		expires

​	content

escape characters: &



## Video and Audio

1. Hosting Service on youtube or vimeo, soundcloud.com or myspace.com
2. `<vedio>` and `<audio>`

​		src

​		poster

​		width and height

​		control: default control

​		autoplay

​		loop

​		preload=

​			none

​			auto

​			metadata

capability: add more than one media format(multi-source), like mp4 and webM 

`		<source>`

​	src

​	type: tell browser the type will save load time

​	codecs

3. js



## New Feature in H5 Layout

No so many `<div>`

`<header>` `<article>` `<footer>` `<aside>` `<section>` `<nav>` `<aside>` `<hgrounp>` `<figure>` `<figurecaption>`

