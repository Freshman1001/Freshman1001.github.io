---
title: Easy CSS
date: 2023-11-05 09:05:06
tags: web
categories:
- web
- [html, css]
cover: https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQuXXqnhoPvHQ9kWgT-CuvhO1DJDMM4Bj3WkA&usqp=CAU
---

CSS，从入门到？
<!-- more -->

[TOC]



## Q&A

### CSS Core?

核心的 CSS 概念之一是“盒子模型”（Box Model），它是 CSS 中用于布局的基本原理。盒子模型描述了 HTML 元素是如何在页面上布局的，每个元素都被看作是一个矩形的“盒子”，包含了内容、内边距、边框和外边距。

#### 盒子模型的组成部分

1. **内容区域（Content Area）**：元素的实际内容，比如文本、图像等。
2. **内边距区域（Padding Area）**：内容区域周围的空白区域，通过 `padding` 属性控制。
3. **边框区域（Border Area）**：内边距区域外围的边框，通过 `border` 属性控制。
4. **外边距区域（Margin Area）**：边框区域外的空白区域，通过 `margin` 属性控制。

#### 如何设置盒子模型的属性

- **设置盒子尺寸：** 使用 `width` 和 `height` 属性设置元素的宽度和高度。

  ```
  div {
    width: 200px;
    height: 100px;
  }
  ```

- **设置内边距：** 使用 `padding` 属性设置元素的内边距。

  ```
  div {
    padding: 20px;
  }
  ```

- **设置边框：** 使用 `border` 属性设置元素的边框。

  ```
  div {
    border: 2px solid #000;
  }
  ```

- **设置外边距：** 使用 `margin` 属性设置元素的外边距。

  ```
  div {
    margin: 10px;
  }
  ```

#### 盒子模型的计算方式

- **标准盒子模型：** 在标准盒子模型中，元素的宽度和高度仅包括内容区域（不包括内边距、边框和外边距）。
- **IE 盒子模型：** 在 IE 盒子模型中，元素的宽度和高度包括了内边距和边框，但不包括外边距。

你可以通过设置 `box-sizing` 属性来指定使用哪种盒子模型。例如：

```
div {
  box-sizing: border-box; /* 使用 IE 盒子模型 */
}
```

总的来说，盒子模型是 CSS 中布局的基础，了解和熟练使用盒子模型的相关属性是掌握 CSS 核心概念的关键之一。

### What can CSS Do?

CSS（层叠样式表）是一种强大的样式语言，使得Web开发人员能够控制网页上HTML元素的呈现和布局。以下是CSS能够实现的一些功能，特别是在“盒子及其内部”这个背景下：

1. **布局和定位：**
   - **盒子模型：** CSS允许通过盒子模型来控制元素的布局。这包括设置元素的宽度、高度、内边距、边框和外边距。
   - **定位：** CSS提供了相对定位、绝对定位、固定定位和粘性定位等不同的定位方案，以精确控制元素在页面上的位置。
2. **样式和装饰：**
   - **颜色和背景：** CSS允许设置文本和背景的颜色，包括使用渐变和图像作为背景。
   - **边框和圆角：** 您可以为元素应用不同样式和宽度的边框，并使用 `border-radius` 创建圆角。
   - **阴影：** CSS可以使用 `box-shadow` 属性为元素创建阴影效果。
3. **排版：**
   - **字体样式：** CSS允许您控制文本的字体系列、大小、粗细、样式等属性。
   - **文本对齐和装饰：** 您可以对齐文本，给文本加下划线或删除线等装饰。
   - **字母和单词间距：** 使用 `letter-spacing` 和 `word-spacing` 属性调整字母和单词之间的间距。
4. **响应式设计：**
   - **媒体查询：** CSS通过使用媒体查询根据设备的特性（如屏幕宽度）应用样式，从而实现响应式设计。
5. **变换和过渡：**
   - **变换：** CSS提供缩放、旋转、倾斜和平移等变换，可以用于调整元素的外观。
   - **过渡：** 使用CSS过渡，可以在一段时间内平滑地动画属性的变化。
6. **Flexbox 和 Grid 布局：**
   - **Flexbox：** CSS的Flexbox是一种布局模型，可以更有效地设计复杂的布局，特别是在分配空间和对齐项目方面。
   - **Grid 布局：** CSS Grid提供了一个二维布局系统，更容易创建基于网格的设计。
7. **伪类和伪元素：**
   - **伪类：** 通过伪类（如 `:hover`、`:active`、`:focus`）选择和样式元素的不同状态。
   - **伪元素：** 样式元素的特定部分，例如 `::before` 和 `::after`。
8. **动画：**
   - **关键帧动画：** CSS支持关键帧动画，通过定义关键帧并将其应用于元素，可以创建复杂的动画效果。
9. **自定义和主题化：**
   - **变量：** CSS变量（`--variable-name`）允许创建可重用和可自定义的样式。
   - **@media规则：** 使用 `@media` 规则根据输出设备的特性应用不同的样式。

总的来说，CSS是Web开发人员控制网页视觉呈现的重要工具，提供了广泛的功能，用于创建美观且响应式的设计。"盒子及其内部"的概念强调HTML元素被视为盒子，并且CSS提供了在文档中样式和排列这些盒子的手段。

### How?

#### Selector and declaration(attribution and value)

1. 在CSS中，样式规则由选择器和声明组成。每个样式规则定义了页面上特定元素的样式，包括元素应用的属性和属性的值。下面是关于选择器和声明的基本概念：

#### 选择器（Selectors）

   选择器用于选择页面上要样式化的元素。它告诉浏览器应该应用哪些样式规则。以下是一些常见的选择器类型：

   1. **元素选择器（Element Selector）：** 根据元素的名称选择元素。

      ```
      p {
        /* 样式规则 */
      }
      ```

   2. **类选择器（Class Selector）：** 根据元素的类名选择元素。

      ```
      .highlight {
        /* 样式规则 */
      }
      ```

   3. **ID 选择器（ID Selector）：** 根据元素的 ID 选择元素。

      ```
      #header {
        /* 样式规则 */
      }
      ```

   4. **属性选择器（Attribute Selector）：** 根据元素的属性选择元素。

      ```
      input[type="text"] {
        /* 样式规则 */
      }
      ```

   5. **伪类选择器（Pseudo-class Selector）：** 根据元素的状态或位置选择元素。

      ```
      a:hover {
        /* 样式规则 */
      }
      ```

   6. **伪元素选择器（Pseudo-element Selector）：** 选择元素的特定部分。

      ```
      p::first-line {
        /* 样式规则 */
      }
      ```

#### 声明（Declarations）

   声明由属性和属性值组成。每个声明指定了要应用于选择的元素的一种样式。以下是声明的基本结构：

   ```
   selector {
     property: value;
   }
   ```

   - **属性（Property）：** 指定要设置的样式的类型，比如 `color`、`font-size`、`margin` 等。
   - **值（Value）：** 指定给属性的具体值，比如 `red`、`16px`、`10px 20px`。

   例如，将段落文字颜色设置为红色：

   ```
   p {
     color: red;
   }
   ```

   或者将标题的字体大小设置为16像素：

   ```
   h1 {
     font-size: 16px;
   }
   ```

   多个声明可以组合在一个样式规则中：

   ```
   h2 {
     color: blue;
     font-size: 18px;
     margin-bottom: 10px;
   }
   ```

   通过选择器和声明，你可以有效地控制页面上各个元素的外观和布局。CSS的强大之处在于其层叠性质，允许多个样式规则同时应用到一个元素上，最终形成最终的样式。

### Add CSS

在HTML文档中添加CSS样式的常见方法有两种：使用`<link>`元素和`<style>`元素。

#### 1. 使用 `<link>` 元素

`<link>` 元素用于将外部样式表链接到HTML文档。它通常位于HTML文档的 `<head>` 部分。以下是添加CSS样式的基本语法：

```
html<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  
  <!-- 使用 link 元素引入外部样式表 -->
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
  <!-- 页面内容 -->
</body>
</html>
```

在上面的例子中，`href` 属性指定了外部样式表的文件路径，`type` 属性指定了样式表的类型为CSS，`rel` 属性表示关系为样式表。

#### 2. 使用 `<style>` 元素

<style> 元素用于在HTML文档中嵌入CSS样式。可以将其放置在文档的 <head> 部分或 <body> 部分。以下是在文档头部添加嵌入式CSS样式的基本语法：

```
html<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  
  <!-- 使用 style 元素嵌入CSS样式 -->
  <style type="text/css">
    /* CSS 样式规则 */
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
    }

    h1 {
      color: blue;
    }
  </style>
</head>
<body>
  <!-- 页面内容 -->
</body>
</html>
```

在上面的例子中，`<style>` 元素的 `type` 属性指定了样式表的类型为CSS。在 `<style>` 元素内部，可以编写CSS样式规则，就像在外部样式表或独立的CSS文件中一样。

**注意：**

- 使用外部样式表的优势在于样式可以在多个页面之间共享，并且使得HTML文档更为清晰和可维护。
- 使用嵌入式样式表的优势在于它将HTML和CSS放在同一个文件中，适用于较小规模的项目或需要特定样式的单个页面。

### How Selector Works?

1. CSS选择器（Selector）用于选择要应用样式的HTML元素。选择器的工作原理是根据选择器的类型和匹配规则，选择文档中的特定元素。以下是一些常见的CSS选择器及其工作原理：

#### 1. 通用选择器 `*`

   `*` 选择器匹配文档中的所有元素。

   ```
   * {
     /* 应用于所有元素的样式规则 */
   }
   ```

#### 2. 标签选择器 `tag`

   标签选择器选择特定类型的元素。

   ```
   p {
     /* 应用于所有 <p> 元素的样式规则 */
   }
   ```

#### 3. 类选择器 `.class`、标签与类选择器 `tag.class`

   类选择器选择具有特定类的元素，标签与类选择器选择特定标签下带有特定类的元素。

   ```
   .button {
     /* 应用于所有类为 button 的元素的样式规则 */
   }
   
   h1.title {
     /* 应用于所有 <h1> 标签且类为 title 的元素的样式规则 */
   }
   ```

#### 4. ID 选择器 `#id`

   ID选择器选择具有特定ID的元素。

   ```
   #header {
     /* 应用于 ID 为 header 的元素的样式规则 */
   }
   ```

#### 5. 子元素选择器 `parent > sub`

   子元素选择器选择作为指定父元素的直接子元素的元素。

   ```
   nav > ul {
     /* 应用于所有 <ul> 元素，但仅在其直接位于 <nav> 下时生效 */
   }
   ```

#### 6. 后代元素选择器 `parent nestedtag`

   后代元素选择器选择指定祖先元素内的所有后代元素。

   ```
   article p {
     /* 应用于所有 <p> 元素，但仅在其位于 <article> 元素内时生效 */
   }
   ```

#### 7. 相邻兄弟选择器 `tag+nexttag`

   相邻兄弟选择器选择紧接在指定元素后的相邻元素。

   ```
   h2 + p {
     /* 应用于紧接在 <h2> 元素后的第一个 <p> 元素 */
   }
   ```

#### 8. 通用兄弟选择器 `tag~siblingtag`

   通用兄弟选择器选择指定元素之后的所有兄弟元素。

   ```
   h2 ~ p {
     /* 应用于 <h2> 元素后的所有 <p> 兄弟元素 */
   }
   ```

#### 9. 属性选择器 `tag[attribute]`

   属性选择器选择具有指定属性的元素。

   ```
   input[type] {
     /* 应用于所有带有 type 属性的 <input> 元素 */
   }
   ```

#### 10. 属性值选择器 `tag[attribute=value]`

   属性值选择器选择具有指定属性和属性值的元素。

   ```
   a[href="https://example.com"] {
     /* 应用于所有链接到 "https://example.com" 的 <a> 元素 */
   }
   ```

#### 11. 包含属性值选择器 `tag[attribute~=value]`

   包含属性值选择器选择具有指定属性，并且该属性的值包含指定词汇的元素。

   ```
   p[class~="important"] {
     /* 应用于所有类属性中包含 "important" 的 <p> 元素 */
   }
   ```

#### 12. 属性值前缀选择器 `tag[attribute^=value]`

   属性值前缀选择器选择具有以指定值开头的属性值的元素。

   ```
   a[href^="https://"] {
     /* 应用于所有链接到以 "https://" 开头的地址的 <a> 元素 */
   }
   ```

#### 13. 属性值后缀选择器 `tag[attribute$=value]`

   属性值后缀选择器选择具有以指定值结尾的属性值的元素。

   ```
   img[src$=".png"] {
     /* 应用于所有引用以 ".png" 结尾的图片的 <img> 元素 */
   }
   ```

#### 14. 属性值包含选择器 `tag[attribute*=value]`

   属性值包含选择器选择具有包含指定值的属性值的元素。

   ```
   a[href*="example"] {
     /* 应用于所有链接到包含 "example" 的地址的 <a> 元素 */
   }
   ```

   CSS选择器的灵活性允许开发人员以多种方式选择和定位页面中的元素，从而实现对页面样式的精确控制。

## 颜色（Color）

#### 颜色属性（Color Properties）

- **文本颜色（Text Color）**：通过 `color` 属性设置文本的颜色。可以使用颜色名称、十六进制值、RGB 值等表示。例如：

  ```
  p {
    color: red;
  }
  ```

- **背景颜色（Background Color）**：通过 `background-color` 属性设置元素的背景颜色。同样，可以使用不同的表示方法。例如：

  ```
  div {
    background-color: #f0f0f0;
  }
  ```

#### 透明度（Opacity）

- **透明度（Opacity）**：通过 `opacity` 属性设置元素的透明度。值为 0.0 到 1.0 之间的数字，0.0 表示完全透明，1.0 表示完全不透明。例如：

  ```
  div {
    opacity: 0.7;
  }
  ```

- **RGBA 颜色表示**：使用 `rgba` 函数表示颜色，其中 `a` 代表 alpha 通道（透明度）。例如：

  ```
  div {
    background-color: rgba(255, 0, 0, 0.5); /* 半透明红色背景 */
  }
  ```

#### HSL 和 HSLA 表示法

- **HSL 颜色表示**：使用 `hsl` 函数表示颜色，分别设置色相（Hue）、饱和度（Saturation）、亮度（Lightness）。例如：

  ```
  div {
    background-color: hsl(120, 100%, 50%); /* 绿色背景 */
  }
  ```

- **HSLA 颜色表示**：在 `hsl` 的基础上增加 alpha 通道。例如：

  ```
  div {
    background-color: hsla(120, 100%, 50%, 0.7); /* 半透明绿色背景 */
  }
  ```

以上是关于颜色的一些常见CSS技术，通过灵活运用这些属性，可以创建丰富多彩的界面效果。

## 文本和字体（Text and Font）

#### 字体族（Font Family）

`font-family` 属性用于设置文本的字体族。可以指定多个字体，以备选项的形式存在，以确保在用户计算机上始终能够找到合适的字体。例如：

```
body {
  font-family: 'Arial', 'Helvetica', sans-serif;
}
```

#### 字体大小（Font Size）

`font-size` 属性用于设置文本的大小，可以使用像素（px）、百分比（%）、相对长度单位（em）等。例如：

```
p {
  font-size: 16px;
}
```

#### 字体引入（@font-face）

`@font-face` 规则允许自定义字体文件，以便在网页上使用。例如：

```
@font-face {
  font-family: 'CustomFont';
  src: url('custom-font.woff') format('woff');
}
body {
  font-family: 'CustomFont', sans-serif;
}
```

#### 字体粗细（Font Weight）

`font-weight` 属性用于设置文本的粗细，可以是数字值，也可以是关键字如 `normal` 或 `bold`。例如：

```
strong {
  font-weight: bold;
}
```

#### 字体样式（Font Style）

`font-style` 属性用于设置文本的样式，如斜体。例如：

```
em {
  font-style: italic;
}
```

#### 字体变形（Text Transform）

`text-transform` 属性用于控制文本的大小写。例如：

```
span {
  text-transform: uppercase;
}
```

#### 文本装饰（Text Decoration）

`text-decoration` 属性用于控制文本的装饰效果，如下划线、删除线等。例如：

```
a {
  text-decoration: none;
}
```

#### 行高（Line Height）

`line-height` 属性用于设置行高，最好使用相对长度单位（如 em）以提高可伸缩性。例如：

```
p {
  line-height: 1.5;
}
```

#### 字母和单词间距（Letter and Word Spacing）

- **字母间距（Letter Spacing）**：`letter-spacing` 属性用于设置字母之间的间距。例如：

  ```
  h1 {
    letter-spacing: 2px;
  }
  ```

- **单词间距（Word Spacing）**：`word-spacing` 属性用于设置单词之间的间距。例如：

  ```
  p {
    word-spacing: 5px;
  }
  ```

#### 文本对齐（Text Align）

`text-align` 属性用于设置文本的对齐方式，如左对齐、右对齐、居中等。例如：

```
div {
  text-align: center;
}
```

#### 垂直对齐（Vertical Align）

`vertical-align` 属性用于设置内联元素的垂直对齐方式。例如：

```
img {
  vertical-align: middle;
}
```

#### 文本缩进（Text Indent）

`text-indent` 属性用于设置文本的首行缩进。例如：

```
p {
  text-indent: 20px;
}
```

#### 文本阴影（Text Shadow）

`text-shadow` 属性用于设置文本的阴影效果，包括阴影方向、偏移、大小和颜色。例如：

```
h1 {
  text-shadow: 2px 2px 4px #999999;
}
```

#### 伪元素（Pseudo Elements）

- `:first-letter`：用于选择文本的第一个字母。
- `:first-line`：用于选择文本的第一行。

```
p:first-letter {
  font-size: 150%;
}

p:first-line {
  color: blue;
}
```

#### 伪类（Pseudo Classes）

- `:link` 和 `:visited`：分别用于选择未访问和已访问的链接。
- `:hover`、 `:active`、 `:focus`：用于响应用户的鼠标悬停、激活和焦点状态。

```
a:link {
  color: blue;
}

a:hover {
  color: red;
}

a:visited {
  color: purple;
}
```

以上是一些关于文本和字体样式的常见CSS技术，它们对于创建吸引人的页面内容至关重要。

## 盒子模型（Box Model）

#### 尺寸属性（Dimension Properties）

- `width`、`min-width`、`max-width`：分别用于设置元素的宽度、最小宽度和最大宽度。例如：

  ```
  div {
    width: 300px;
    min-width: 100px;
    max-width: 500px;
  }
  ```

- `height`、`min-height`、`max-height`：分别用于设置元素的高度、最小高度和最大高度。例如：

  ```
  div {
    height: 200px;
    min-height: 50px;
    max-height: 300px;
  }
  ```

#### 溢出处理（Overflow）

`overflow` 属性用于控制当内容溢出容器时的处理方式。例如：

```
div {
  overflow: hidden; /* 或者 overflow: scroll; */
}
```

#### 内边距、边框、外边距（Padding, Border, Margin）

- **内边距（Padding）**：`padding` 属性用于设置元素内部内容与边框之间的空白区域。可以分别设置上、右、下、左的内边距。例如：

  ```
  div {
    padding: 10px 20px 15px 5px;
  }
  ```

- **边框（Border）**：`border` 属性用于设置元素的边框，包括宽度、样式和颜色。例如：

  ```
  div {
    border: 2px solid #000;
  }
  ```

  - **边框样式（Border Style）**：`border-style` 属性定义边框的样式，如实线、虚线等。例如：

    ```
    div {
      border-style: dashed;
    }
    ```

  - **边框颜色（Border Color）**：`border-color` 属性定义边框的颜色。例如：

    ```
    div {
      border-color: #00f;
    }
    ```

- **外边距（Margin）**：`margin` 属性用于设置元素与相邻元素之间的空白区域。可以分别设置上、右、下、左的外边距。例如：

  ```
  div {
    margin: 10px 20px 15px 5px;
  }
  ```

#### 显示属性（Display Properties）

`display` 属性用于设置元素的显示方式，包括块级元素、内联元素、内联块级元素等。例如：

```
div {
  display: block; /* 或者 display: inline; */
}
```

- **可见性（Visibility）**：`visibility` 属性用于控制元素的可见性，可以是隐藏或可见。例如：

  ```
  div {
    visibility: hidden;
  }
  ```

#### 边框图片（Border Image）

`border-image` 属性用于设置边框的图片样式，包括URL、拉伸、重复等。例如：

```
div {
  border-image: url('border-image.png') 30 30 round;
}
```

#### 盒子阴影和圆角（Box Shadow and Border Radius）

- **盒子阴影（Box Shadow）**：`box-shadow` 属性用于创建元素的阴影效果。例如：

  ```
  div {
    box-shadow: 5px 5px 10px #888888;
  }
  ```

- **圆角（Border Radius）**：`border-radius` 属性用于设置元素的边框角的圆角程度。可以分别设置水平和垂直方向的圆角半径。例如：

  ```
  div {
    border-radius: 10px 20px;
  }
  ```

以上是有关盒子模型的一些常见CSS技术，它们对于布局和样式设计中起到了关键的作用。

## 列表、表格和表单（List, Table, and Form）

#### 列表样式（List Style）

列表样式用于定义列表项的外观。它包括以下属性：

- `list-style-type`：指定列表项的标志类型，如圆点、数字、字母等。例如：

  ```
  ul {
    list-style-type: circle;
  }
  ```

- `list-style-image`：用图像替代列表项的标志。例如：

  ```
  ul {
    list-style-image: url('bullet.png');
  }
  ```

- `list-style-position`：控制列表项标志的位置，可以是内部或外部。例如：

  ```
  ul {
    list-style-position: inside;
  }
  ```

#### 空单元格处理（Empty Cells）

`empty-cells` 属性用于控制表格中空单元格的显示。例如：

```
table {
  empty-cells: hide;
}
```

#### 表格边框和间距（Border and Spacing in Tables）

- `border-spacing`：设置相邻单元格之间的边框间距。例如：

  ```
  table {
    border-spacing: 5px;
  }
  ```

- `border-collapse`：定义表格的边框模型，可以是分离的（separate）或合并的（collapse）。例如：

  ```
  table {
    border-collapse: collapse;
  }
  ```

#### 表单布局（Form Layout）

表单元素的布局可以通过不同的CSS属性来实现。以下是一些常用的属性：

- `float`：通过浮动来布局表单元素。例如：

  ```
  input {
    float: left;
  }
  ```

- `cursor`：定义鼠标悬停在表单元素上时的光标形状。例如：

  ```
  button {
    cursor: pointer;
  }
  ```

- `auto`：浏览器设置默认的光标形状。例如：

  ```
  input {
    cursor: auto;
  }
  ```

- `crosshair`、`default`、`pointer`、`move`、`text`、`wait`、`help`：分别设置光标形状为十字线、默认、指针、移动、文本输入、等待、帮助。例如：

  ```
  a {
    cursor: pointer;
  }
  ```

- `url("")`：通过指定自定义光标的URL来设置光标形状。例如：

  ```
  a {
    cursor: url('custom-cursor.png'), auto;
  }
  ```

以上是一些与列表、表格和表单相关的常见CSS技术，它们有助于定制化这些元素的外观和布局。

## 布局和定位（Layout and Position）

#### 静态流动（Static）

静态流动是元素默认的定位方式。块级元素（block）会独占一行，而行内元素（inline）则在同一行内排列。例如：

```
div {
  display: block; /* 或者 display: inline; */
}
```

#### 相对定位（Relative）

相对定位是相对于元素在文档流中的原始位置进行定位。通过使用 `position: relative;` 属性，你可以使用 `top`、`right`、`bottom` 和 `left` 属性来调整元素的位置。例如：

```
div {
  position: relative;
  top: 10px;
  left: 20px;
}
```

#### 绝对定位（Absolute）

绝对定位是相对于最近的非静态定位祖先元素进行定位，如果没有这样的祖先元素，它将相对于文档的初始包含块。例如：

```
div {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

##### 绝对定位的变种

- **跟随页面滚动（Absolute）**

  当页面滚动时，元素保持在相对于视口的固定位置。例如：

  ```
  div {
    position: absolute;
    top: 10px;
    left: 10px;
  }
  ```

- **固定位置（Fixed Position）**

  元素相对于视口固定，不随页面滚动而变化。例如：

  ```
  div {
    position: fixed;
    top: 0;
    left: 0;
  }
  ```

#### 浮动定位（Float Position）

浮动是一种使元素脱离正常文档流，向左或向右移动的布局方式。在浮动元素周围的文本和内联元素将围绕着它。例如：

```
img {
  float: left;
}
```

#### 层叠顺序（Z-Index）

`z-index` 属性用于控制元素的层叠顺序。具有较高 `z-index` 值的元素将显示在具有较低 `z-index` 值的元素之上。例如：

```
div {
  z-index: 1;
}
```

#### 清除浮动（Clear）

`clear` 属性用于控制元素的浮动行为。它指定了在元素旁边不允许浮动元素的一侧。例如：

```
div {
  clear: both;
}
```

以上是有关布局和定位的一些常见CSS技术，它们对于创建灵活和响应式的页面布局至关重要。

## 图片（Image）

#### 尺寸（Size）

在CSS中，你可以使用 `width` 和 `height` 属性来设置图像的尺寸。例如：

```
img {
  width: 100px;
  height: 100px;
}
```

#### 对齐（Align）

通过使用 `float` 或 `display: flex`，你可以控制图像在其容器中的对齐方式。例如：

```
img {
  float: left;
  /* 或者使用 flexbox */
  display: flex;
  align-items: center;
  justify-content: center;
}
```

### 背景（Background）

#### 背景图像（Background Image）

使用 `background-image` 属性可以设置元素的背景图像。例如：

```
div {
  background-image: url('example.jpg');
}
```

#### 背景颜色（Background Color）

通过 `background-color` 属性，你可以设置元素的背景颜色。例如：

```
div {
  background-color: #f0f0f0;
}
```

#### 背景重复（Background Repeat）

使用 `background-repeat` 属性可以控制背景图像的重复方式。例如：

```
div {
  background-repeat: repeat-x; /* 水平重复 */
}
```

#### 背景附着（Background Attachment）

通过 `background-attachment` 属性，你可以设置背景图像是随着页面滚动还是固定在一个位置。例如：

```
div {
  background-attachment: fixed;
}
```

#### 线性渐变（Linear Gradient）

使用 `linear-gradient` 属性，你可以创建线性渐变的背景。例如：

```
div {
  background: linear-gradient(to right, #ff0000, #00ff00);
}
```

## 伪类（Pseudo-classes）

#### 悬停状态（:hover）

`:hover` 伪类用于在用户悬停在元素上时应用样式。例如：

```
a:hover {
  color: #ff0000;
}
```

#### 激活状态（:active）

`:active` 伪类用于在用户点击并按住鼠标按钮时应用样式。例如：

```
button:active {
  background-color: #00ff00;
}
```

这些是CSS中一些常见的图像和背景处理技术，以及一些常用的伪类，它们有助于创建吸引人的界面和交互效果。

## 补充和进阶

## 伪类

在CSS（层叠样式表）中，伪类（pseudo-class）是一种用于选择元素的特殊选择器。伪类不是实际存在于文档中的元素，而是表示元素的特定状态或位置关系。它们允许你选择不同状态下的元素，而无需修改HTML结构。

以下是一些常见的CSS伪类：

1. **:hover** - 鼠标悬停在元素上时应用的样式。

   ```
   a:hover {
     color: red;
   }
   ```

2. **:active** - 用户点击元素但尚未释放鼠标按钮时应用的样式。

   ```
   button:active {
     background-color: yellow;
   }
   ```

3. **:focus** - 元素获得焦点时应用的样式，通常用于表单元素。

   ```
   input:focus {
     border: 2px solid blue;
   }
   ```

4. **:first-child** - 选择元素的第一个子元素。

   ```
   li:first-child {
     font-weight: bold;
   }
   ```

5. **:last-child** - 选择元素的最后一个子元素。

   ```
   div p:last-child {
     margin-bottom: 0;
   }
   ```

6. **:nth-child(n)** - 选择元素的第 n 个子元素。

   ```
   li:nth-child(odd) {
     background-color: lightgray;
   }
   ```

   在这个例子中，奇数位置的 `li` 元素会有灰色背景。

7. **:nth-of-type(n)** - 选择相同类型的元素中的第 n 个元素。

   ```
   p:nth-of-type(2) {
     color: red;
   }
   ```

   在这个例子中，文档中的第二个 `p` 元素文本颜色会变为红色。

这些只是一些常见的伪类，还有其他伪类可用于更复杂的选择。伪类是CSS中强大而灵活的工具，它们使得可以根据元素的状态或位置更精确地选择和样式化元素。

CSS伪类可以分为几个不同类型，其中之一是“状态型”伪类。这些伪类基于元素的状态或用户与元素的交互来选择元素。以下是一些常见的状态型伪类：

1. **:hover**：当用户将鼠标悬停在元素上时应用的样式。常用于创建交互式效果，例如按钮在鼠标悬停时改变颜色。

   ```
   button:hover {
     background-color: #3498db;
     color: #fff;
   }
   ```

2. **:active**：当元素处于活动（被点击但尚未释放）状态时应用的样式。通常用于创建按钮被点击时的样式。

   ```
   button:active {
     background-color: #e74c3c;
     color: #fff;
   }
   ```

3. **:focus**：当元素获得焦点时应用的样式。常用于增强表单元素的可访问性，使用户知道当前哪个输入字段处于焦点状态。

   ```
   input:focus {
     border: 2px solid #3498db;
   }
   ```

4. **:visited**：选择已被访问的链接。这使得可以为已访问和未访问的链接应用不同的样式。

   ```
   a:visited {
     color: purple;
   }
   ```

5. **:link** 和 **:visited**：分别选择未被访问的链接和已被访问的链接。这两者通常与`:hover`和`:active`一起使用，以创建链接的完整状态样式。

   ```
   a:link {
     color: blue;
   }
   
   a:visited {
     color: purple;
   }
   
   a:hover {
     color: red;
   }
   
   a:active {
     color: orange;
   }
   ```

这些状态型伪类允许你根据用户的交互或元素的状态动态地应用样式，以改变页面的外观和行为。

1. **:hover**：

   - 描述：当用户将鼠标悬停在元素上时应用的样式。
   - 用例：用于创建交互式效果，例如在悬停时改变链接或按钮的颜色。

   ```
   button:hover {
     background-color: #3498db;
     color: #fff;
   }
   ```

2. **:active**：

   - 描述：当元素处于活动状态（被点击但尚未释放）时应用的样式。
   - 用例：用于创建按钮被点击时的样式。

   ```
   button:active {
     background-color: #e74c3c;
     color: #fff;
   }
   ```

3. **:focus**：

   - 描述：当元素获得焦点时应用的样式。通常用于增强表单元素的可访问性。
   - 用例：用于突出当前输入字段。

   ```
   input:focus {
     border: 2px solid #3498db;
   }
   ```

4. **:visited**：

   - 描述：选择已被访问的链接。
   - 用例：用于为已访问和未访问的链接应用不同的样式。

   ```
   a:visited {
     color: purple;
   }
   ```

5. **:checked**：

   - 描述：选择被选中的表单元素，如复选框或单选按钮。
   - 用例：用于在选择某个选项时应用样式。

   ```
   input[type="checkbox"]:checked {
     background-color: #2ecc71;
   }
   ```

6. **:enabled**：

   - 描述：选择处于启用状态的表单元素。
   - 用例：用于在表单元素启用时应用样式。

   ```
   input:enabled {
     border: 1px solid #3498db;
   }
   ```

7. **:disabled**：

   - 描述：选择处于禁用状态的表单元素。
   - 用例：用于在表单元素禁用时应用样式。

   ```
   input:disabled {
     background-color: #ecf0f1;
   }
   ```

这些伪类使得可以根据元素的状态或用户与元素的交互来动态地应用样式，从而增加页面的交互性和可访问性。

1. **::before**：

   - 描述：在元素的内容之前插入生成的内容。
   - 用例：用于在元素前面添加装饰性内容，例如图标或引用符号。

   ```
   p::before {
     content: "\201C"; /* 左双引号 */
   }
   ```

2. **::after**：

   - 描述：在元素的内容之后插入生成的内容。
   - 用例：用于在元素后面添加额外的内容，比如清除浮动或添加尾随图标。

   ```
   p::after {
     content: "\201D"; /* 右双引号 */
   }
   ```

3. **::first-line**：

   - 描述：选择元素的第一行并应用样式。
   - 用例：用于改变段落的首行样式，如字体大小或颜色。

   ```
   p::first-line {
     font-weight: bold;
   }
   ```

4. **::first-letter**：

   - 描述：选择元素的第一个字母并应用样式。
   - 用例：用于创建首字母大写或添加特殊样式的效果。

   ```
   p::first-letter {
     font-size: 1.5em;
     color: #3498db;
   }
   ```

5. **::selection**：

   - 描述：选择用户选择的文本部分并应用样式。
   - 用例：用于自定义用户选择文本时的背景和文本颜色。

   ```
   ::selection {
     background-color: #3498db;
     color: #fff;
   }
   ```

这些伪元素允许你选择元素的特定部分并对其应用样式，从而提供更多样式化的可能性。每个伪元素都有其独特的应用场景和效果。

## Transform

在CSS中，`transform`属性用于对元素进行平移（translate）、缩放（scale）、旋转（rotate）、扭曲（skew）和透视（perspective）等变换操作。这些变换可以单独应用或组合在一起，以创建各种视觉效果。下面是对每个变换的简要说明：

1. **平移（Translate）**：

   - 描述：通过指定元素在水平和垂直方向上的偏移来移动元素。
   - 语法：`translate(x, y)`，其中 `x` 和 `y` 分别是水平和垂直方向上的偏移值。

   ```
   .box {
     transform: translate(50px, 20px);
   }
   ```

2. **缩放（Scale）**：

   - 描述：通过指定元素在水平和垂直方向上的缩放比例来调整元素的大小。
   - 语法：`scale(x, y)`，其中 `x` 和 `y` 分别是水平和垂直方向上的缩放比例。

   ```
   .box {
     transform: scale(1.5, 2);
   }
   ```

3. **旋转（Rotate）**：

   - 描述：通过指定元素的旋转角度来旋转元素。
   - 语法：`rotate(angle)`，其中 `angle` 是旋转的角度。

   ```
   .box {
     transform: rotate(45deg);
   }
   ```

4. **扭曲（Skew）**：

   - 描述：通过指定元素在水平和垂直方向上的倾斜角度来扭曲元素。
   - 语法：`skew(x-angle, y-angle)`，其中 `x-angle` 和 `y-angle` 分别是水平和垂直方向上的倾斜角度。

   ```
   .box {
     transform: skew(30deg, 20deg);
   }
   ```

5. **透视（Perspective）**：

   - 描述：通过指定透视距离来创建透视效果，影响 3D 变换的效果。
   - 语法：`perspective(length)`，其中 `length` 是透视距离。

   ```
   .container {
     perspective: 1000px;
   }
   ```

这些变换可以单独使用，也可以组合在一起。例如，可以在一个规则中同时使用 `translate`、`rotate` 和 `scale` 来实现多个变换效果。CSS变换为Web开发者提供了强大的工具，用于实现各种交互和动画效果。

#### Transision

在CSS中，`transition`是一种用于在元素状态发生变化时平滑过渡效果的属性。通过使用`transition`属性，可以定义元素的属性在发生变化时应用过渡效果，而不是突然改变。

`transition`属性通常与伪类（例如`:hover`）一起使用，以在元素状态变化时提供平滑的过渡。以下是`transition`属性的基本语法：

```
selector {
  transition: property duration timing-function delay;
}
```

- `property`：要过渡的CSS属性，如`color`、`opacity`、`transform`等。
- `duration`：过渡的持续时间，以秒（s）或毫秒（ms）为单位。
- `timing-function`：过渡的时间函数，控制过渡的速度曲线（例如线性、ease-in、ease-out等）。
- `delay`：过渡开始之前的延迟时间，以秒（s）或毫秒（ms）为单位。

以下是一个简单的示例，演示了当鼠标悬停在一个按钮上时，背景颜色会平滑过渡变化：

```
button {
  background-color: #3498db;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #e74c3c;
}
```

在这个例子中，当鼠标悬停在按钮上时，`background-color`属性将以`ease`的时间函数在0.3秒内从蓝色平滑过渡到红色。

通过使用`transition`属性，可以增强用户体验，使页面元素状态变化更加流畅和自然。此属性广泛用于实现按钮、链接和其他用户界面元素的动画效果。

## 动画

在CSS中，`@keyframes` 和 `animation` 属性用于创建和应用动画。`@keyframes`规则定义动画的关键帧，而 `animation` 属性用于指定动画的名称、持续时间、时间函数、延迟、迭代次数、方向和填充模式等。

### @keyframes 规则

`@keyframes` 规则用于定义动画的关键帧，即在动画过程中的不同阶段。它的基本语法如下：

```
@keyframes animationName {
  from {
    /* styles at the beginning of the animation */
  }

  to {
    /* styles at the end of the animation */
  }

  /* or use percentage for intermediate keyframes */
  25% {
    /* styles at 25% of the animation */
  }

  /* additional keyframes as needed */
}
```

### animation 属性

`animation` 属性用于将动画应用于元素。其基本语法如下：

```
selector {
  animation: name duration timing-function delay iteration-count direction fill-mode;
}
```

- `name`：指定要应用的 `@keyframes` 规则的名称。
- `duration`：动画的持续时间，以秒（s）或毫秒（ms）为单位。
- `timing-function`：动画的时间函数，控制动画的速度曲线（例如 `ease`、`linear`、`ease-in` 等）。
- `delay`：动画开始前的延迟时间，以秒（s）或毫秒（ms）为单位。
- `iteration-count`：动画的迭代次数，可以是具体次数或 `infinite` 表示无限次。
- `direction`：动画的播放方向，可以是 `normal`（正常播放）、`reverse`（反向播放）、`alternate`（交替正反播放）等。
- `fill-mode`：动画执行前和执行后的样式，可以是 `forwards`、`backwards`、`both` 或 `none`。

以下是一个简单的例子，演示了一个使用 `@keyframes` 和 `animation` 属性的动画：

```
@keyframes slide-in {
  from {
    transform: translateX(-100%);
  }

  to {
    transform: translateX(0);
  }
}

.slide-in {
  animation: slide-in 1s ease-out;
}
```

在这个例子中，一个名为 `slide-in` 的关键帧规则定义了一个元素从左侧滑入的动画，然后通过 `.slide-in` 类将这个动画应用到特定的元素上。

## 字库

```
@font-face {
  font-family: fnt;
  src: url(../remixicon.woff) format("woff");
}
```

- `@font-face` 规则是用于定义字体的规则，使得你可以使用自定义字体。
- `font-family` 属性定义了字体的名称，这个名称可以在后续的 CSS 规则中使用。
- `src` 属性指定了字体文件的路径和格式。在这个例子中，字体文件是 `remixicon.woff`，它使用 WOFF 格式（Web Open Font Format）。

然后，你可以在其他地方的样式规则中使用 `font-family: fnt;` 来引用这个自定义字体，例如：

```
body {
  font-family: fnt, sans-serif;
}
```

这会将 `fnt` 字体应用于页面的主体文本，如果字体不可用，那么将回退到系统默认的 sans-serif 字体。

## CSS 结构规划

CSS的结构规划对于项目的可维护性和团队协作至关重要。以下是一些关于引入方式、作用域和团队协作的考虑：

### 引入方式

1. **内联样式（Inline Styles）：**

   - **语法：** `style="..."`。
   - **特点：** 样式与HTML元素直接关联，不推荐在大型项目中使用，因为难以维护。

   ```
   html
   <p style="color: red; font-size: 16px;">This is a paragraph.</p>
   ```

2. **嵌入样式（Embedded Styles）：**

   - **语法：** `<style>...</style>`。
   - **特点：** 样式写在HTML文档的头部，适用于小型项目或需要页面特定样式的情况。

   ```
   html<head>
     <style>
       p {
         color: blue;
         font-size: 18px;
       }
     </style>
   </head>
   ```

3. **外部样式表（External Stylesheet）：**

   - **语法：** `<link rel="stylesheet" type="text/css" href="style.css">`。
   - **特点：** 样式定义在独立的CSS文件中，适用于大型项目和样式共享。

   ```
   html<head>
     <link rel="stylesheet" type="text/css" href="style.css">
   </head>
   ```

### 作用域

1. **类选择器 `.class` vs ID 选择器 `#id` vs 属性选择器 `[...]`：**

   - **类选择器：** 适用于多个元素共享相似样式的情况。
   - **ID 选择器：** 应该避免过度使用，因为ID在整个页面中是唯一的，可能导致样式不可复用，容易发生命名冲突。
   - **属性选择器：** 适用于根据元素的属性选择样式，例如 `[disabled]`。

   ```
   .highlight {
     color: red;
   }
   
   #header {
     font-size: 20px;
   }
   
   [disabled] {
     opacity: 0.5;
   }
   ```

2. **路径限制作用域：**

   - 通过合理的CSS选择器路径，限制样式的作用域，避免全局定义。
   - 避免过于宽泛的选择器，以免影响到其他模块的样式。

   ```
   .section1 .content {
     /* 样式规则 */
   }
   ```

### 团队协作

1. **规范和命名约定：**
   - 制定明确的CSS规范和命名约定，确保团队成员有一致的样式书写风格。
   - 使用有意义的类名和ID，避免单个字母或缩写，提高代码可读性。
2. **模块化和组件化：**
   - 将样式分为模块或组件，使其易于维护和复用。
   - 可以考虑使用CSS预处理器（如Sass或Less）来实现模块化。
3. **版本控制：**
   - 使用版本控制系统（如Git）管理样式表，确保团队成员能够协同工作并追踪变更历史。
4. **代码审查：**
   - 定期进行代码审查，确保符合团队规范，并且样式表的结构清晰、合理。
5. **文档和注释：**
   - 添加注释和文档，解释样式表的结构、作用和用法，方便团队成员理解和使用。

综合考虑引入方式、作用域和团队协作，可以建立一个清晰、可维护且协作良好的CSS结构，提高项目的开发效率和代码质量。

## CSS 浏览器私有前缀

浏览器私有前缀是为了兼容不同浏览器的特定CSS属性和规则。不同浏览器厂商在实现新的CSS属性或规则时可能存在一些差异，为了确保网页在不同浏览器中都能正常显示，开发者可以使用浏览器私有前缀。以下是一些主要浏览器的私有前缀：

- **WebKit（Chrome、Safari）:**
  - `-webkit-`
- **Mozilla Firefox:**
  - `-moz-`
- **Internet Explorer:**
  - `-ms-`
- **Opera:**
  - `-o-`

### CSS浏览器版本兼容方式

在写CSS样式时，通常会使用带有浏览器私有前缀的规则，以确保在各种浏览器中都能正确渲染。一种通用的方式是使用带前缀和不带前缀的规则，例如：

```
.transition {
  -webkit-transition: all .5s; /* Chrome, Safari */
  -moz-transition: all .5s;    /* Firefox */
  -o-transition: all .5s;      /* Opera */
  transition: all .5s;         /* Standard */
}
```

在这个例子中，`.transition` 类使用了带有不同私有前缀和不带前缀的 `transition` 属性。浏览器会选择解析符合其规范的属性，并忽略不认识的属性。这样，无论用户使用哪种浏览器，都能保证过渡效果的兼容性。当浏览器逐渐支持标准的写法时，可以逐步去掉私有前缀。
