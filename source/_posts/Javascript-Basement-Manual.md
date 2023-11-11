---
title: Javascript Basement Quick Overview - Interactive Front-end Development
date: 2023-11-07 20:58:48
tags: javascript
categories:
- web
cover: https://bairesdev.mo.cloudinary.net/blog/2023/08/What-Is-JavaScript-Used-For.jpg?tx=w_3840,q_auto
---

The article is about quick through or review on javascript. Notice that it is not a tutorial.

Before all start, I recommend you to learn html and css first. If you want to get started quickly, referring to the quick overview of html and css is an option.

<!--more-->

## Q&A

### How Javascript Work?

1. Visit html;
2. Modify content;
3. Make rules;
4. Respond to events.

### What is Script?

Series of commands.

### How to Write a Script?

Goal -> tasks -> coding.

### Object and Attribute?

Help computer know about the world.

Object:

Event;

Attribute;

Method.

### How Web Browser Work?

Objects:

1. Window
2. Document

Step:

1. Receive an html;
2. Modeling and storage to memory.
3. Rendering.

### How html, css and js  work Together?

1. html: content;
2. css: visual effect;
3. js: action.

### How to connect js and html?

`<script>`

### Debug?

console.log() or Web Browser



## Basement of Basement

comment

variable

​	data type: var array undefined

To try:

```javascript
document.getElementByID()
document.write()
[element].textContent = [*]
```



## Function, Methods and Objects

### Function

```js
function functionName(parameters, here){
    function body here;
    var outcome[ret1, ret2];
    return outcome;
}
functionName(parameter1, parameter2)[ansIndex];
```

Anonymous function

### Variable Scope

local & global

### Object

```js
var obj = {
    key: value，
    key: value,
    functionName: function(){
        functionBody here;
        return value;
    }
};
// or
var obj = new Object();
var obj = {};
// or constructor
function Obj (var1, var2, var3){
    this.var1 = value；
    this.var2 = value；
}
var obj = new Obj(var1, var2);
```

#### Visit Object Attribute

obj.attr or obj[‘arrt name’]

`delete` to delete an attribution.

#### Built-in Objects

1. #### BOM - window

   1. document

   2. history

   3. location

   4. navigator

   5. screen

      ```js
      window.innerHeight
      window.innerWidth
      window.pageXOffset
      window.pageYOffset
      window.screenX
      window.screenY
      window.location
      window.document
      window.history
      window.history.length
      window.screen
      window.screen.width
      window.screen.height
      window.alert()
      window.open()
      window.print()
      ```

      

2. #### DOM - Document

   1. `<html>`

      1. `<head>`
      2. `<title>`
      3. `<body>`
      4. `<div>`
         1. attribute
      5. `<p>`
      6. text

      ```js
      document.title
      document.lastModified
      document.URL
      ducument.domain
      ducument.write()
      ducument.getElementById()
      document.querySelectorAll()
      document.createElement()
      document.createTextNode()
      ```

      

3. #### Global js objects

   1. String
      1. length *length of '' is 0*
      2. toUpperCase()
      3. toLowerCase()
      4. charAt()
      5. indexOf()
      6. lastIndexOf()
      7. subString()
      8. split()
      9. trim()
      10. replace()
   2. Number
      1. isNan()
      2. toFixed()
      3. toPresicition()
      4. toExponential()
   3. Boolean
   4. Date
      1. getDate() setDate()
      2. getDay()
      3. getFullYear() setFullYear()
      4. getHours() setHours()
      5. get/setMilliseconds()
      6. getMinutes() setMinutes()
      7. get/setMonth()
      8. get/setSeconds()
      9. 
   5. Math
      1. PI
      2. round()
      3. sqrt(n)
      4. ceil()
      5. floor()
      6. random()
   6. RegEx

## DOM

document.getElementById()

document.getElementsByTagName()

document.querySelector()

document.querySelectorAll()

document.getElementsByClassName()

### Traverse

parentNode

previousSibling

nextSibling

firstChild

lastChild

### Get and Update

nodeValue

textContent

innerHTML: handle like a string

### Add and Remove

document.write() (not recommended)

createElement()	

createTextContent()

appendChild()

removeChild()

### Injection and XSS

Check and template

ESCAPE

### Attributes

.getAttribute()

.hasAttribute()

.setAttribute()





