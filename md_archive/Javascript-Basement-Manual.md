---
title: Javascript Basement Quick Overview - Interactive Front-end Development
date: 2023-11-07 20:58:48
tags: javascript
categories:
- 学习
- 计算机
- 前端
cover: https://bairesdev.mo.cloudinary.net/blog/2023/08/What-Is-JavaScript-Used-For.jpg?tx=w_3840,q_auto
---

js开发

<!--more-->

## Q&A

### JavaScript工作原理

JavaScript是一种用于网页交互的脚本语言，它主要通过以下步骤来工作：

1. **访问HTML (Visit HTML):** JavaScript通常嵌入在HTML文档中，并通过`<script>`标签嵌入到HTML代码中。当浏览器加载页面时，会解释并执行嵌入的JavaScript代码。

   示例：

   ```js
   html<!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>JavaScript Example</title>
   </head>
   <body>
       <!-- JavaScript代码嵌入在这里 -->
       <script>
           // JavaScript代码
       </script>
   </body>
   </html>
   ```

2. **修改内容 (Modify Content):** JavaScript可以通过操作文档对象模型（DOM）来动态修改网页内容。DOM表示网页的结构，通过JavaScript，可以添加、删除或修改HTML元素、属性和文本内容。

   示例：

   ```js
   javascript// 获取元素并修改内容
   var element = document.getElementById("myElement");
   element.innerHTML = "新的内容";
   ```

3. **制定规则 (Make Rules):** JavaScript用于制定网页的行为规则，包括对数据的处理、条件判断、循环等。这有助于实现动态和交互式的用户体验。

   示例：

   ```js
   javascript// 制定规则 - 条件判断
   var age = 20;
   if (age >= 18) {
       console.log("成年人");
   } else {
       console.log("未成年人");
   }
   ```

4. **响应事件 (Respond to Events):** JavaScript使网页能够对用户的交互作出响应，例如点击按钮、提交表单等。通过事件处理程序，可以定义在事件发生时执行的操作。

   示例：

   ```js
   html<!-- HTML中的按钮 -->
   <button id="myButton" onclick="myFunction()">点击我</button>
   
   <!-- JavaScript中的事件处理程序 -->
   <script>
       function myFunction() {
           alert("按钮被点击了！");
       }
   </script>
   ```

这些步骤使JavaScript成为一种强大的客户端脚本语言，为网页提供了丰富的交互和动态性。

### 什么是脚本？

**脚本（Script）** 是一系列命令或指令的集合，通常编写成文本文件。这些命令按照一定的顺序执行，用于完成特定的任务或操作。脚本通常用于自动化任务、批处理处理、或在特定条件下触发一系列操作。

在计算机编程领域，脚本通常是解释性语言编写的，与编译型语言相对。脚本语言的特点是代码不需要事先编译成机器码，而是由解释器逐行解释执行。

对于JavaScript来说，它是一种脚本语言，用于在Web浏览器中添加交互性。JavaScript代码以脚本的形式嵌入在HTML文档中，由浏览器解释执行。这使得开发人员能够在网页上创建动态、交互式的用户体验，通过一系列的脚本命令来修改文档内容、响应事件等。

总体而言，脚本是一种轻量级的编程方式，适用于一些需要快速执行、适应变化的场景。

### 如何编写脚本？

编写脚本通常可以分为以下步骤：目标（Goal）-> 任务（Tasks）-> 编码（Coding）。

1. **明确目标 (Goal):** 首先，明确你的脚本的目标是什么。确定你想要实现的最终结果，这有助于指导后续的编码过程。

2. **分解任务 (Tasks):** 将整个目标分解为小的、可管理的任务。每个任务应该对应脚本中的一个功能或操作。这有助于组织代码，使其更易于理解和维护。

3. **编写代码 (Coding):** 针对每个任务，编写相应的代码来实现它。使用适当的编程语言，并根据任务的要求选择合适的数据结构、算法和控制流程。

   示例（伪代码）：

   ```plaintext
   plaintext// 目标：计算并输出两个数的和
   
   // 任务1: 获取用户输入
   输入第一个数
   输入第二个数
   
   // 任务2: 计算和
   和 = 第一个数 + 第二个数
   
   // 任务3: 输出结果
   输出和
   ```

   

4. **测试和调试 (Testing and Debugging):** 编写完代码后，进行测试以确保脚本按照预期工作。调试任何潜在的错误或问题，并确保脚本的稳定性和正确性。

5. **文档 (Documentation):** 为你的脚本编写文档，描述脚本的目的、用法和任何特殊注意事项。这有助于其他人理解和使用你的脚本。

6. **优化 (Optimization):** 针对性能和代码质量进行优化。检查是否有冗余的代码，是否有更有效的方法实现相同的功能。

记住，编写脚本是一个迭代的过程。在编码和测试过程中可能会发现一些需要调整的地方，因此保持灵活性并根据需要进行修改。

### 对象和属性

在计算机编程中，对象和属性是用于帮助计算机理解和处理世界的概念。

**对象 (Object):** 对象是现实生活中或计算机程序中的实体，可以具有状态和行为。在编程中，对象通常是具有相关属性和方法的实例。例如，一个表示汽车的对象可以有属性（颜色、型号）和方法（启动、停止）。

**属性 (Attribute):** 属性是对象的特征或状态，描述对象的某个方面。属性可以是对象的数据，例如颜色、大小、重量等。通过访问对象的属性，我们可以了解或修改对象的状态。

**事件 (Event):** 事件是对象发生的动作或事情，可以触发相应的响应。在编程中，事件通常与用户交互有关，例如点击按钮、输入文本等。处理事件的代码被称为事件处理程序。

例如（伪代码）：

```plaintext
plaintext// 创建汽车对象
car = {
    color: "blue",         // 属性: 颜色
    model: "sedan",        // 属性: 型号

    start: function() {    // 方法: 启动
        // 启动汽车的代码
    },

    stop: function() {     // 方法: 停止
        // 停止汽车的代码
    }
}

// 访问汽车对象的属性和方法
car.color             // 输出: "blue"
car.start()           // 启动汽车
```

通过使用对象、属性和方法，计算机可以模拟现实世界中的实体和动作，从而更好地理解和处理程序的逻辑。这种面向对象的编程方法有助于组织和抽象复杂的系统。

### 网页浏览器的工作原理

网页浏览器是用于显示和解释网页内容的软件应用程序。它的工作涉及多个对象和步骤。

**对象:**

1. **Window（窗口）:**
   - 代表浏览器窗口，是浏览器的顶层对象。它包含了整个浏览器窗口的信息，以及全局的JavaScript对象和方法。
2. **Document（文档）:**
   - 代表当前加载的网页文档，即HTML文档。它提供了对文档内容的访问和操作，如修改元素、添加事件等。

**步骤:**

1. **接收HTML（Receive an HTML）:**
   - 当用户在浏览器中输入URL或点击链接时，浏览器发送请求到服务器，并接收服务器返回的HTML文件。这个HTML文件包含了网页的结构和内容。
2. **建模和存储到内存（Modeling and Storage to Memory）:**
   - 浏览器解析HTML文档，构建文档对象模型（DOM）和样式表对象模型（CSSOM）。DOM表示网页的结构，CSSOM表示网页的样式。这些模型被存储在浏览器的内存中，以便后续的渲染过程使用。
3. **渲染（Rendering）:**
   - 浏览器通过将DOM和CSSOM合并成渲染树（Render Tree），然后通过布局（Layout）和绘制（Painting）的过程，将网页呈现到屏幕上。JavaScript代码也可能在这个阶段修改DOM，触发重新渲染。

这些步骤是简化的概括，实际上浏览器的工作涉及更多的细节和优化。浏览器还涉及其他对象和组件，如网络模块、解析器、JavaScript引擎等，以提供完整的浏览体验。

总体而言，浏览器的工作可以看作是将从服务器获取的HTML、CSS和JavaScript文件转化为用户可视化的网页。这个过程包括了解析、建模、存储和渲染等多个步骤。

### HTML、CSS和JS如何协同工作？

HTML、CSS和JavaScript通常一起协同工作，分别负责内容、视觉效果和交互动作。

1. **HTML（内容）:**
   - HTML（超文本标记语言）用于定义网页的结构和内容。它包含了页面上的各种元素，如文本、图像、链接等。HTML提供了页面的骨架，但它通常没有处理页面的外观和行为。
2. **CSS（视觉效果）:**
   - CSS（层叠样式表）用于控制HTML元素的样式和布局。通过选择器和规则，CSS可以指定元素的颜色、字体、大小、位置等样式。CSS为网页提供了外观和样式，使其更具吸引力和可读性。
3. **JavaScript（动作）:**
   - JavaScript是一种脚本语言，用于添加网页的交互性和动态性。它可以修改HTML和CSS，响应用户的操作，处理数据等。JavaScript通过DOM（文档对象模型）和CSSOM（样式表对象模型）与HTML和CSS进行交互，使网页更具活力。

### 如何连接JS和HTML？

在HTML文件中，通过`<script>`标签可以将JavaScript代码嵌入到HTML文档中。这可以在文档的头部或尾部完成，例如：

```html
html<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML, CSS, and JS</title>
    <!-- 连接JS文件 -->
    <script src="myscript.js"></script>
</head>
<body>
    <!-- 页面内容 -->
</body>
</html>
```

在上面的例子中，`myscript.js`是包含JavaScript代码的外部文件，通过`<script>`标签的`src`属性进行引用。

### 调试方法？

在调试过程中，可以使用以下方法：

- **console.log():** 在JavaScript代码中插入`console.log()`语句，将变量的值或特定信息输出到浏览器的开发者工具控制台，以便检查代码的执行过程。
- **浏览器开发者工具:** 现代浏览器提供了开发者工具，其中包含调试器。在调试器中，可以逐行执行代码、设置断点、监视变量等，以便更详细地分析和修复问题。可以通过按F12或右键点击页面并选择"检查"来打开开发者工具。

这些调试方法有助于识别和修复HTML、CSS和JavaScript代码中的错误，确保它们协同工作以实现预期的效果和功能。



## 基础的基础

在编程中，有一些基础的概念和操作，其中包括注释、变量和数据类型。

#### 注释（Comment）

注释用于在代码中添加说明性的文字，这些文字不会被计算机执行，而是用于帮助人们理解代码。在JavaScript中，单行注释使用`//`，多行注释使用`/* */`。

```
javascript// 这是单行注释

/*
   这是
   多行
   注释
*/
```

#### 变量（Variable）

变量用于存储和表示数据。在JavaScript中，使用`var`关键字来声明变量。变量可以存储不同数据类型的值，例如数字、字符串、数组等。

```
javascriptvar x = 5;         // 数字
var name = "John"; // 字符串
var numbers = [1, 2, 3]; // 数组
var status;        // 未定义的变量
```

#### 数据类型（Data Type）

JavaScript中有多种数据类型，其中包括：

- **数字（Number）:** 表示数值，如 `5` 或 `3.14`。
- **字符串（String）:** 表示文本，用引号括起来，如 `"Hello"`。
- **数组（Array）:** 用于存储多个值的有序集合，如 `[1, 2, 3]`。
- **未定义（Undefined）:** 表示变量没有被赋值。
- 等等...

```
javascriptvar num = 10;          // 数字
var greeting = "Hi";   // 字符串
var colors = ["red", "green", "blue"]; // 数组
var notDefined;        // 未定义
```

#### 尝试：

在JavaScript中，使用以下方法可以尝试操作HTML文档：

- **`document.getElementById()`:** 通过元素的ID获取HTML元素。
- **`document.write()`:** 将内容写入文档。
- **`[element].textContent = [\*]`:** 设置元素的文本内容。

```
javascript// 尝试获取ID为 "myElement" 的元素
var myElement = document.getElementById("myElement");

// 将文本写入文档
document.write("Hello, World!");

// 尝试设置元素的文本内容
myElement.textContent = "New Text";
```

这些基础操作为编写简单的JavaScript代码和与HTML文档交互提供了一些起点。



## 函数、方法和对象

### 函数（Function）

在JavaScript中，函数用于执行特定任务或操作。函数通常由函数名、参数和函数体组成。可以使用`return`语句返回值。示例：

```
javascript// 命名函数
function addNumbers(num1, num2) {
    var sum = num1 + num2;
    return sum;
}

// 调用函数
var result = addNumbers(3, 5);
console.log(result); // 输出: 8
```

匿名函数：

```
javascriptvar multiply = function(x, y) {
    return x * y;
};
var product = multiply(4, 6);
console.log(product); // 输出: 24
```

### 变量作用域

在JavaScript中，变量的作用域分为本地（局部）和全局两种。

- **本地作用域：** 在函数内声明的变量具有本地作用域，仅在该函数内部可见。

```
javascriptfunction example() {
    var localVar = "I am local";
    console.log(localVar);
}

example();      // 输出: "I am local"
console.log(localVar);  // 错误，localVar 在这里不可见
```

- **全局作用域：** 在函数外声明的变量具有全局作用域，可在整个程序中访问。

```
javascriptvar globalVar = "I am global";

function example() {
    console.log(globalVar);
}

example();      // 输出: "I am global"
console.log(globalVar);  // 输出: "I am global"
```

### 对象（Object）

对象是包含键值对的数据集合。在JavaScript中，对象可以包含属性和方法。

```
javascript// 对象字面量
var person = {
    firstName: "John",
    lastName: "Doe",
    sayHello: function() {
        console.log("Hello, " + this.firstName + " " + this.lastName);
    }
};

// 访问对象属性
console.log(person.firstName); // 输出: "John"

// 调用对象方法
person.sayHello(); // 输出: "Hello, John Doe"
```

对象也可以使用构造函数创建：

```
javascript// 构造函数
function Person(firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
}

// 创建对象实例
var person = new Person("John", "Doe");
console.log(person.firstName); // 输出: "John"
```

#### 访问对象属性

可以使用点号或方括号来访问对象的属性：

```
javascriptconsole.log(person.firstName); // 使用点号访问
console.log(person["firstName"]); // 使用方括号访问
```

#### 删除对象属性

可以使用 `delete` 关键字删除对象的属性：

```
javascript
delete person.lastName; // 删除 lastName 属性
```

这些是JavaScript中函数、作用域和对象的基本概念和用法。函数用于执行代码块，作用域定义了变量的可见范围，而对象用于组织和存储数据。

#### Built-in Objects

1. #### BOM - window

   ```js
   window.innerHeight;      // 浏览器窗口的内部高度
   window.innerWidth;       // 浏览器窗口的内部宽度
   window.pageXOffset;      // 窗口中内容横向滚动的像素值
   window.pageYOffset;      // 窗口中内容纵向滚动的像素值
   window.screenX;          // 窗口相对于屏幕左上角的横坐标
   window.screenY;          // 窗口相对于屏幕左上角的纵坐标
   window.location;         // 当前窗口的URL信息
   window.document;         // 表示文档对象
   window.history;          // 表示浏览器的历史记录对象
   window.history.length;   // 当前会话中的历史记录条数
   window.screen;           // 表示屏幕信息
   window.screen.width;     // 屏幕的宽度
   window.screen.height;    // 屏幕的高度
   window.alert();          // 显示警告对话框
   window.open();           // 打开新窗口
   window.print();          // 打印当前页面
   ```

   

#### DOM - Document

`<html>`

1. `<head>`

2. `<title>`

3. `<body>`

4. `<div>`
   
   1. attribute
   
5. `<p>`

6. text

   document.title: 获取或设置文档的标题。

   document.lastModified: 获取文档的上次修改日期和时间。

   document.URL: 获取文档的URL。

   document.domain: 获取或设置文档的域。

   document.write(): 向文档写入HTML内容。

   document.getElementById(): 通过元素的ID获取HTML元素。

   document.querySelectorAll(): 通过选择器获取匹配的所有元素。

   document.createElement(): 创建新的HTML元素。

   document.createTextNode(): 创建新的文本节点。

```js


示例：

javascript

console.log(document.title);             // 获取文档标题
console.log(document.lastModified);      // 获取上次修改时间
console.log(document.URL);                // 获取文档URL
console.log(document.domain);             // 获取文档域

document.write("Hello, World!");         // 向文档写入内容

var myElement = document.getElementById("myElement");  // 通过ID获取元素

var elements = document.querySelectorAll(".myClass");  // 通过类名获取元素

var newElement = document.createElement("div");        // 创建新元素
var newText = document.createTextNode("New Text");      // 创建新文本节点
```



#### 全局 JavaScript 对象

JavaScript 提供了一些全局对象，其中包括字符串、数字、布尔、日期、数学和正则表达式对象。以下是其中一些常见的全局对象及其方法：

1. **String（字符串）:**

   ```
   javascriptvar str = "Hello, World!";
   
   str.length;               // 字符串长度
   str.toUpperCase();        // 转换为大写
   str.toLowerCase();        // 转换为小写
   str.charAt(index);        // 获取指定位置的字符
   str.indexOf(substring);   // 查找子串第一次出现的位置
   str.lastIndexOf(substring); // 查找子串最后一次出现的位置
   str.substring(start, end); // 提取子串
   str.split(separator);      // 拆分字符串为数组
   str.trim();               // 去除字符串两端的空格
   str.replace(old, new);    // 替换字符串中的文本
   ```

2. **Number（数字）:**

   ```
   javascriptvar num = 42;
   
   isNaN(num);               // 判断是否为NaN
   num.toFixed(n);           // 将数字转为字符串，保留 n 位小数
   num.toPrecision(n);        // 将数字转为字符串，保留 n 位有效数字
   num.toExponential(n);      // 将数字转为指数形式的字符串，保留 n 位有效数字
   ```

3. **Boolean（布尔）:**

   JavaScript 中布尔对象没有明确的构造函数或方法，因为布尔值只有 `true` 和 `false`。

4. **Date（日期）:**

   ```
   javascriptvar today = new Date();
   
   today.getDate();          // 获取当前日期的天
   today.setDate(n);         // 设置当前日期的天
   today.getDay();           // 获取当前星期的天
   today.getFullYear();      // 获取当前年份
   today.setFullYear(year);  // 设置当前年份
   today.getHours();         // 获取当前小时
   today.setHours(hours);    // 设置当前小时
   // 更多方法...
   ```

5. **Math（数学）:**

   ```
   javascriptMath.PI;                  // 圆周率
   Math.round(n);            // 四舍五入
   Math.sqrt(n);             // 平方根
   Math.ceil(n);             // 向上取整
   Math.floor(n);            // 向下取整
   Math.random();            // 生成 0 到 1 之间的随机数
   // 更多方法...
   ```

6. **RegExp（正则表达式）:**

   正则表达式对象没有明确的构造函数，通常通过字面量或 `RegExp` 构造函数创建。

   ```
   javascriptvar pattern = /pattern/;
   var pattern = new RegExp("pattern");
   ```



## DOM（文档对象模型）

DOM（文档对象模型）是一种用于处理HTML和XML文档的编程接口。通过DOM，可以通过JavaScript脚本访问、修改文档的结构、样式和内容。以下是一些常见的DOM操作：

### 获取元素

- **document.getElementById():** 通过元素的ID获取单个元素。

  ```
  javascript
  var element = document.getElementById("myElement");
  ```

- **document.getElementsByTagName():** 通过标签名获取一组元素。

  ```
  javascript
  var elements = document.getElementsByTagName("p");
  ```

- **document.querySelector():** 通过CSS选择器获取单个元素。

  ```
  javascript
  var element = document.querySelector(".myClass");
  ```

- **document.querySelectorAll():** 通过CSS选择器获取一组元素。

  ```
  javascript
  var elements = document.querySelectorAll(".myClass");
  ```

- **document.getElementsByClassName():** 通过类名获取一组元素。

  ```
  javascript
  var elements = document.getElementsByClassName("myClass");
  ```

### 遍历（Traverse）

- **parentNode:** 获取父节点。
- **previousSibling:** 获取前一个同级节点。
- **nextSibling:** 获取后一个同级节点。
- **firstChild:** 获取第一个子节点。
- **lastChild:** 获取最后一个子节点。

### 获取和更新

- **nodeValue:** 获取或设置节点的值。
- **textContent:** 获取或设置节点的文本内容。
- **innerHTML:** 获取或设置节点的HTML内容。请谨慎使用，以防止XSS攻击。

### 添加和删除

- **createElement():** 创建新元素。
- **createTextNode():** 创建新文本节点。
- **appendChild():** 将子节点添加到父节点。
- **removeChild():** 从父节点中删除子节点。

### 注入和XSS

- 避免使用`document.write()`，因为它可能导致文档被覆盖。
- 确保从用户输入生成的内容被正确转义，以防止XSS攻击。

### 属性

- **getAttribute():** 获取元素的属性值。
- **hasAttribute():** 检查元素是否具有特定属性。
- **setAttribute():** 设置元素的属性值。

这些DOM操作允许开发人员通过JavaScript与HTML文档进行交互，动态地更新和修改页面的内容和结构。



## 事件

### 机制

在JavaScript中，事件机制是一种重要的编程范式，它使得网页可以对用户的操作或其他发生的事件做出响应。事件机制主要分为三个关键步骤：

1. **交互（Interaction）：** 用户与网页进行交互，例如点击、滚动、键盘输入等。
2. **触发（Trigger）：** 用户的交互导致特定的事件被触发，这可以是浏览器事件（如点击、加载），也可以是用户自定义的事件。
3. **相应（Response）：** 在事件触发后，相应的JavaScript代码会执行，执行的内容可以包括修改页面内容、发送请求等。

### 事件

在JavaScript中，事件分为不同的类型，主要有以下几类：

1. **W3C 事件：** 这是由World Wide Web Consortium定义的标准事件模型，包括常见的事件类型如点击（click）、变化（change）等。

   ```
   javascript// 示例：监听按钮点击事件
   document.getElementById('myButton').addEventListener('click', function() {
       console.log('按钮被点击了');
   });
   ```

2. **HTML 事件：** 这是一些与HTML元素相关的特定事件，如鼠标悬停（mouseover）、失去焦点（blur）等。

   ```
   javascript// 示例：监听输入框失去焦点事件
   document.getElementById('myInput').addEventListener('blur', function() {
       console.log('输入框失去焦点');
   });
   ```

3. **BOM 事件：** 浏览器对象模型（BOM）定义的事件，例如窗口加载（load）事件、窗口关闭（beforeunload）事件等。

   ```
   javascript// 示例：监听窗口加载事件
   window.addEventListener('load', function() {
       console.log('页面加载完成');
   });
   ```

#### UI事件

##### Load 事件

**介绍：** `load` 事件在页面或资源加载完成后触发，可以用于执行一些需要在页面完全加载后执行的操作。

```
javascript// 示例：监听页面加载完成事件
window.addEventListener('load', function() {
    console.log('页面加载完成');
});
```

##### Unload 事件

**介绍：** `unload` 事件在用户离开页面时触发，常用于执行清理操作，例如释放资源或保存用户数据。

```
javascript// 示例：监听页面卸载事件
window.addEventListener('unload', function() {
    console.log('页面即将卸载');
});
```

###### Error 事件

**介绍：** `error` 事件用于捕捉页面或资源加载过程中的错误，帮助调试和记录错误信息。

```
javascript// 示例：捕捉图片加载错误事件
document.getElementById('myImage').addEventListener('error', function() {
    console.log('图片加载失败');
});
```

###### Resize 事件

**介绍：** `resize` 事件在窗口或元素大小改变时触发，可用于响应页面布局变化。

```
javascript// 示例：监听窗口大小改变事件
window.addEventListener('resize', function() {
    console.log('窗口大小已改变');
});
```

###### Scroll 事件

**介绍：** `scroll` 事件在页面滚动时触发，可用于实现滚动时的交互效果。

```
javascript// 示例：监听页面滚动事件
window.addEventListener('scroll', function() {
    console.log('页面正在滚动');
});
```

#### 键盘事件

##### Keydown 事件

**介绍：** `keydown` 事件在用户按下键盘上的任意键时触发。

```
javascript// 示例：监听键盘按下事件
document.addEventListener('keydown', function(event) {
    console.log('键盘按下：', event.key);
});
```

##### Keyup 事件

**介绍：** `keyup` 事件在用户释放键盘上的键时触发。

```
javascript// 示例：监听键盘释放事件
document.addEventListener('keyup', function(event) {
    console.log('键盘释放：', event.key);
});
```

##### Keypress 事件

**介绍：** `keypress` 事件在用户按下并释放键盘上的键时触发。

```
javascript// 示例：监听键盘按下并释放事件
document.addEventListener('keypress', function(event) {
    console.log('键盘按下并释放：', event.key);
});
```

#### 鼠标事件

##### Click 事件

**介绍：** `click` 事件在鼠标点击元素时触发，通常用于处理用户的点击行为。

```
javascript// 示例：监听元素被点击事件
document.getElementById('myButton').addEventListener('click', function() {
    console.log('按钮被点击了');
});
```

##### Double Click 事件

**介绍：** `dblclick` 事件在鼠标双击元素时触发，用于处理双击行为。

```
javascript// 示例：监听元素被双击事件
document.getElementById('myElement').addEventListener('dblclick', function() {
    console.log('元素被双击了');
});
```

##### Mouseup 事件

**介绍：** `mouseup` 事件在鼠标按键释放时触发，适用于处理鼠标按键释放的情况。

```
javascript// 示例：监听鼠标按键释放事件
document.addEventListener('mouseup', function() {
    console.log('鼠标按键释放了');
});
```

##### Mousedown 事件

**介绍：** `mousedown` 事件在鼠标按键按下时触发，通常用于处理鼠标按键按下的情况。

```
javascript// 示例：监听鼠标按键按下事件
document.addEventListener('mousedown', function() {
    console.log('鼠标按键按下了');
});
```

##### Mouseover 事件

**介绍：** `mouseover` 事件在鼠标移入元素时触发，可用于实现鼠标移入时的效果。

```
javascript// 示例：监听鼠标移入事件
document.getElementById('myElement').addEventListener('mouseover', function() {
    console.log('鼠标移入了元素');
});
```

##### Mouseout 事件

**介绍：** `mouseout` 事件在鼠标移出元素时触发，适用于实现鼠标移出时的效果。

```
javascript// 示例：监听鼠标移出事件
document.getElementById('myElement').addEventListener('mouseout', function() {
    console.log('鼠标移出了元素');
});
```

##### Mousemove 事件

**介绍：** `mousemove` 事件在鼠标在元素内移动时触发，可用于实现鼠标跟随效果等。

```
javascript// 示例：监听鼠标移动事件
document.addEventListener('mousemove', function(event) {
    console.log('鼠标移动了，坐标：', event.clientX, event.clientY);
});
```

#### 焦点事件

##### Focus 事件

**介绍：** `focus` 事件在元素获得焦点时触发，可用于处理用户聚焦输入框或其他元素的情况。

```
javascript// 示例：监听输入框获得焦点事件
document.getElementById('myInput').addEventListener('focus', function() {
    console.log('输入框获得焦点');
});
```

##### Blur 事件

**介绍：** `blur` 事件在元素失去焦点时触发，通常用于处理用户离开输入框或其他元素的情况。

```
javascript// 示例：监听输入框失去焦点事件
document.getElementById('myInput').addEventListener('blur', function() {
    console.log('输入框失去焦点');
});
```

#### 表单事件

##### Input 事件

**介绍：** `input` 事件在用户输入内容时触发，可用于实时响应用户输入。

```
javascript// 示例：监听输入框内容变化事件
document.getElementById('myInput').addEventListener('input', function() {
    console.log('输入框内容变化：', this.value);
});
```

##### Change 事件

**介绍：** `change` 事件在表单元素的值发生变化，并失去焦点时触发，适用于处理输入框、下拉列表等的变化。

```
javascript// 示例：监听下拉列表变化事件
document.getElementById('mySelect').addEventListener('change', function() {
    console.log('下拉列表值变化：', this.value);
});
```

##### Submit 事件

**介绍：** `submit` 事件在表单提交时触发，可用于执行一些前端验证或在提交前进行操作。

```
javascript// 示例：监听表单提交事件
document.getElementById('myForm').addEventListener('submit', function(event) {
    event.preventDefault(); // 阻止默认提交行为
    console.log('表单提交了');
    // 进行其他操作或验证
});
```

##### Reset 事件

**介绍：** `reset` 事件在表单重置时触发，适用于在重置前执行一些操作。

```
javascript// 示例：监听表单重置事件
document.getElementById('myForm').addEventListener('reset', function() {
    console.log('表单被重置了');
});
```

##### Cut、Copy、Paste 事件

**介绍：** `cut`、`copy`、`paste` 事件分别在用户剪切、复制、粘贴时触发，可用于对剪贴板操作进行监听。

```
javascript// 示例：监听剪切事件
document.getElementById('myInput').addEventListener('cut', function() {
    console.log('文本被剪切了');
});

// 示例：监听复制事件
document.getElementById('myInput').addEventListener('copy', function() {
    console.log('文本被复制了');
});

// 示例：监听粘贴事件
document.getElementById('myInput').addEventListener('paste', function() {
    console.log('文本被粘贴了');
});
```

##### Select 事件

**介绍：** `select` 事件在用户选择文本时触发，可用于监听用户选择文本的操作。

```
javascript// 示例：监听文本选择事件
document.getElementById('myInput').addEventListener('select', function() {
    console.log('文本被选择了');
});
```

#### 文档事件

##### DOMSubtreeModified 事件

**介绍：** `DOMSubtreeModified` 事件在文档的某个子树结构发生变化时触发，可以用于监听DOM结构的变化。

```
javascript// 示例：监听DOM子树结构变化事件
document.addEventListener('DOMSubtreeModified', function() {
    console.log('DOM子树结构发生变化');
});
```

##### DOMNodeInserted 事件

**介绍：** `DOMNodeInserted` 事件在一个节点被插入到文档中时触发。

```
javascript// 示例：监听节点插入事件
document.addEventListener('DOMNodeInserted', function(event) {
    console.log('节点被插入到文档中：', event.target);
});
```

##### DOMNodeRemoved 事件

**介绍：** `DOMNodeRemoved` 事件在一个节点从文档中移除时触发。

```
javascript// 示例：监听节点移除事件
document.addEventListener('DOMNodeRemoved', function(event) {
    console.log('节点被从文档中移除：', event.target);
});
```

##### DOMNodeInsertedIntoDocument 事件

**介绍：** `DOMNodeInsertedIntoDocument` 事件在一个节点被插入到文档中时触发，与 `DOMNodeInserted` 类似。

```
javascript// 示例：监听节点插入到文档事件
document.addEventListener('DOMNodeInsertedIntoDocument', function(event) {
    console.log('节点插入到文档中：', event.target);
});
```

##### DOMNodeRemovedFromDocument 事件

**介绍：** `DOMNodeRemovedFromDocument` 事件在一个节点从文档中移除时触发，与 `DOMNodeRemoved` 类似。

```
javascript// 示例：监听节点从文档中移除事件
document.addEventListener('DOMNodeRemovedFromDocument', function(event) {
    console.log('节点从文档中移除：', event.target);
});
```

####  HTML事件

##### DOMContentLoaded 事件

**介绍：** `DOMContentLoaded` 事件在文档解析完成且所有DOM节点都已经构建完成时触发，而无需等待样式表、图像和子框架的完成加载。

```
javascript// 示例：监听DOM内容加载完成事件
document.addEventListener('DOMContentLoaded', function() {
    console.log('DOM内容加载完成');
});
```

##### Hashchange 事件

**介绍：** `hashchange` 事件在文档的片段标识符（URL 中的#后的部分）发生变化时触发。

```
javascript// 示例：监听URL的片段标识符变化事件
window.addEventListener('hashchange', function() {
    console.log('URL的片段标识符发生变化');
});
```

##### beforeunload 事件

**介绍：** `beforeunload` 事件在窗口即将关闭或刷新时触发，常用于在用户离开页面之前进行确认操作。

```
javascript// 示例：监听窗口即将关闭或刷新事件
window.addEventListener('beforeunload', function(event) {
    // 在此添加确认操作，例如弹出确认框
    event.returnValue = '确定离开页面吗？';
});
```

### 触发

在JavaScript中，有多种方式可以触发事件，以下是一些常见的方法：

#### HTML事件处理程序（不推荐）

这是一种将事件直接绑定到HTML元素的方法，不推荐使用，因为它将HTML和JavaScript代码混合在一起，不利于维护和阅读。

```
html
<input type="text" id="username" onblur="checkUsername()" />
```

#### 传统的DOM事件处理

使用传统的DOM事件处理方式，直接将函数赋值给事件处理属性。

```
jsfunction checkUsername() {
    // 进行用户名长度检查的代码
}

var el = document.getElementById('username');
el.onblur = checkUsername;
```

#### 第2级DOM监听器

使用第二级DOM事件监听器，通过 `addEventListener` 方法来绑定事件。

```
jsfunction checkUsername() {
    // 进行用户名长度检查的代码
}

var el = document.getElementById('username');
el.addEventListener('blur', checkUsername, false);
```

在这些示例中，`checkUsername` 函数表示事件触发后执行的逻辑代码。你可以根据需要替换这个函数来执行不同的操作。触发逻辑代码可以包含任何你想要在事件发生时执行的操作，例如表单验证、动画效果等。

##### 	传参问题

匿名函数封装

```js
el.addEventListener ('blur', function() {
checkUsername (5);
}, false);
```

###  事件流

事件流描述的是从页面中接收事件的顺序。当页面中嵌套了多个元素，并且这些元素之间发生事件时，事件的传播顺序可以通过事件流来理解。

#### 事件冒泡

在事件冒泡中，事件首先从最内层的元素开始触发，然后逐级向外传播至最外层的元素。如果你使用 `addEventListener` 来注册事件，可以将第三个参数设置为 `false`，表示使用事件冒泡。

```
js// 事件冒泡示例
var outer = document.getElementById('outer');
var inner = document.getElementById('inner');

outer.addEventListener('click', function() {
    console.log('外层元素被点击');
}, false);

inner.addEventListener('click', function() {
    console.log('内层元素被点击');
}, false);
```

在上面的例子中，如果你点击内层元素（id为`inner`），事件将首先在内层元素上触发，然后冒泡到外层元素（id为`outer`）。

#### 事件捕获

在事件捕获中，事件从最外层的元素开始触发，然后逐级向内传播至最内层的元素。如果你使用 `addEventListener` 来注册事件，可以将第三个参数设置为 `true`，表示使用事件捕获。

```
js// 事件捕获示例
var outer = document.getElementById('outer');
var inner = document.getElementById('inner');

outer.addEventListener('click', function() {
    console.log('外层元素被点击');
}, true);

inner.addEventListener('click', function() {
    console.log('内层元素被点击');
}, true);
```

在上面的例子中，如果你点击内层元素（id为`inner`），事件将首先在外层元素（id为`outer`）上捕获，然后传播到内层元素。

### 事件对象

事件对象（Event Object）是在事件触发时由浏览器传递给事件处理程序的对象。这个对象包含了与事件相关的信息，可以通过它来获取事件的各种属性和方法。

在事件处理程序中，通常将事件对象作为参数传递给事件处理函数。不同的事件类型可能有不同的事件对象，但它们都共享一些通用的属性和方法。

以下是一些常见的事件对象属性和方法：

##### 通用属性和方法

1. **`type`：** 表示事件的类型，如 `'click'`、`'mouseover'` 等。

   ```
   javascriptfunction handleClick(event) {
       console.log('事件类型：', event.type);
   }
   ```

2. **`target`：** 表示触发事件的元素。

   ```
   javascriptfunction handleClick(event) {
       console.log('触发事件的元素：', event.target);
   }
   ```

3. **`currentTarget`：** 表示当前事件处理程序正在处理事件的元素。

   ```
   javascriptfunction handleClick(event) {
       console.log('当前处理事件的元素：', event.currentTarget);
   }
   ```

##### 鼠标事件属性

对于鼠标事件，事件对象还包含一些特定的属性：

1. **`clientX` 和 `clientY`：** 表示鼠标事件发生时鼠标指针相对于浏览器窗口的水平和垂直坐标。

   ```
   javascriptfunction handleMouseMove(event) {
       console.log('鼠标坐标：', event.clientX, event.clientY);
   }
   ```

2. **`button`：** 表示按下或释放的鼠标按键的编码。

   ```
   javascriptfunction handleMouseClick(event) {
       console.log('鼠标按键编码：', event.button);
   }
   ```

##### 键盘事件属性

对于键盘事件，事件对象还包含一些特定的属性：

1. **`keyCode` 和 `key`：** 表示按下或释放的键的键码和键名。

   ```
   javascriptfunction handleKeyPress(event) {
       console.log('按键编码：', event.keyCode);
       console.log('按键名称：', event.key);
   }
   ```



## jQuery

jQuery 是一个流行的 JavaScript 库，旨在简化处理 HTML 文档、事件处理、动画和 AJAX 的任务。通过使用 jQuery，你可以更轻松地选择和操作 HTML 元素，以及执行各种常见的前端开发任务。

以下是 jQuery 常用的一些功能和用法：

#### 选择元素

通过使用类似 CSS 选择器的语法，可以轻松地选择和操作 HTML 元素。

```
javascript// 选择所有段落元素
$('p').text('Hello, jQuery!');

// 选择具有特定类的元素
$('.myClass').css('color', 'red');

// 选择具有特定 ID 的元素
$('#myId').hide();
```

#### 高效开发

jQuery 提供了许多简化开发的方法，比如处理事件、执行动画等。

#### 事件处理

```
javascript// 监听点击事件
$('#myButton').click(function() {
    alert('按钮被点击了！');
});

// 监听表单提交事件
$('form').submit(function() {
    alert('表单已提交！');
});
```

动画

```
javascript// 淡入淡出效果
$('#myElement').fadeOut(1000).fadeIn(1000);

// 移动元素
$('#myElement').animate({ left: '200px', top: '200px' }, 1000);
```

### 引入 jQuery

在你的 HTML 文件中引入 jQuery 库，可以通过下载 jQuery 文件并在 HTML 中引用，或者使用 CDN（内容分发网络）：

```
html<!-- 通过 CDN 引入 jQuery -->
<script src="https://code.jquery.com/jquery-3.6.4.min.js"></script>
```

**除了类似与css选择器的方式，jQuery还提供筛选器**

### 筛选器

- `:not(selector)`: 选择不匹配给定选择器的元素。

```
javascript// 选择不含有类名为 'exclude' 的所有段落元素
$('p:not(.exclude)').css('color', 'green');
```

- `:first`: 选择匹配的元素集合中的第一个元素。

```
javascript// 选择第一个段落元素
$('p:first').css('font-weight', 'bold');
```

- `:last`: 选择匹配的元素集合中的最后一个元素。

```
javascript// 选择最后一个段落元素
$('p:last').css('font-style', 'italic');
```

- `:even`: 选择匹配的元素集合中的偶数位置的元素（从 0 开始计数）。

```
javascript// 选择偶数位置的段落元素
$('p:even').css('background-color', 'lightblue');
```

- `:odd`: 选择匹配的元素集合中的奇数位置的元素（从 0 开始计数）。

```
javascript// 选择奇数位置的段落元素
$('p:odd').css('background-color', 'lightyellow');
```

- `:eq(index)`: 选择匹配的元素集合中指定索引位置的元素（从 0 开始计数）。

```
javascript// 选择第二个段落元素
$('p:eq(1)').css('text-decoration', 'underline');
```

- `:gt(index)`: 选择匹配的元素集合中索引大于指定索引的所有元素。

```
javascript// 选择索引大于 2 的段落元素
$('p:gt(2)').css('color', 'purple');
```

- `:lt(index)`: 选择匹配的元素集合中索引小于指定索引的所有元素。

```
javascript// 选择索引小于 3 的段落元素
$('p:lt(3)').css('color', 'orange');
```

- `:header`: 选择所有标题元素 (`h1`, `h2`, `h3`, ..., `h6`)。

```
javascript// 选择所有标题元素
$(':header').css('border-bottom', '2px solid black');
```

- `:animated`: 选择当前正在执行动画的所有元素。

```
javascript// 选择当前正在执行动画的元素并停止动画
$(':animated').stop();
```

- `:focus`: 选择当前获得焦点的元素。

```
javascript// 选择当前获得焦点的输入框
$(':focus').css('border', '2px solid red');
```

- `:contains('text')`: 选择包含指定文本的元素。

```
javascript// 选择包含文本 "Hello" 的段落元素
$('p:contains("Hello")').css('background-color', 'yellow');
```

- `:empty`: 选择没有子元素或者文本的空元素。

```
javascript// 选择没有内容的 div 元素
$('div:empty').text('This div was empty!').css('border', '1px solid black');
```

- `:parent`: 选择至少含有一个子元素或文本的父元素。

```
javascript// 选择含有子元素的 div 元素
$('div:parent').css('border', '2px solid blue');
```

- `:has(selector)`: 选择至少含有一个匹配给定选择器的子元素的元素。

```
javascript// 选择含有类名为 'highlight' 的子元素的段落元素
$('p:has(.highlight)').css('font-weight', 'bold');
```

- `:hidden`: 选择所有隐藏的元素。

```
javascript// 选择所有隐藏的输入框
$('input:hidden').show();
```

- `:visible`: 选择所有可见的元素。

```
javascript// 选择所有可见的按钮元素
$('button:visible').css('background-color', 'green');
```

- `:nth-child(expr)`: 选择其父元素的第 N 个子元素，其中 N 由表达式 `expr` 决定。

```
javascript// 选择每个父元素的第三个子元素
$('p:nth-child(3)').css('color', 'red');
```

- `:first-child`: 选择其父元素的第一个子元素。

```
javascript// 选择每个父元素的第一个子元素
$('p:first-child').css('text-decoration', 'underline');
```

- `:last-child`: 选择其父元素的最后一个子元素。

```
javascript// 选择每个父元素的最后一个子元素
$('p:last-child').css('font-style', 'italic');
```

- `:only-child`: 选择其父元素中唯一的子元素。

```
javascript// 选择每个父元素中唯一的子元素
$('p:only-child').css('font-size', '24px');
```

- `[attribute]`: 选择具有指定属性的元素。

```
javascript// 选择具有 'data-toggle' 属性的按钮元素
$('button[data-toggle]').css('background-color', 'yellow');
```

- `[attribute='value']`: 选择具有指定属性和属性值的元素。

```
javascript// 选择 'src' 属性为 'image.jpg' 的图像元素
$('img[src="image.jpg"]').css('border', '2px solid red');
```

- `[attribute != 'value']`: 选择具有指定属性但属性值不等于给定值的元素。

```
javascript// 选择 'type' 属性不为 'checkbox' 的输入框元素
$('input[type!="checkbox"]').css('color', 'blue');
```

- `[attribute^='value']`: 选择具有指定属性且属性值以给定值开头的元素。

```
javascript// 选择 'href' 属性以 'https://' 开头的链接元素
$('a[href^="https://"]').css('color', 'green');
```

- `[attribute$='value']`: 选择具有指定属性且属性值以给定值结尾的元素。

```
javascript// 选择 'src' 属性以 '.png' 结尾的图像元素
$('img[src$=".png"]').css('border', '2px solid blue');
```

- `[attribute*='value']`: 选择具有指定属性且属性值包含给定值的元素。

```
javascript// 选择 'alt' 属性包含 'cat' 的图像元素
$('img[alt*="cat"]').css('border', '2px solid pink');
```

- `[attribute|='value']`: 选择具有指定属性且属性值以给定值开头，后跟一个连字符 `-` 或是与给定值完全相同的元素。

```
javascript// 选择 'lang' 属性值为 'en' 或以 'en-' 开头的元素
$('[lang|="en"]').css('font-family', 'Arial, sans-serif');
```

- `[attribute ~= 'value']`: 选择具有指定属性且属性值包含多个空格分隔的词，其中一个词与给定值相同的元素。

```
javascript// 选择 'class' 属性包含 'active' 的元素
$('.active').css('background-color', 'yellow');
```

- `[attribute] [attribute2]`: 选择同时具有两个属性的元素，可以用空格分隔多个属性选择器。

```
javascript// 选择同时具有 'data-toggle' 和 'data-target' 属性的按钮元素
$('button[data-toggle][data-target]').css('color', 'purple');
```

- `:input`: 选择所有的输入元素，包括文本框、复选框、单选按钮、提交按钮等。

```
javascript// 选择所有输入元素并设置它们的边框颜色
$(':input').css('border', '1px solid gray');
```

- `:text`: 选择所有文本框元素。

```
javascript// 选择所有文本框并设置它们的背景颜色
$(':text').css('background-color', 'lightyellow');
```

- `:password`: 选择所有密码框元素。

```
javascript// 选择所有密码框并设置它们的边框颜色
$(':password').css('border', '2px solid darkred');
```

- `:radio`: 选择所有单选按钮元素。

```
javascript// 选择所有单选按钮并设置它们的字体颜色
$(':radio').css('color', 'green');
```

- `:checkbox`: 选择所有复选框元素。

```
javascript// 选择所有复选框并设置它们的边框颜色
$(':checkbox').css('border', '2px solid purple');
```

- `:submit`: 选择所有提交按钮元素。

```
javascript// 选择所有提交按钮并设置它们的背景颜色
$(':submit').css('background-color', 'lightblue');
```

- `:image`: 选择所有图像按钮元素。

```
javascript// 选择所有图像按钮并设置它们的边框颜色
$(':image').css('border', '1px solid orange');
```

- `:reset`: 选择所有重置按钮元素。

```
javascript// 选择所有重置按钮并设置它们的字体样式
$(':reset').css('font-style', 'italic');
```

- `:button`: 选择所有按钮元素，包括提交按钮、重置按钮以及普通按钮。

```
javascript// 选择所有按钮并设置它们的颜色
$(':button').css('color', 'darkblue');
```

- `:file`: 选择所有文件上传元素。

```
javascript// 选择所有文件上传元素并设置它们的背景颜色
$(':file').css('background-color', 'lightgreen');
```

- `:selected`: 选择所有被选中的元素，通常用于 `select` 元素。

```
javascript// 选择所有被选中的选项并设置它们的颜色
$('option:selected').css('color', 'red');
```

- `:enabled`: 选择所有可用的元素。

```
javascript// 选择所有可用的输入元素并设置它们的边框颜色
$(':enabled').css('border', '1px solid green');
```

- `:disabled`: 选择所有禁用的元素。

```
javascript// 选择所有禁用的输入元素并设置它们的背景颜色
$(':disabled').css('background-color', 'lightgray');
```

- `:checked`: 选择所有被选中的复选框或单选按钮元素。

```
javascript// 选择所有被选中的复选框并设置它们的边框颜色
$(':checked').css('border', '2px solid pink');
```

### 方法

#### 元素选择

##### 获取/更改

1. **.html():**

   - **描述：** 用于获取或设置元素的 HTML 内容。

   - 例子：

     ```js
     html
     <div id="myDiv">原始内容</div>
     ```

     ```js
     javascript// 获取HTML内容
     var content = $("#myDiv").html();
     console.log(content); // 输出: 原始内容
     
     // 设置HTML内容
     $("#myDiv").html("新的内容");
     ```

2. **.text():**

   - **描述：** 用于获取或设置元素的纯文本内容。

   - 例子：

     ```
     html
     <p id="myPara">原始文本</p>
     ```

     ```
     javascript// 获取文本内容
     var textContent = $("#myPara").text();
     console.log(textContent); // 输出: 原始文本
     
     // 设置文本内容
     $("#myPara").text("新的文本");
     ```

3. **.replaceWith():**

   - **描述：** 用一个或多个元素替换匹配的元素。

   - 例子：

     ```
     html<div class="original">原始内容</div>
     <div class="replacement">替换的内容</div>
     ```

     ```
     javascript// 替换元素
     $(".original").replaceWith("<p>新的内容</p>");
     ```

4. **.remove():**

   - **描述：** 从DOM中移除匹配的元素。

   - 例子：

     ```
     html
     <div id="toBeRemoved">要移除的内容</div>
     ```

     ```
     javascript// 移除元素
     $("#toBeRemoved").remove();
     ```

##### 元素

1. **.before():**

   - **描述：** 在每个匹配的元素之前插入指定的内容。

   - 例子：

     ```
     html
     <p class="target">目标元素</p>
     ```

     ```
     javascript// 在目标元素之前插入新内容
     $(".target").before("<div>新内容</div>");
     ```

2. **.after():**

   - **描述：** 在每个匹配的元素之后插入指定的内容。

   - 例子：

     ```
     html
     <p class="target">目标元素</p>
     ```

     ```
     javascript// 在目标元素之后插入新内容
     $(".target").after("<div>新内容</div>");
     ```

3. **.prepend():**

   - **描述：** 在每个匹配的元素内部的开始位置插入指定的内容。

   - 例子：

     ```
     html
     <div class="target">目标元素</div>
     ```

     ```
     javascript// 在目标元素内部的开始位置插入新内容
     $(".target").prepend("<p>新内容</p>");
     ```

4. **.append():**

   - **描述：** 在每个匹配的元素内部的末尾位置插入指定的内容。

   - 例子：

     ```
     html
     <div class="target">目标元素</div>
     ```

     ```
     javascript// 在目标元素内部的末尾位置插入新内容
     $(".target").append("<p>新内容</p>");
     ```

5. **.remove():**

   - **描述：** 从DOM中移除匹配的元素。

   - 例子：

     ```
     html
     <div class="toBeRemoved">要移除的内容</div>
     ```

     ```
     javascript// 移除元素
     $(".toBeRemoved").remove();
     ```

6. **.clone():**

   - **描述：** 复制匹配的元素，包括所有的子元素和事件处理程序。

   - 例子：

     ```
     html
     <div class="original">原始内容</div>
     ```

     ```
     javascript// 复制元素
     var clone = $(".original").clone();
     ```

7. **.unwrap():**

   - **描述：** 从DOM中移除匹配元素的父元素，保留匹配元素本身。

   - 例子：

     ```
     html
     <div class="wrapper"><p>被包裹的内容</p></div>
     ```

     ```
     javascript// 移除包裹元素
     $("p").unwrap();
     ```

8. **.detach():**

   - **描述：** 从DOM中移除匹配的元素，但保留元素的数据和事件处理程序。

   - 例子：

     ```
     html
     <div class="toBeDetached">要移除但保留数据的内容</div>
     ```

     ```
     javascript// 移除元素但保留数据
     $(".toBeDetached").detach();
     ```

9. **.empty():**

   - **描述：** 从匹配的元素中移除所有子元素和内容。

   - 例子：

     ```
     html
     <div class="toBeEmptied"><p>要清空的内容</p></div>
     ```

     ```
     javascript// 清空元素内容
     $(".toBeEmptied").empty();
     ```

10. **.add():**

    - **描述：** 将元素添加到当前集合中。

    - 例子：

      ```
      html
      <div class="existing">已有的元素</div>
      ```

      ```
      javascript// 将新元素添加到已有元素集合中
      var newElement = $("<p>新元素</p>");
      $(".existing").add(newElement);
      ```

##### 属性

1. **.attr():**

   - **描述：** 用于获取或设置匹配元素的属性。

   - 例子：

     ```
     html
     <img id="myImage" src="oldImage.jpg" alt="Old Image">
     ```

     ```
     javascript// 获取属性值
     var srcValue = $("#myImage").attr("src");
     console.log(srcValue); // 输出: oldImage.jpg
     
     // 设置属性值
     $("#myImage").attr("src", "newImage.jpg");
     ```

2. **.removeAttr():**

   - **描述：** 从匹配的元素中移除属性。

   - 例子：

     ```
     html
     <input type="text" id="myInput" value="Some text">
     ```

     ```
     javascript// 移除属性
     $("#myInput").removeAttr("value");
     ```

3. **.addClass():**

   - **描述：** 向匹配的元素添加一个或多个类。

   - 例子：

     ```
     html
     <div id="myDiv" class="oldClass">内容</div>
     ```

     ```
     javascript// 添加类
     $("#myDiv").addClass("newClass");
     ```

4. **.removeClass():**

   - **描述：** 从匹配的元素中移除一个或多个类。

   - 例子：

     ```
     html
     <div id="myDiv" class="oldClass newClass">内容</div>
     ```

     ```
     javascript// 移除类
     $("#myDiv").removeClass("oldClass");
     ```

5. **.css():**

   - **描述：** 获取或设置匹配元素的样式属性。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取样式属性值
     var backgroundColor = $("#myDiv").css("background-color");
     console.log(backgroundColor); // 输出: 样式属性值
     
     // 设置样式属性值
     $("#myDiv").css("color", "blue");
     ```

##### 表单

1. **.val():**

   - **描述：** 用于获取或设置表单元素的值。

   - 例子：

     ```
     html
     <input type="text" id="myInput" value="默认值">
     ```

     ```
     javascript// 获取输入框的值
     var inputValue = $("#myInput").val();
     console.log(inputValue); // 输出: 默认值
     
     // 设置输入框的值
     $("#myInput").val("新的值");
     ```

2. **.isNumeric():**

   - **描述：** 判断给定的值是否为数字。

   - 例子：

     ```
     javascript// 检查是否为数字
     var numericValue = 42;
     var isNumeric = $.isNumeric(numericValue);
     console.log(isNumeric); // 输出: true
     
     // 非数字情况
     var stringValue = "Not a number";
     var isNotNumeric = $.isNumeric(stringValue);
     console.log(isNotNumeric); // 输出: false
     ```

##### 一般方法

1. **.find():**

   - **描述：** 在匹配的元素中查找后代元素。

   - 例子：

     ```
     html<div class="container">
       <div class="target">目标元素</div>
     </div>
     ```

     ```
     javascript// 查找后代元素
     var descendantElement = $(".container").find(".target");
     ```

2. **.closest():**

   - **描述：** 在匹配的元素及其祖先元素中，找到最近的一个匹配选择器的元素。

   - 例子：

     ```
     html<div class="container">
       <div class="inner">
         <div class="target">目标元素</div>
       </div>
     </div>
     ```

     ```
     javascript// 找到最近的匹配元素
     var closestElement = $(".target").closest(".container");
     ```

3. **.parent():**

   - **描述：** 获取匹配元素的父元素。

   - 例子：

     ```
     html<div class="parent">
       <div class="target">目标元素</div>
     </div>
     ```

     ```
     javascript// 获取父元素
     var parentElement = $(".target").parent();
     ```

4. **.parents():**

   - **描述：** 获取匹配元素的所有祖先元素。

   - 例子：

     ```
     html<div class="grandparent">
       <div class="parent">
         <div class="target">目标元素</div>
       </div>
     </div>
     ```

     ```
     javascript// 获取所有祖先元素
     var ancestorElements = $(".target").parents();
     ```

5. **.children():**

   - **描述：** 获取匹配元素的所有子元素。

   - 例子：

     ```
     html<div class="parent">
       <div class="child">子元素</div>
     </div>
     ```

     ```
     javascript// 获取所有子元素
     var childElements = $(".parent").children();
     ```

6. **.siblings():**

   - **描述：** 获取匹配元素的所有同级元素。

   - 例子：

     ```
     html<div class="sibling">同级元素 1</div>
     <div class="sibling">同级元素 2</div>
     <div class="target">目标元素</div>
     ```

     ```
     javascript// 获取所有同级元素
     var siblingElements = $(".target").siblings();
     ```

7. **.next():**

   - **描述：** 获取匹配元素的下一个同级元素。

   - 例子：

     ```
     html<div class="target">目标元素</div>
     <div class="next-sibling">下一个同级元素</div>
     ```

     ```
     javascript// 获取下一个同级元素
     var nextElement = $(".target").next();
     ```

8. **.nextAll():**

   - **描述：** 获取匹配元素之后的所有同级元素。

   - 例子：

     ```
     html<div class="target">目标元素</div>
     <div class="next-sibling">下一个同级元素 1</div>
     <div class="next-sibling">下一个同级元素 2</div>
     ```

     ```
     javascript// 获取之后的所有同级元素
     var nextAllElements = $(".target").nextAll();
     ```

9. **.prev():**

   - **描述：** 获取匹配元素的上一个同级元素。

   - 例子：

     ```
     html<div class="prev-sibling">上一个同级元素</div>
     <div class="target">目标元素</div>
     ```

     ```
     javascript// 获取上一个同级元素
     var prevElement = $(".target").prev();
     ```

10. **.prevAll():**

    - **描述：** 获取匹配元素之前的所有同级元素。

    - 例子：

      ```
      html<div class="prev-sibling">上一个同级元素 2</div>
      <div class="prev-sibling">上一个同级元素 1</div>
      <div class="target">目标元素</div>
      ```

      ```
      javascript// 获取之前的所有同级元素
      var prevAllElements = $(".target").prevAll();
      ```

##### 筛选器/测试

1. **.filter():**

   - **描述：** 用于筛选匹配元素集合中满足指定条件的元素。

   - 例子：

     ```
     html<ul>
       <li>Item 1</li>
       <li class="selected">Item 2</li>
       <li>Item 3</li>
     </ul>
     ```

     ```
     javascript// 筛选出有特定类的元素
     var selectedItems = $("li").filter(".selected");
     ```

2. **.not():**

   - **描述：** 用于筛选匹配元素集合中不满足指定条件的元素。

   - 例子：

     ```
     html<ul>
       <li>Item 1</li>
       <li class="exclude">Item 2</li>
       <li>Item 3</li>
     </ul>
     ```

     ```
     javascript// 筛选出没有特定类的元素
     var nonExcludedItems = $("li").not(".exclude");
     ```

3. **.has():**

   - **描述：** 用于筛选匹配元素集合中包含特定后代的元素。

   - 例子：

     ```
     html<div class="container">
       <p>包含段落的元素</p>
     </div>
     ```

     ```
     javascript// 筛选出包含特定后代的元素
     var containerWithParagraph = $(".container").has("p");
     ```

4. **.is():**

   - **描述：** 用于检查匹配元素集合中的元素是否匹配指定的选择器、元素或 jQuery 对象。

   - 例子：

     ```
     html
     <div class="target">目标元素</div>
     ```

     ```
     javascript// 检查元素是否有特定类
     var hasClass = $(".target").is(".target");
     ```

5. **:contains():**

   - **描述：** 用于选择包含指定文本的元素。

   - 例子：

     ```
     html<ul>
       <li>Item 1</li>
       <li>Item 2 contains text</li>
       <li>Item 3</li>
     </ul>
     ```

     ```
     javascript// 选择包含特定文本的元素
     var containsText = $("li:contains('contains text')");
     ```

##### 元素选中顺序（索引）

1. **.eq():**

   - **描述：** 用于选择匹配元素集合中指定索引位置的元素。

   - 例子：

     ```
     html<ul>
       <li>Item 1</li>
       <li>Item 2</li>
       <li>Item 3</li>
     </ul>
     ```

     ```
     javascript// 选择第二个 li 元素（索引从 0 开始）
     var secondItem = $("li").eq(1);
     ```

2. **:lt():**

   - **描述：** 选择匹配元素集合中所有位置小于给定索引的元素。

   - 例子：

     ```
     html<ul>
       <li>Item 1</li>
       <li>Item 2</li>
       <li>Item 3</li>
     </ul>
     ```

     ```
     javascript// 选择索引小于 2 的元素
     var itemsBeforeIndex2 = $("li:lt(2)");
     ```

3. **:gt():**

   - **描述：** 选择匹配元素集合中所有位置大于给定索引的元素。

   - 例子：

     ```
     html<ul>
       <li>Item 1</li>
       <li>Item 2</li>
       <li>Item 3</li>
     </ul>
     ```

     ```
     javascript// 选择索引大于 0 的元素
     var itemsAfterIndex0 = $("li:gt(0)");
     ```

#### 内容操作

##### 尺寸

1. **.height():**

   - **描述：** 获取或设置匹配元素的高度。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取元素的高度
     var elementHeight = $("#myDiv").height();
     ```

2. **.width():**

   - **描述：** 获取或设置匹配元素的宽度。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取元素的宽度
     var elementWidth = $("#myDiv").width();
     ```

3. **.innerHeight():**

   - **描述：** 获取匹配元素的高度，包括内边距但不包括边框和外边距。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取元素的内部高度
     var innerHeight = $("#myDiv").innerHeight();
     ```

4. **.innerWidth():**

   - **描述：** 获取匹配元素的宽度，包括内边距但不包括边框和外边距。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取元素的内部宽度
     var innerWidth = $("#myDiv").innerWidth();
     ```

5. **.outerHeight():**

   - **描述：** 获取匹配元素的高度，包括内边距和边框，但不包括外边距。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取元素的外部高度
     var outerHeight = $("#myDiv").outerHeight();
     ```

6. **.outerWidth():**

   - **描述：** 获取匹配元素的宽度，包括内边距和边框，但不包括外边距。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取元素的外部宽度
     var outerWidth = $("#myDiv").outerWidth();
     ```

7. **$(document).height():**

   - **描述：** 获取文档的高度。

   - 例子：

     ```
     javascript// 获取文档的高度
     var documentHeight = $(document).height();
     ```

8. **$(document).width():**

   - **描述：** 获取文档的宽度。

   - 例子：

     ```
     javascript// 获取文档的宽度
     var documentWidth = $(document).width();
     ```

9. **$(window).height():**

   - **描述：** 获取浏览器窗口的高度。

   - 例子：

     ```
     javascript// 获取窗口的高度
     var windowHeight = $(window).height();
     ```

10. **$(window).width():**

    - **描述：** 获取浏览器窗口的宽度。

    - 例子：

      ```
      javascript// 获取窗口的宽度
      var windowWidth = $(window).width();
      ```

##### 位置

1. **.offset():**

   - **描述：** 获取匹配元素相对于文档的偏移。

   - 例子：

     ```
     html
     <div id="myDiv">内容</div>
     ```

     ```
     javascript// 获取元素的文档偏移
     var elementOffset = $("#myDiv").offset();
     ```

2. **.position():**

   - **描述：** 获取匹配元素相对于其最近的定位祖先的偏移。

   - 例子：

     ```
     html<div id="parent" style="position: relative;">
       <div id="myDiv">内容</div>
     </div>
     ```

     ```
     javascript// 获取元素相对于定位祖先的偏移
     var elementPosition = $("#myDiv").position();
     ```

3. **.scrollLeft():**

   - **描述：** 获取或设置匹配元素的水平滚动位置。

   - 例子：

     ```
     html<div id="scrollContainer" style="overflow-x: scroll; white-space: nowrap;">
       <!-- 长内容 -->
       <div id="scrollContent" style="width: 1000px;">滚动内容</div>
     </div>
     ```

     ```
     javascript// 获取水平滚动位置
     var scrollLeftValue = $("#scrollContainer").scrollLeft();
     ```

4. **.scrollTop():**

   - **描述：** 获取或设置匹配元素的垂直滚动位置。

   - 例子：

     ```
     html<div id="scrollContainer" style="overflow-y: scroll; height: 200px;">
       <!-- 长内容 -->
       <div id="scrollContent" style="height: 500px;">滚动内容</div>
     </div>
     ```

     ```
     javascript// 获取垂直滚动位置
     var scrollTopValue = $("#scrollContainer").scrollTop();
     ```

##### 特效和动画

###### 一般

1. **.show():**

   - **描述：** 用于显示匹配的元素。

   - 例子：

     ```
     javascript// 显示元素
     $("#myElement").show();
     ```

2. **.hide():**

   - **描述：** 用于隐藏匹配的元素。

   - 例子：

     ```
     javascript// 隐藏元素
     $("#myElement").hide();
     ```

3. **.toggle():**

   - **描述：** 用于在显示和隐藏之间切换匹配的元素。

   - 例子：

     ```
     javascript// 切换元素的显示和隐藏状态
     $("#myElement").toggle();
     ```

###### 淡出

1. **.fadeIn():**

   - **描述：** 用于淡入匹配的元素，逐渐使元素从不透明到透明。

   - 例子：

     ```
     javascript// 淡入元素
     $("#myElement").fadeIn();
     ```

2. **.fadeOut():**

   - **描述：** 用于淡出匹配的元素，逐渐使元素从透明到不透明。

   - 例子：

     ```
     javascript// 淡出元素
     $("#myElement").fadeOut();
     ```

3. **.fadeTo():**

   - **描述：** 用于将匹配元素的不透明度渐变到指定值。

   - 例子：

     ```
     javascript// 渐变元素的不透明度到0.5
     $("#myElement").fadeTo("slow", 0.5);
     ```

4. **.fadeToggle():**

   - **描述：** 用于在淡入和淡出之间切换匹配的元素。

   - 例子：

     ```
     javascript// 切换元素的淡入和淡出状态
     $("#myElement").fadeToggle();
     ```

###### 滑动

1. **.slideDown():**

   - **描述：** 用于滑动显示匹配的元素。

   - 例子：

     ```
     javascript// 滑动显示元素
     $("#myElement").slideDown();
     ```

2. **.slideUp():**

   - **描述：** 用于滑动隐藏匹配的元素。

   - 例子：

     ```
     javascript// 滑动隐藏元素
     $("#myElement").slideUp();
     ```

3. **.slideToggle():**

   - **描述：** 用于在滑动显示和滑动隐藏之间切换匹配的元素。

   - 例子：

     ```
     javascript// 切换元素的滑动显示和隐藏状态
     $("#myElement").slideToggle();
     ```

###### 自定义

1. **.delay():**

   - **描述：** 用于设置动画开始之前的延迟。

   - 例子：

     ```
     javascript// 在动画开始之前延迟500毫秒
     $("#myElement").delay(500).fadeIn();
     ```

2. **.stop():**

   - **描述：** 用于停止当前正在运行的动画。

   - 例子：

     ```
     javascript// 停止当前元素的所有动画
     $("#myElement").stop();
     ```

3. **.animate():**

   - **描述：** 用于创建自定义的动画效果。

   - 例子：

     ```
     javascript// 自定义动画
     $("#myElement").animate({
       opacity: 0.5,
       width: "50%"
     }, 1000);
     ```

##### 文档

1. **.ready():**

   - **描述：** 用于在文档加载完成后执行函数。

   - 例子：

     ```
     javascript
     $(document).ready(function() {
       // 在文档加载完成后执行的代码
       console.log("文档加载完成！");
     });
     ```

     或简写为：

     ```
     javascript
     $(function() {
       // 在文档加载完成后执行的代码
       console.log("文档加载完成！");
     });
     ```

2. **.load():**

   - **描述：** 用于在元素加载完成后执行函数。

   - 例子：

     ```
     javascript
     $("#myImage").load(function() {
       // 图片加载完成后执行的代码
       console.log("图片加载完成！");
     });
     ```

3. **.on():**

   - **描述：** 用于附加一个或多个事件处理程序到匹配元素。

   - 例子：

     ```
     javascript
     $("button").on("click", function() {
       // 按钮被点击时执行的代码
       console.log("按钮被点击！");
     });
     ```

##### 遍历

`.each()` 方法是 jQuery 提供的用于迭代处理集合中的元素的方法。它可以用于循环遍历数组、对象或 jQuery 对象中的元素，执行指定的函数。

以下是 `.each()` 方法的基本语法：

```
$.each(collection, function(index, value) {
  // 处理每个元素的代码
});
```

#### 链式操作

例子：

```js
$('li[id != "one"]') .hide ().delay (500) . fadeIn (1400) ;
```

## 

## 运行调试与错误处理

### 执行顺序

#### 1. 执行上下文

- **内容介绍：** 执行上下文是JavaScript代码执行的环境，包括变量、函数、this等信息。了解执行上下文的创建和执行过程对于理解代码执行流程至关重要。

- 例子：

  ```js
  console.log(x); // 输出 undefined，但不报错
  var x = 5;
  ```

#### 2. 堆栈

- **内容介绍：** JavaScript使用调用栈（执行栈）来管理执行上下文。学习调用栈的概念有助于理解代码的执行顺序和调用关系。

- 例子：

  ```js
  function foo() {
    console.log('foo');
  }
  function bar() {
    foo();
    console.log('bar');
  }
  bar();
  ```

#### 3. 准备阶段

- **内容介绍：** 在代码执行之前，JavaScript会进行准备工作，包括创建新的作用域、变量、函数和参数，以及确定this关键字的值。

- 例子：

  ```js
  console.log(a); // 输出 undefined，不会报错
  var a = 10;
  ```

#### 4. 执行阶段

- **内容介绍：** 一旦准备阶段完成，JavaScript开始执行代码，包括给变量赋值、引用函数来执行其代码以及执行语句。

- 例子：

  ```js
  function multiply(x, y) {
    return x * y;
  }
  console.log(multiply(3, 4)); // 输出 12
  ```

### 变量作用域与性能

#### 1. 作用域链

- **内容介绍：** JavaScript中的作用域链决定了变量的访问范围。深入了解作用域链有助于更好地组织和理解代码。

- 例子：

  ```js
  function outer() {
    var x = 10;
    function inner() {
      console.log(x);
    }
    inner();
  }
  outer(); // 输出 10
  ```

#### 2. 闭包

- **内容介绍：** 闭包是指函数能够访问其词法作用域外部的变量。了解闭包的概念和使用场景对于优化代码结构和性能至关重要。

- 例子：

  ```js
  function outer() {
    var x = 10;
    function inner() {
      console.log(x);
    }
    return inner;
  }
  var closureFn = outer();
  closureFn(); // 输出 10
  ```

###  错误理解和处理

#### 1. 异常机制

- **内容介绍：** JavaScript中的异常是指运行时错误，可能导致代码无法正常执行。了解异常的机制有助于及时发现和处理错误。

- 例子：

  ```js
  try {
    // 可能会引发异常的代码
  } catch (error) {
    // 异常处理代码
    console.error(error.message);
  } finally {
      // 最终执行的必须执行的代码
  }
  ```

#### 2. Error 对象

- **内容介绍：** Error 对象是 JavaScript 中用于表示错误的基础对象，它包含了多个属性用于描述错误的详细信息。

- 属性：

  - **name：** 错误名称
  - **message：** 错误消息
  - **stack：** 错误堆栈信息

- 例子：

  ```js
  try {
    // 可能会引发异常的代码
  } catch (error) {
    console.error(error.name); // 输出错误名称
    console.error(error.message); // 输出错误消息
    console.error(error.stack); // 输出错误堆栈信息
  }
  ```

#### 3. 内置错误类型

- **内容介绍：** JavaScript内置了多种错误类型，每种类型代表不同的错误情况，包括但不限于语法错误、引用错误、类型错误、范围错误、URI错误和评估错误。

- 内置错误类型：

  - **Error：** 通用错误对象
  - **SyntaxError：** 语法错误
  - **ReferenceError：** 引用错误
  - **TypeError：** 类型错误
  - **RangeError：** 范围错误
  - **URIError：** URI错误
  - **EvalError：** 评估错误

- 例子：

  ```js
  try {
    // 可能会引发不同类型的错误的代码
  } catch (error) {
    if (error instanceof SyntaxError) {
      console.error('语法错误');
    } else if (error instanceof ReferenceError) {
      console.error('引用错误');
    } else if (error instanceof TypeError) {
      console.error('类型错误');
    }
    // 其他错误类型的处理
  }
  ```

以上是关于错误理解和处理的基本大纲，通过了解异常机制、Error 对象和内置错误类型，你可以更有效地调试和处理JavaScript代码中的错误。

### 调试

#### 1. 浏览器开发者工具和 Console

- **内容介绍：** 浏览器开发者工具是调试JavaScript代码的重要工具之一，而Console是其中一个强大的组件，用于输出日志和进行交互性的调试。

- **使用开发者工具：** 打开浏览器开发者工具，切换到“Console”选项卡。

- 例子：

  ```js
  // 使用不同的 console 方法输出日志
  console.log('普通日志');
  console.info('信息日志');
  console.warn('警告日志');
  console.error('错误日志');
  
  // 使用 group 和 groupEnd 创建日志分组
  console.group('日志分组');
  console.log('分组内的日志');
  console.groupEnd();
  
  // 使用 table 打印表格形式的日志
  const data = [{ name: 'John', age: 28 }, { name: 'Alice', age: 24 }];
  console.table(data);
  
  // 使用 assert 进行断言，如果条件不满足则输出错误信息
  console.assert(1 === 2, '断言失败，输出错误信息');
  ```

### 断点调试

#### 1. 断点

- **内容介绍：** 断点是调试过程中的标记，它允许你在代码执行到特定位置时停止执行，方便你逐步检查代码。

- **设置断点：** 在开发者工具的“Sources”或“Debugger”选项卡中，找到要设置断点的代码行，点击行号左侧即可设置断点。

- 例子：

  ```js
  function exampleFunction() {
    let x = 10;
    let y = 20;
    let result = x + y; // 设置断点
    console.log(result);
  }
  exampleFunction();
  ```

#### 2. 条件断点

- **内容介绍：** 条件断点是一种特殊的断点，只有当指定条件满足时才会触发断点停止执行。

- **设置条件断点：** 在设置断点后，右键点击断点图标，选择“Edit Breakpoint”，然后可以输入条件表达式。

- 例子：

  ```js
  let i = 0;
  while (i < 5) {
    console.log(i);
    i++;
  }
  ```

  在上述代码中，你可以设置一个条件断点，条件为 

  ```js
  i === 3
  ```

  ，这样当 i 等于 3 时会触发断点。

#### 3. 执行方式

- **内容介绍：** 在调试过程中，你可以选择不同的执行方式，如单步执行、继续执行等，以便更灵活地控制调试流程。
- 执行方式：
  - **单步执行（Step Over）：** 逐行执行代码，不进入函数内部。
  - **进入函数（Step Into）：** 如果当前行包含函数调用，进入函数内部执行。
  - **跳出函数（Step Out）：** 执行完当前函数的剩余代码，并跳回到调用该函数的地方。
  - **继续执行（Resume）：** 从当前位置继续执行，直到下一个断点或程序结束。
- **例子：** 在调试器的“Debugger”选项卡中，你可以使用上述执行方式按钮来控制代码的逐步执行。

### 错误

### 错误处理

#### 1. 捕获错误

- **内容介绍：** 在JavaScript中，通过使用 `try`、`catch`、`finally` 关键字来捕获和处理错误，从而使程序能够更加健壮。

- 使用方式：

  ```js
  try {
    // 可能会引发异常的代码
  } catch (error) {
    // 异常处理代码
    console.error(error.message);
  } finally {
    // 最终执行的代码，无论是否发生异常都会执行
  }
  ```

- 例子：

  ```js
  try {
    let result = x / y; // 如果y为0，将抛出除以零的错误
    console.log(result);
  } catch (error) {
    console.error('发生错误：' + error.message);
  } finally {
    console.log('最终执行的代码');
  }
  ```

#### 2. 抛出错误

- **内容介绍：** 在JavaScript中，通过 `throw` 关键字可以手动抛出一个错误，可以是内置的Error对象或自定义的错误对象。

- 使用方式：

  ```js
  
  throw new Error('错误消息');
  ```

- 例子：

  ```js
  function divide(x, y) {
    if (y === 0) {
      throw new Error('除数不能为零');
    }
    return x / y;
  }
  
  try {
    let result = divide(10, 0);
    console.log(result);
  } catch (error) {
    console.error('发生错误：' + error.message);
  }
  ```

以上是关于错误的捕获和抛出的基本介绍。通过使用 `try`、`catch`、`finally` 可以有效地处理代码中可能出现的异常，而通过 `throw` 可以手动引发错误。这些机制有助于提高代码的健壮性和可维护性。

#### 常见错误

1. **SyntaxError（语法错误）:**

   - **描述：** 代码中存在语法错误，违反了JavaScript语法规则。

   - 例子：

     ```js
     let x = 10;
     if (x == 10 {  // 缺少右括号
       console.log('x 等于 10');
     }
     ```

2. **ReferenceError（引用错误）:**

   - **描述：** 尝试访问未声明的变量或未定义的对象属性。

   - 例子：

     ```js
     console.log(y); // y未定义
     ```

3. **TypeError（类型错误）:**

   - **描述：** 变量或参数的类型不符合预期，无法执行特定的操作。

   - 例子：

     ```js
     let num = 'abc';
     console.log(num.toUpperCase()); // num 不是字符串类型，无法调用 toUpperCase 方法
     ```

4. **RangeError（范围错误）:**

   - **描述：** 数值超出有效范围，例如数组长度为负数。

   - 例子：

     ```js
     let arr = new Array(-1); // 数组长度不能为负数
     ```

5. **URIError（URI错误）:**

   - **描述：** 与 URI 相关的函数（比如 decodeURIComponent）使用了无效的参数。

   - 例子：

     ```js
     decodeURIComponent('%'); // 无效的 URI 编码
     ```

6. **EvalError（评估错误）:**

   - **描述：** 在使用全局函数 eval() 时发生的错误（在现代 JavaScript 中，很少会遇到这个错误）。

   - 例子：

     ```js
     
     eval('alert("Hello, World!")'); // 在严格模式下可能会抛出 EvalError
     ```



## Ajax

### 入门

让我们来了解一下Ajax（Asynchronous JavaScript and XML）技术。Ajax是一种用于创建异步网络应用的技术，它使得在不重新加载整个页面的情况下，能够向服务器发送请求并获取数据。

以下是使用Ajax的基本步骤：

1. **创建一个XMLHttpRequest对象：** 在现代浏览器中，你可以使用`XMLHttpRequest`对象来创建一个HTTP请求。示例代码如下：

   ```js
   var xhttp = new XMLHttpRequest();
   ```

2. **指定请求的类型、URL以及是否异步：** 设置请求的方法（GET或POST）、URL以及是否异步。异步是Ajax的关键，它允许页面在等待服务器响应的同时执行其他操作。示例代码如下：

   ```js
   xhttp.open("GET", "https://example.com/api/data", true);
   ```

3. **定义响应函数：** 在请求的`onreadystatechange`事件中定义一个函数，该函数将在服务器响应发生变化时被调用。通常，在`readyState`为4（表示请求已完成）且`status`为200（表示成功）时执行相应的操作。示例代码如下：

   ```js
   xhttp.onreadystatechange = function() {
     if (this.readyState == 4 && this.status == 200) {
       // 处理服务器响应的数据
       console.log(this.responseText);
     }
   };
   ```

4. **发送请求：** 最后，使用`send`方法发送请求。如果是GET请求，可以将参数附加在URL上；如果是POST请求，需要在`send`方法中传递参数。示例代码如下：

   ```js
   xhttp.send();
   ```

### AJAX概述

AJAX的全称为（Asynchronous JavaScript and XML，异步JavaScript和XML） ，是Web开发应用的一个里程碑

在用户和服务器之间引入了一个中间媒介，从而改变了同步交互过程中“处理－等待－处理－等待”的模式

揭开了无刷新更新页面的新时代，代替传统Web请求方式和通过隐藏的框架来进行异步提交的趋势

AJAX独立于用户与Web服务器之间的交互，数据编辑、页面导航和数据验证等操作不再需要重新加载整个页面

### XMLHttpRequest的创建

创建`XMLHttpRequest`对象，并且在不同的浏览器中有不同的实现方式。这是因为不同的浏览器在支持Ajax时采用了不同的技术实现。

在现代的浏览器中，你可以使用`window.XMLHttpRequest`来检查是否支持`XMLHttpRequest`对象。如果支持，就直接使用`new XMLHttpRequest()`来创建对象。这是因为现代浏览器通常都支持这个标准的方式。

在某些旧版本的Internet Explorer浏览器中，`XMLHttpRequest`对象可能不被支持，因此需要使用`ActiveXObject`来创建一个类似的对象。在这种情况下，你可以通过检查`window.ActiveXObject`来确定浏览器是否支持这种方式，并使用`new ActiveXObject("Microsoft.XMLHTTP")`来创建对象。

下面是一个结合判断的完整示例：

```js
var xhr;

if (window.XMLHttpRequest) {
  // 现代浏览器
  xhr = new XMLHttpRequest();
} else if (window.ActiveXObject) {
  // IE浏览器
  try {
    xhr = new ActiveXObject("Microsoft.XMLHTTP");
  } catch (e) {
    // 可能存在某些IE版本不支持
    console.error("Error creating XMLHttpRequest object:", e);
  }
} else {
  // 不支持Ajax方式
  console.error("Ajax not supported in this browser");
}

// 接下来，你可以继续使用xhr对象进行Ajax请求
```

这种方法确保了在现代浏览器和一些旧版本的IE浏览器中都能够正确创建`XMLHttpRequest`对象。

### XMLHttpRequest简单流程

### 同步方式：

```js
var xhr = new XMLHttpRequest(); // 创建
xhr.open("GET", "/test.json", false); // 目标(绝对相对网址)，false 表示同步
xhr.send(); // 发送
console.log(xhr.status + ':' + xhr.responseText); // 内容
```

这是一个同步的Ajax请求，其中：

- `xhr.open("GET", "/test.json", false);` 指定了请求的目标为"/test.json"，并设置为同步请求（`false`表示同步）。
- `xhr.send();` 发送了请求，代码会等待服务器响应，直到请求完成为止。
- `console.log(xhr.status + ':' + xhr.responseText);` 打印了服务器的响应状态码和响应文本。

### 异步方式：

```js
var xhr = new XMLHttpRequest(); // 创建
xhr.open("GET", "/test.json", true); // 目标，true 表示异步
xhr.onreadystatechange = function (e) {
  if (xhr.readyState != 4) return; // 不是就绪状态
  console.log(xhr.status + ':' + xhr.responseText); // 内容
}
xhr.send(); // 发送
console.log('OK');
```

这是一个异步的Ajax请求，其中：

- `xhr.open("GET", "/test.json", true);` 指定了请求的目标为"/test.json"，并设置为异步请求（`true`表示异步）。
- `xhr.onreadystatechange` 是一个回调函数，当`xhr`对象的状态改变时，该函数将被调用。在这里，我们检查`xhr.readyState`是否为4（表示请求完成），然后打印服务器的响应状态码和响应文本。
- `xhr.send();` 发送了异步请求，代码继续执行而不等待服务器响应。
- `console.log('OK');` 这行代码会在请求发送后立即执行，而不等待响应。

总的来说，异步方式的优势在于不会阻塞页面的其他操作，而同步方式会导致页面在等待响应时被冻结。在现代Web开发中，一般推荐使用异步方式。

### XMLHttpRequest的属性

1. **`readyState`（只读）：** 表示当前请求的状态，具体取值如下：
   - 0: 请求未初始化
   - 1: 服务器连接已建立
   - 2: 请求已接收
   - 3: 请求处理中
   - 4: 请求已完成，且响应已就绪
2. **`responseType`：** 在调用`send()`方法前设置，用于指定返回的响应数据类型，例如`"text"`、`"json"`、`"blob"`等。
3. **`responseBody`（只读）：** 返回信息的无符号字节数组形式。
4. **`responseStream`（只读）：** 返回信息的ADO Stream对象形式。
5. **`responseText`（只读）：** 返回信息的字符串形式。
6. **`responseXML`（只读）：** 返回信息的XML Document对象形式。
7. **`status`（只读）：** 返回信息的HTTP状态码。
8. **`statusText`（只读）：** 返回信息的响应行文本。
9. **`timeout`：** 异步请求的超时时间（毫秒）。需要在调用`open()`方法后、`send()`方法前进行设置。早期浏览器可能不支持。
10. **`withCredentials`：** 一个布尔值，默认为`false`。表示跨域请求是否携带凭据（如Cookie或HTTP认证信息）。

这些属性为开发者提供了对Ajax请求和其结果的详细控制和访问。在实际应用中，可以利用这些属性来处理不同的响应类型、状态变化等情况。

### XMLHttpRequest的responseType

`XMLHttpRequest`的`responseType`属性用于指定服务器返回的数据类型。以下是常见的`responseType`值及其含义：

1. **`""`（空字符串）：** 将`responseType`设为空字符串与设置为`text`相同，表示返回的数据将以字符串（DOMString）形式处理，这是默认类型。
2. **`arraybuffer`：** 表示返回的数据将以JavaScript的ArrayBuffer对象形式处理，用于处理二进制数据。
3. **`blob`：** 表示返回的数据将以Blob对象形式处理，适用于处理二进制数据。请注意，部分浏览器可能不支持此类型。
4. **`document`：** 表示返回的数据将以HTML Document或XML XMLDocument形式处理，具体取决于接收到的数据的MIME类型。
5. **`json`：** 表示返回的数据将被视为JSON，自动解析为JavaScript对象。
6. **`text`：** 表示返回的数据将包含在DOMString对象中的文本。请注意，IE10/IE11不支持这个类型。
7. **`moz-chunked-arraybuffer`：** 类似于`arraybuffer`，但数据将以流的形式接收。在使用此响应类型时，响应中的值仅在progress事件的处理程序中可用，并且只包含上一次响应progress事件以后收到的数据，而不是自请求发送以来收到的所有数据。在progress事件处理时访问`response`将返回到目前为止收到的数据。在progress事件处理程序之外访问，`response`的值会始终为`null`。
8. **`ms-stream`：** 表示返回的数据将以unsigned byte数组形式处理，仅在IE中可用。

选择适当的`responseType`取决于你期望从服务器接收到的数据类型。

### XMLHttpRequest的方法

1. **`abort()`：** 用于取消当前的请求。

   ```js
   
   xhr.abort();
   ```

2. **`getAllResponseHeaders()`：** 获取所有响应的HTTP头，返回一个包含所有头信息的字符串。

   ```js
   
   var allHeaders = xhr.getAllResponseHeaders();
   ```

3. **`getResponseHeader(headerName)`：** 从响应信息中获取指定的HTTP头。

   ```js
   
   var contentType = xhr.getResponseHeader("Content-Type");
   ```

4. **`open(method, url, async, user, password)`：** 创建一个新的HTTP请求，并指定此请求的方法、URL以及验证信息（可选的用户名和密码）。

   ```js
   
   xhr.open("GET", "/example/api", true, "username", "password");
   ```

5. **`send(data)`：** 发送请求到HTTP服务器并接收回应。可以传递可选的数据参数，适用于POST请求。

   ```js
   
   xhr.send();
   ```

6. **`setRequestHeader(header, value)`：** 单独指定请求的某个HTTP头。必须在`open()`之后调用，`send()`之前调用。

   ```js
   
   xhr.setRequestHeader("Content-Type", "application/json");
   ```

这些方法提供了对`XMLHttpRequest`对象的进一步控制，允许你在请求过程中进行取消、获取响应头、设置请求头等操作。请注意，一些方法的调用顺序是有讲究的，例如在调用`setRequestHeader`之前必须先调用`open`。

### XMLHttpRequest的事件

1. **`onreadystatechange`：** 当`readyState`属性改变时触发，表示请求的状态发生了变化。注意，当`readyState`由非0值变为0时，不会触发该事件。

   ```js
   xhr.onreadystatechange = function() {
     if (xhr.readyState == 4 && xhr.status == 200) {
       // 请求已完成，可以处理响应
     }
   };
   ```

2. **`onloadstart`：** 在调用`send()`方法后立即触发，表示请求开始。

   ```js
   xhr.onloadstart = function() {
     // 请求开始时执行的代码
   };
   ```

3. **`onprogress`：** 在上传阶段（`send()`之后，`readyState`为2之前）和下载阶段（`readyState`为3时）触发，每50ms触发一次。

   ```js
   xhr.onprogress = function(event) {
     // 处理上传或下载的进度
   };
   ```

4. **`onload`：** 当请求成功完成时触发，此时`readyState`为4。

   ```js
   xhr.onload = function() {
     // 请求成功完成时执行的代码
   };
   ```

5. **`onloadend`：** 当请求结束（包括请求成功和请求失败）时触发。

   ```js
   xhr.onloadend = function() {
     // 请求结束时执行的代码
   };
   ```

6. **`onabort`：** 当调用`abort()`方法后触发。

   ```js
   xhr.onabort = function() {
     // 请求被取消时执行的代码
   };
   ```

7. **`ontimeout`：** 当设置了超时时间（`timeout`不等于0）并在`onloadstart`开始后超时未发生`onloadend`时触发。

   ```js
   xhr.ontimeout = function() {
     // 超时时执行的代码
   };
   ```

8. **`onerror`：** 发生网络错误时触发。

   ```js
   xhr.onerror = function() {
     // 网络错误时执行的代码
   };
   ```

这些事件提供了对Ajax请求过程中不同阶段的控制和处理机会，使开发者能够更好地处理请求的状态变化和处理响应。

## JSON

### 概述

JSON(JavaScript Object Notation)JavaScript对象表示法

JSON是Douglas Crockford在2001年开始推广使用

在2005年-2006年正式成为主流的数据格式

成为Standard ECMA-262 3rd Edition - December 1999的子集

SON（JavaScript Object Notation）是一种轻量级的数据交换格式。它是一种易于人阅读和编写，同时也易于机器解析和生成的文本格式。JSON是基于JavaScript语言的，但它是一种独立于语言的数据格式，因此可以被多种编程语言使用。

### JSON的特点：

1. **简洁性：** JSON采用键值对的方式表示数据，使得数据结构清晰简洁，易于理解和阅读。
2. **易于扩展：** 可以很容易地向JSON中添加新的数据类型，而无需更改解析JSON的代码。
3. **自描述性：** JSON数据是自描述的，每个数据字段都有对应的键名，使得数据的含义更加清晰。
4. **跨语言性：** JSON数据格式是独立于语言的，因此可以在不同编程语言之间进行轻松的数据交换。

### JSON的基本语法：

- **对象（Object）：** 由键值对组成，键和值之间使用冒号分隔，不同键值对之间使用逗号分隔，整个对象使用花括号括起来。

  ```json
  {
    "name": "John",
    "age": 30,
    "city": "New York"
  }
  ```

- **数组（Array）：** 有序列表，使用方括号括起来，数组中的元素可以是任意数据类型，包括对象和数组。

  ```json
  
  ["apple", "orange", "banana"]
  ```

- **值：** 可以是字符串、数字、布尔值、对象、数组、null等。

  ```json
  {
    "name": "Alice",
    "age": 25,
    "isStudent": true,
    "grades": [95, 87, 92],
    "address": {
      "street": "123 Main St",
      "city": "Cityville"
    },
    "isMarried": null
  }
  ```

### JSON与JavaScript的关系：

JSON的语法是JavaScript对象表示法的子集，这意味着几乎所有的JavaScript对象都可以表示为JSON。在JavaScript中，可以使用`JSON.stringify()`将对象转换为JSON字符串，而使用`JSON.parse()`将JSON字符串转换为JavaScript对象。

```js
// JavaScript对象
var person = { "name": "John", "age": 30, "city": "New York" };

// 将JavaScript对象转换为JSON字符串
var jsonStr = JSON.stringify(person);
console.log(jsonStr);

// 将JSON字符串转换为JavaScript对象
var jsonObj = JSON.parse(jsonStr);
console.log(jsonObj);
```

JSON在Web开发中广泛应用于数据传输和配置文件等领域，它的简洁性和跨语言性使得它成为一种优秀的数据交换格式。

### JSON-value

在JSON（JavaScript Object Notation）中，一个 "JSON value" 表示 JSON 数据的最小单元，它可以是以下几种类型之一：

1. **字符串（String）：** 表示文本数据，使用双引号括起来。

   ```json
   
   "Hello, World!"
   ```

2. **数字（Number）：** 表示数值数据，可以是整数或浮点数。

   ```json
   
   42
   ```

   ```json
   
   3.14
   ```

3. **布尔值（Boolean）：** 表示逻辑值，可以是 `true` 或 `false`。

   ```json
   
   true
   ```

4. **对象（Object）：** 表示键值对集合，使用花括号括起来。

   ```json
   
   {"name": "John", "age": 30}
   ```

5. **数组（Array）：** 表示有序的值列表，使用方括号括起来。

   ```json
   
   ["apple", "orange", "banana"]
   ```

6. **空值（null）：** 表示空值。

   ```json
   
   null
   ```

### 内嵌对象

在 JavaScript 中，JSON 内嵌对象通常是指 JSON 对象中包含其他 JSON 对象的情况。下面我将解释与 JSON 内嵌对象相关的几个概念和问题。

### 1. JSON.parse(String):

`JSON.parse()` 方法用于解析 JSON 字符串，将其转换为对应的 JavaScript 对象。

```js
var jsonString = '{"name": "John", "age": 30}';
var jsonObj = JSON.parse(jsonString);
console.log(jsonObj);
```

### 2. JSON.stringify(Value):

`JSON.stringify()` 方法用于将 JavaScript 对象转换为 JSON 字符串。

```js
var obj = { a: 1, f: function(x) { x++; } };
var jsonString = JSON.stringify(obj);
console.log(jsonString);
```

请注意，`JSON.stringify()` 在处理函数时会将函数忽略，因此在上述例子中，函数 `f` 不会出现在生成的 JSON 字符串中。

### 3. 循环引用问题:

当对象存在循环引用（对象之间相互引用）时，使用 `JSON.stringify()` 可能会导致问题，因为 JSON 不支持循环引用。

```js
var obj = { a: 1, b: {} };
obj.c = obj.b;
obj.b.x = obj.c;

try {
  var jsonString = JSON.stringify(obj);
} catch (error) {
  console.error(error.message); // TypeError: Converting circular structure to JSON
}
```

上述例子中，`obj` 对象存在循环引用，尝试使用 `JSON.stringify()` 会抛出 `TypeError`。

解决循环引用问题的一种方式是在调用 `JSON.stringify()` 时传递一个 replacer 函数，用于控制对象的序列化过程。

```js
var obj = { a: 1, b: {} };
obj.c = obj.b;
obj.b.x = obj.c;

var jsonString = JSON.stringify(obj, function(key, value) {
  if (key !== "" && value === obj) {
    return undefined; // 遇到循环引用时返回 undefined
  }
  return value;
});

console.log(jsonString);
```

这样可以避免抛出错误，但需要注意，在这种情况下，生成的 JSON 字符串中会缺少循环引用的部分。解决循环引用问题需要谨慎处理，具体方案可能取决于你的应用场景。
