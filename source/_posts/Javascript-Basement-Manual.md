---
title: Javascript Basement Quick Overview - Interactive Front-end Development
date: 2023-11-07 20:58:48
tags: 前端技术
categories:
- 学习
- 计算机
- 前端
cover: https://bairesdev.mo.cloudinary.net/blog/2023/08/What-Is-JavaScript-Used-For.jpg?tx=w_3840,q_auto
---

<body>
<p>Javascript，live your pages.</p>
<!--more-->
<h2 id='qa'>Q&amp;A</h2>
<h3 id='javascript工作原理'>JavaScript工作原理</h3>
<p>JavaScript是一种用于网页交互的脚本语言，它主要通过以下步骤来工作：</p>
<ol start='' >
<li><p><strong>访问HTML (Visit HTML):</strong> JavaScript通常嵌入在HTML文档中，并通过<code>&lt;script&gt;</code>标签嵌入到HTML代码中。当浏览器加载页面时，会解释并执行嵌入的JavaScript代码。</p>
<p>示例：</p>
<pre><code class='language-javascript' lang='javascript'>html&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;en&quot;&gt;
&lt;head&gt;
    &lt;meta charset=&quot;UTF-8&quot;&gt;
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
    &lt;title&gt;JavaScript Example&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;!-- JavaScript代码嵌入在这里 --&gt;
    &lt;script&gt;
        // JavaScript代码
    &lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;
</code></pre>
</li>
<li><p><strong>修改内容 (Modify Content):</strong> JavaScript可以通过操作文档对象模型（DOM）来动态修改网页内容。DOM表示网页的结构，通过JavaScript，可以添加、删除或修改HTML元素、属性和文本内容。</p>
<p>示例：</p>
<pre><code class='language-javascript' lang='javascript'>javascript// 获取元素并修改内容
var element = document.getElementById(&quot;myElement&quot;);
element.innerHTML = &quot;新的内容&quot;;
</code></pre>
</li>
<li><p><strong>制定规则 (Make Rules):</strong> JavaScript用于制定网页的行为规则，包括对数据的处理、条件判断、循环等。这有助于实现动态和交互式的用户体验。</p>
<p>示例：</p>
<pre><code class='language-javascript' lang='javascript'>javascript// 制定规则 - 条件判断
var age = 20;
if (age &gt;= 18) {
    console.log(&quot;成年人&quot;);
} else {
    console.log(&quot;未成年人&quot;);
}
</code></pre>
</li>
<li><p><strong>响应事件 (Respond to Events):</strong> JavaScript使网页能够对用户的交互作出响应，例如点击按钮、提交表单等。通过事件处理程序，可以定义在事件发生时执行的操作。</p>
<p>示例：</p>
<pre><code class='language-javascript' lang='javascript'>html&lt;!-- HTML中的按钮 --&gt;
&lt;button id=&quot;myButton&quot; onclick=&quot;myFunction()&quot;&gt;点击我&lt;/button&gt;

&lt;!-- JavaScript中的事件处理程序 --&gt;
&lt;script&gt;
    function myFunction() {
        alert(&quot;按钮被点击了！&quot;);
    }
&lt;/script&gt;
</code></pre>
</li>

</ol>
<p>这些步骤使JavaScript成为一种强大的客户端脚本语言，为网页提供了丰富的交互和动态性。</p>
<h3 id='什么是脚本'>什么是脚本？</h3>
<p><strong>脚本（Script）</strong> 是一系列命令或指令的集合，通常编写成文本文件。这些命令按照一定的顺序执行，用于完成特定的任务或操作。脚本通常用于自动化任务、批处理处理、或在特定条件下触发一系列操作。</p>
<p>在计算机编程领域，脚本通常是解释性语言编写的，与编译型语言相对。脚本语言的特点是代码不需要事先编译成机器码，而是由解释器逐行解释执行。</p>
<p>对于JavaScript来说，它是一种脚本语言，用于在Web浏览器中添加交互性。JavaScript代码以脚本的形式嵌入在HTML文档中，由浏览器解释执行。这使得开发人员能够在网页上创建动态、交互式的用户体验，通过一系列的脚本命令来修改文档内容、响应事件等。</p>
<p>总体而言，脚本是一种轻量级的编程方式，适用于一些需要快速执行、适应变化的场景。</p>
<h3 id='如何编写脚本'>如何编写脚本？</h3>
<p>编写脚本通常可以分为以下步骤：目标（Goal）-&gt; 任务（Tasks）-&gt; 编码（Coding）。</p>
<ol start='' >
<li><p><strong>明确目标 (Goal):</strong> 首先，明确你的脚本的目标是什么。确定你想要实现的最终结果，这有助于指导后续的编码过程。</p>
</li>
<li><p><strong>分解任务 (Tasks):</strong> 将整个目标分解为小的、可管理的任务。每个任务应该对应脚本中的一个功能或操作。这有助于组织代码，使其更易于理解和维护。</p>
</li>
<li><p><strong>编写代码 (Coding):</strong> 针对每个任务，编写相应的代码来实现它。使用适当的编程语言，并根据任务的要求选择合适的数据结构、算法和控制流程。</p>
<p>示例（伪代码）：</p>
<pre><code class='language-plaintext' lang='plaintext'>plaintext// 目标：计算并输出两个数的和

// 任务1: 获取用户输入
输入第一个数
输入第二个数

// 任务2: 计算和
和 = 第一个数 + 第二个数

// 任务3: 输出结果
输出和
</code></pre>
<p>&nbsp;</p>
</li>
<li><p><strong>测试和调试 (Testing and Debugging):</strong> 编写完代码后，进行测试以确保脚本按照预期工作。调试任何潜在的错误或问题，并确保脚本的稳定性和正确性。</p>
</li>
<li><p><strong>文档 (Documentation):</strong> 为你的脚本编写文档，描述脚本的目的、用法和任何特殊注意事项。这有助于其他人理解和使用你的脚本。</p>
</li>
<li><p><strong>优化 (Optimization):</strong> 针对性能和代码质量进行优化。检查是否有冗余的代码，是否有更有效的方法实现相同的功能。</p>
</li>

</ol>
<p>记住，编写脚本是一个迭代的过程。在编码和测试过程中可能会发现一些需要调整的地方，因此保持灵活性并根据需要进行修改。</p>
<h3 id='对象和属性'>对象和属性</h3>
<p>在计算机编程中，对象和属性是用于帮助计算机理解和处理世界的概念。</p>
<p><strong>对象 (Object):</strong> 对象是现实生活中或计算机程序中的实体，可以具有状态和行为。在编程中，对象通常是具有相关属性和方法的实例。例如，一个表示汽车的对象可以有属性（颜色、型号）和方法（启动、停止）。</p>
<p><strong>属性 (Attribute):</strong> 属性是对象的特征或状态，描述对象的某个方面。属性可以是对象的数据，例如颜色、大小、重量等。通过访问对象的属性，我们可以了解或修改对象的状态。</p>
<p><strong>事件 (Event):</strong> 事件是对象发生的动作或事情，可以触发相应的响应。在编程中，事件通常与用户交互有关，例如点击按钮、输入文本等。处理事件的代码被称为事件处理程序。</p>
<p>例如（伪代码）：</p>
<pre><code class='language-plaintext' lang='plaintext'>plaintext// 创建汽车对象
car = {
    color: &quot;blue&quot;,         // 属性: 颜色
    model: &quot;sedan&quot;,        // 属性: 型号

    start: function() {    // 方法: 启动
        // 启动汽车的代码
    },

    stop: function() {     // 方法: 停止
        // 停止汽车的代码
    }
}

// 访问汽车对象的属性和方法
car.color             // 输出: &quot;blue&quot;
car.start()           // 启动汽车
</code></pre>
<p>通过使用对象、属性和方法，计算机可以模拟现实世界中的实体和动作，从而更好地理解和处理程序的逻辑。这种面向对象的编程方法有助于组织和抽象复杂的系统。</p>
<h3 id='网页浏览器的工作原理'>网页浏览器的工作原理</h3>
<p>网页浏览器是用于显示和解释网页内容的软件应用程序。它的工作涉及多个对象和步骤。</p>
<p><strong>对象:</strong></p>
<ol start='' >
<li><p><strong>Window（窗口）:</strong></p>
<ul>
<li>代表浏览器窗口，是浏览器的顶层对象。它包含了整个浏览器窗口的信息，以及全局的JavaScript对象和方法。</li>

</ul>
</li>
<li><p><strong>Document（文档）:</strong></p>
<ul>
<li>代表当前加载的网页文档，即HTML文档。它提供了对文档内容的访问和操作，如修改元素、添加事件等。</li>

</ul>
</li>

</ol>
<p><strong>步骤:</strong></p>
<ol start='' >
<li><p><strong>接收HTML（Receive an HTML）:</strong></p>
<ul>
<li>当用户在浏览器中输入URL或点击链接时，浏览器发送请求到服务器，并接收服务器返回的HTML文件。这个HTML文件包含了网页的结构和内容。</li>

</ul>
</li>
<li><p><strong>建模和存储到内存（Modeling and Storage to Memory）:</strong></p>
<ul>
<li>浏览器解析HTML文档，构建文档对象模型（DOM）和样式表对象模型（CSSOM）。DOM表示网页的结构，CSSOM表示网页的样式。这些模型被存储在浏览器的内存中，以便后续的渲染过程使用。</li>

</ul>
</li>
<li><p><strong>渲染（Rendering）:</strong></p>
<ul>
<li>浏览器通过将DOM和CSSOM合并成渲染树（Render Tree），然后通过布局（Layout）和绘制（Painting）的过程，将网页呈现到屏幕上。JavaScript代码也可能在这个阶段修改DOM，触发重新渲染。</li>

</ul>
</li>

</ol>
<p>这些步骤是简化的概括，实际上浏览器的工作涉及更多的细节和优化。浏览器还涉及其他对象和组件，如网络模块、解析器、JavaScript引擎等，以提供完整的浏览体验。</p>
<p>总体而言，浏览器的工作可以看作是将从服务器获取的HTML、CSS和JavaScript文件转化为用户可视化的网页。这个过程包括了解析、建模、存储和渲染等多个步骤。</p>
<h3 id='htmlcss和js如何协同工作'>HTML、CSS和JS如何协同工作？</h3>
<p>HTML、CSS和JavaScript通常一起协同工作，分别负责内容、视觉效果和交互动作。</p>
<ol start='' >
<li><p><strong>HTML（内容）:</strong></p>
<ul>
<li>HTML（超文本标记语言）用于定义网页的结构和内容。它包含了页面上的各种元素，如文本、图像、链接等。HTML提供了页面的骨架，但它通常没有处理页面的外观和行为。</li>

</ul>
</li>
<li><p><strong>CSS（视觉效果）:</strong></p>
<ul>
<li>CSS（层叠样式表）用于控制HTML元素的样式和布局。通过选择器和规则，CSS可以指定元素的颜色、字体、大小、位置等样式。CSS为网页提供了外观和样式，使其更具吸引力和可读性。</li>

</ul>
</li>
<li><p><strong>JavaScript（动作）:</strong></p>
<ul>
<li>JavaScript是一种脚本语言，用于添加网页的交互性和动态性。它可以修改HTML和CSS，响应用户的操作，处理数据等。JavaScript通过DOM（文档对象模型）和CSSOM（样式表对象模型）与HTML和CSS进行交互，使网页更具活力。</li>

</ul>
</li>

</ol>
<h3 id='如何连接js和html'>如何连接JS和HTML？</h3>
<p>在HTML文件中，通过<code>&lt;script&gt;</code>标签可以将JavaScript代码嵌入到HTML文档中。这可以在文档的头部或尾部完成，例如：</p>
<pre><code class='language-html' lang='html'>html&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;en&quot;&gt;
&lt;head&gt;
    &lt;meta charset=&quot;UTF-8&quot;&gt;
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
    &lt;title&gt;HTML, CSS, and JS&lt;/title&gt;
    &lt;!-- 连接JS文件 --&gt;
    &lt;script src=&quot;myscript.js&quot;&gt;&lt;/script&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;!-- 页面内容 --&gt;
&lt;/body&gt;
&lt;/html&gt;
</code></pre>
<p>在上面的例子中，<code>myscript.js</code>是包含JavaScript代码的外部文件，通过<code>&lt;script&gt;</code>标签的<code>src</code>属性进行引用。</p>
<h3 id='调试方法'>调试方法？</h3>
<p>在调试过程中，可以使用以下方法：</p>
<ul>
<li><strong>console.log():</strong> 在JavaScript代码中插入<code>console.log()</code>语句，将变量的值或特定信息输出到浏览器的开发者工具控制台，以便检查代码的执行过程。</li>
<li><strong>浏览器开发者工具:</strong> 现代浏览器提供了开发者工具，其中包含调试器。在调试器中，可以逐行执行代码、设置断点、监视变量等，以便更详细地分析和修复问题。可以通过按F12或右键点击页面并选择&quot;检查&quot;来打开开发者工具。</li>

</ul>
<p>这些调试方法有助于识别和修复HTML、CSS和JavaScript代码中的错误，确保它们协同工作以实现预期的效果和功能。</p>
<p>&nbsp;</p>
<h2 id='基础的基础'>基础的基础</h2>
<p>在编程中，有一些基础的概念和操作，其中包括注释、变量和数据类型。</p>
<h4 id='注释comment）'>注释（Comment）</h4>
<p>注释用于在代码中添加说明性的文字，这些文字不会被计算机执行，而是用于帮助人们理解代码。在JavaScript中，单行注释使用<code>//</code>，多行注释使用<code>/* */</code>。</p>
<pre><code>javascript// 这是单行注释

/*
   这是
   多行
   注释
*/
</code></pre>
<h4 id='变量variable）'>变量（Variable）</h4>
<p>变量用于存储和表示数据。在JavaScript中，使用<code>var</code>关键字来声明变量。变量可以存储不同数据类型的值，例如数字、字符串、数组等。</p>
<pre><code>javascriptvar x = 5;         // 数字
var name = &quot;John&quot;; // 字符串
var numbers = [1, 2, 3]; // 数组
var status;        // 未定义的变量
</code></pre>
<h4 id='数据类型data-type）'>数据类型（Data Type）</h4>
<p>JavaScript中有多种数据类型，其中包括：</p>
<ul>
<li><strong>数字（Number）:</strong> 表示数值，如 <code>5</code> 或 <code>3.14</code>。</li>
<li><strong>字符串（String）:</strong> 表示文本，用引号括起来，如 <code>&quot;Hello&quot;</code>。</li>
<li><strong>数组（Array）:</strong> 用于存储多个值的有序集合，如 <code>[1, 2, 3]</code>。</li>
<li><strong>未定义（Undefined）:</strong> 表示变量没有被赋值。</li>
<li>等等...</li>

</ul>
<pre><code>javascriptvar num = 10;          // 数字
var greeting = &quot;Hi&quot;;   // 字符串
var colors = [&quot;red&quot;, &quot;green&quot;, &quot;blue&quot;]; // 数组
var notDefined;        // 未定义
</code></pre>
<h4 id='尝试'>尝试：</h4>
<p>在JavaScript中，使用以下方法可以尝试操作HTML文档：</p>
<ul>
<li><strong><code>document.getElementById()</code>:</strong> 通过元素的ID获取HTML元素。</li>
<li><strong><code>document.write()</code>:</strong> 将内容写入文档。</li>
<li><strong><code>[element].textContent = [\*]</code>:</strong> 设置元素的文本内容。</li>

</ul>
<pre><code>javascript// 尝试获取ID为 &quot;myElement&quot; 的元素
var myElement = document.getElementById(&quot;myElement&quot;);

// 将文本写入文档
document.write(&quot;Hello, World!&quot;);

// 尝试设置元素的文本内容
myElement.textContent = &quot;New Text&quot;;
</code></pre>
<p>这些基础操作为编写简单的JavaScript代码和与HTML文档交互提供了一些起点。</p>
<p>&nbsp;</p>
<h2 id='函数方法和对象'>函数、方法和对象</h2>
<h3 id='函数function）'>函数（Function）</h3>
<p>在JavaScript中，函数用于执行特定任务或操作。函数通常由函数名、参数和函数体组成。可以使用<code>return</code>语句返回值。示例：</p>
<pre><code>javascript// 命名函数
function addNumbers(num1, num2) {
    var sum = num1 + num2;
    return sum;
}

// 调用函数
var result = addNumbers(3, 5);
console.log(result); // 输出: 8
</code></pre>
<p>匿名函数：</p>
<pre><code>javascriptvar multiply = function(x, y) {
    return x * y;
};
var product = multiply(4, 6);
console.log(product); // 输出: 24
</code></pre>
<h3 id='变量作用域'>变量作用域</h3>
<p>在JavaScript中，变量的作用域分为本地（局部）和全局两种。</p>
<ul>
<li><strong>本地作用域：</strong> 在函数内声明的变量具有本地作用域，仅在该函数内部可见。</li>

</ul>
<pre><code>javascriptfunction example() {
    var localVar = &quot;I am local&quot;;
    console.log(localVar);
}

example();      // 输出: &quot;I am local&quot;
console.log(localVar);  // 错误，localVar 在这里不可见
</code></pre>
<ul>
<li><strong>全局作用域：</strong> 在函数外声明的变量具有全局作用域，可在整个程序中访问。</li>

</ul>
<pre><code>javascriptvar globalVar = &quot;I am global&quot;;

function example() {
    console.log(globalVar);
}

example();      // 输出: &quot;I am global&quot;
console.log(globalVar);  // 输出: &quot;I am global&quot;
</code></pre>
<h3 id='对象object）'>对象（Object）</h3>
<p>对象是包含键值对的数据集合。在JavaScript中，对象可以包含属性和方法。</p>
<pre><code>javascript// 对象字面量
var person = {
    firstName: &quot;John&quot;,
    lastName: &quot;Doe&quot;,
    sayHello: function() {
        console.log(&quot;Hello, &quot; + this.firstName + &quot; &quot; + this.lastName);
    }
};

// 访问对象属性
console.log(person.firstName); // 输出: &quot;John&quot;

// 调用对象方法
person.sayHello(); // 输出: &quot;Hello, John Doe&quot;
</code></pre>
<p>对象也可以使用构造函数创建：</p>
<pre><code>javascript// 构造函数
function Person(firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
}

// 创建对象实例
var person = new Person(&quot;John&quot;, &quot;Doe&quot;);
console.log(person.firstName); // 输出: &quot;John&quot;
</code></pre>
<h4 id='访问对象属性'>访问对象属性</h4>
<p>可以使用点号或方括号来访问对象的属性：</p>
<pre><code>javascriptconsole.log(person.firstName); // 使用点号访问
console.log(person[&quot;firstName&quot;]); // 使用方括号访问
</code></pre>
<h4 id='删除对象属性'>删除对象属性</h4>
<p>可以使用 <code>delete</code> 关键字删除对象的属性：</p>
<pre><code>javascript
delete person.lastName; // 删除 lastName 属性
</code></pre>
<p>这些是JavaScript中函数、作用域和对象的基本概念和用法。函数用于执行代码块，作用域定义了变量的可见范围，而对象用于组织和存储数据。</p>
<h4 id='built-in-objects'>Built-in Objects</h4>
<ol start='' >
<li><h4 id='bom---window'>BOM - window</h4>
<pre><code class='language-javascript' lang='javascript'>window.innerHeight;      // 浏览器窗口的内部高度
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
</code></pre>
<p>&nbsp;</p>
</li>

</ol>
<h4 id='dom---document'>DOM - Document</h4>
<p><code>&lt;html&gt;</code></p>
<ol start='' >
<li><p><code>&lt;head&gt;</code></p>
</li>
<li><p><code>&lt;title&gt;</code></p>
</li>
<li><p><code>&lt;body&gt;</code></p>
</li>
<li><p><code>&lt;div&gt;</code></p>
<ol start='' >
<li>attribute</li>

</ol>
</li>
<li><p><code>&lt;p&gt;</code></p>
</li>
<li><p>text</p>
<p>document.title: 获取或设置文档的标题。</p>
<p>document.lastModified: 获取文档的上次修改日期和时间。</p>
<p>document.URL: 获取文档的URL。</p>
<p>document.domain: 获取或设置文档的域。</p>
<p>document.write(): 向文档写入HTML内容。</p>
<p>document.getElementById(): 通过元素的ID获取HTML元素。</p>
<p>document.querySelectorAll(): 通过选择器获取匹配的所有元素。</p>
<p>document.createElement(): 创建新的HTML元素。</p>
<p>document.createTextNode(): 创建新的文本节点。</p>
</li>

</ol>
<pre><code class='language-javascript' lang='javascript'>

示例：

javascript

console.log(document.title);             // 获取文档标题
console.log(document.lastModified);      // 获取上次修改时间
console.log(document.URL);                // 获取文档URL
console.log(document.domain);             // 获取文档域

document.write(&quot;Hello, World!&quot;);         // 向文档写入内容

var myElement = document.getElementById(&quot;myElement&quot;);  // 通过ID获取元素

var elements = document.querySelectorAll(&quot;.myClass&quot;);  // 通过类名获取元素

var newElement = document.createElement(&quot;div&quot;);        // 创建新元素
var newText = document.createTextNode(&quot;New Text&quot;);      // 创建新文本节点
</code></pre>
<p>&nbsp;</p>
<h4 id='全局-javascript-对象'>全局 JavaScript 对象</h4>
<p>JavaScript 提供了一些全局对象，其中包括字符串、数字、布尔、日期、数学和正则表达式对象。以下是其中一些常见的全局对象及其方法：</p>
<ol start='' >
<li><p><strong>String（字符串）:</strong></p>
<pre><code>javascriptvar str = &quot;Hello, World!&quot;;

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
</code></pre>
</li>
<li><p><strong>Number（数字）:</strong></p>
<pre><code>javascriptvar num = 42;

isNaN(num);               // 判断是否为NaN
num.toFixed(n);           // 将数字转为字符串，保留 n 位小数
num.toPrecision(n);        // 将数字转为字符串，保留 n 位有效数字
num.toExponential(n);      // 将数字转为指数形式的字符串，保留 n 位有效数字
</code></pre>
</li>
<li><p><strong>Boolean（布尔）:</strong></p>
<p>JavaScript 中布尔对象没有明确的构造函数或方法，因为布尔值只有 <code>true</code> 和 <code>false</code>。</p>
</li>
<li><p><strong>Date（日期）:</strong></p>
<pre><code>javascriptvar today = new Date();

today.getDate();          // 获取当前日期的天
today.setDate(n);         // 设置当前日期的天
today.getDay();           // 获取当前星期的天
today.getFullYear();      // 获取当前年份
today.setFullYear(year);  // 设置当前年份
today.getHours();         // 获取当前小时
today.setHours(hours);    // 设置当前小时
// 更多方法...
</code></pre>
</li>
<li><p><strong>Math（数学）:</strong></p>
<pre><code>javascriptMath.PI;                  // 圆周率
Math.round(n);            // 四舍五入
Math.sqrt(n);             // 平方根
Math.ceil(n);             // 向上取整
Math.floor(n);            // 向下取整
Math.random();            // 生成 0 到 1 之间的随机数
// 更多方法...
</code></pre>
</li>
<li><p><strong>RegExp（正则表达式）:</strong></p>
<p>正则表达式对象没有明确的构造函数，通常通过字面量或 <code>RegExp</code> 构造函数创建。</p>
<pre><code>javascriptvar pattern = /pattern/;
var pattern = new RegExp(&quot;pattern&quot;);
</code></pre>
</li>

</ol>
<p>&nbsp;</p>
<h2 id='dom文档对象模型）'>DOM（文档对象模型）</h2>
<p>DOM（文档对象模型）是一种用于处理HTML和XML文档的编程接口。通过DOM，可以通过JavaScript脚本访问、修改文档的结构、样式和内容。以下是一些常见的DOM操作：</p>
<h3 id='获取元素'>获取元素</h3>
<ul>
<li><p><strong>document.getElementById():</strong> 通过元素的ID获取单个元素。</p>
<pre><code>javascript
var element = document.getElementById(&quot;myElement&quot;);
</code></pre>
</li>
<li><p><strong>document.getElementsByTagName():</strong> 通过标签名获取一组元素。</p>
<pre><code>javascript
var elements = document.getElementsByTagName(&quot;p&quot;);
</code></pre>
</li>
<li><p><strong>document.querySelector():</strong> 通过CSS选择器获取单个元素。</p>
<pre><code>javascript
var element = document.querySelector(&quot;.myClass&quot;);
</code></pre>
</li>
<li><p><strong>document.querySelectorAll():</strong> 通过CSS选择器获取一组元素。</p>
<pre><code>javascript
var elements = document.querySelectorAll(&quot;.myClass&quot;);
</code></pre>
</li>
<li><p><strong>document.getElementsByClassName():</strong> 通过类名获取一组元素。</p>
<pre><code>javascript
var elements = document.getElementsByClassName(&quot;myClass&quot;);
</code></pre>
</li>

</ul>
<h3 id='遍历traverse）'>遍历（Traverse）</h3>
<ul>
<li><strong>parentNode:</strong> 获取父节点。</li>
<li><strong>previousSibling:</strong> 获取前一个同级节点。</li>
<li><strong>nextSibling:</strong> 获取后一个同级节点。</li>
<li><strong>firstChild:</strong> 获取第一个子节点。</li>
<li><strong>lastChild:</strong> 获取最后一个子节点。</li>

</ul>
<h3 id='获取和更新'>获取和更新</h3>
<ul>
<li><strong>nodeValue:</strong> 获取或设置节点的值。</li>
<li><strong>textContent:</strong> 获取或设置节点的文本内容。</li>
<li><strong>innerHTML:</strong> 获取或设置节点的HTML内容。请谨慎使用，以防止XSS攻击。</li>

</ul>
<h3 id='添加和删除'>添加和删除</h3>
<ul>
<li><strong>createElement():</strong> 创建新元素。</li>
<li><strong>createTextNode():</strong> 创建新文本节点。</li>
<li><strong>appendChild():</strong> 将子节点添加到父节点。</li>
<li><strong>removeChild():</strong> 从父节点中删除子节点。</li>

</ul>
<h3 id='注入和xss'>注入和XSS</h3>
<ul>
<li>避免使用<code>document.write()</code>，因为它可能导致文档被覆盖。</li>
<li>确保从用户输入生成的内容被正确转义，以防止XSS攻击。</li>

</ul>
<h3 id='属性-1'>属性</h3>
<ul>
<li><strong>getAttribute():</strong> 获取元素的属性值。</li>
<li><strong>hasAttribute():</strong> 检查元素是否具有特定属性。</li>
<li><strong>setAttribute():</strong> 设置元素的属性值。</li>

</ul>
<p>这些DOM操作允许开发人员通过JavaScript与HTML文档进行交互，动态地更新和修改页面的内容和结构。</p>
<p>&nbsp;</p>
<h2 id='事件-1'>事件</h2>
<h3 id='机制'>机制</h3>
<p>在JavaScript中，事件机制是一种重要的编程范式，它使得网页可以对用户的操作或其他发生的事件做出响应。事件机制主要分为三个关键步骤：</p>
<ol start='' >
<li><strong>交互（Interaction）：</strong> 用户与网页进行交互，例如点击、滚动、键盘输入等。</li>
<li><strong>触发（Trigger）：</strong> 用户的交互导致特定的事件被触发，这可以是浏览器事件（如点击、加载），也可以是用户自定义的事件。</li>
<li><strong>相应（Response）：</strong> 在事件触发后，相应的JavaScript代码会执行，执行的内容可以包括修改页面内容、发送请求等。</li>

</ol>
<h3 id='事件-2'>事件</h3>
<p>在JavaScript中，事件分为不同的类型，主要有以下几类：</p>
<ol start='' >
<li><p><strong>W3C 事件：</strong> 这是由World Wide Web Consortium定义的标准事件模型，包括常见的事件类型如点击（click）、变化（change）等。</p>
<pre><code>javascript// 示例：监听按钮点击事件
document.getElementById(&#39;myButton&#39;).addEventListener(&#39;click&#39;, function() {
    console.log(&#39;按钮被点击了&#39;);
});
</code></pre>
</li>
<li><p><strong>HTML 事件：</strong> 这是一些与HTML元素相关的特定事件，如鼠标悬停（mouseover）、失去焦点（blur）等。</p>
<pre><code>javascript// 示例：监听输入框失去焦点事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;blur&#39;, function() {
    console.log(&#39;输入框失去焦点&#39;);
});
</code></pre>
</li>
<li><p><strong>BOM 事件：</strong> 浏览器对象模型（BOM）定义的事件，例如窗口加载（load）事件、窗口关闭（beforeunload）事件等。</p>
<pre><code>javascript// 示例：监听窗口加载事件
window.addEventListener(&#39;load&#39;, function() {
    console.log(&#39;页面加载完成&#39;);
});
</code></pre>
</li>

</ol>
<h4 id='ui事件'>UI事件</h4>
<h5 id='load-事件'>Load 事件</h5>
<p><strong>介绍：</strong> <code>load</code> 事件在页面或资源加载完成后触发，可以用于执行一些需要在页面完全加载后执行的操作。</p>
<pre><code>javascript// 示例：监听页面加载完成事件
window.addEventListener(&#39;load&#39;, function() {
    console.log(&#39;页面加载完成&#39;);
});
</code></pre>
<h5 id='unload-事件'>Unload 事件</h5>
<p><strong>介绍：</strong> <code>unload</code> 事件在用户离开页面时触发，常用于执行清理操作，例如释放资源或保存用户数据。</p>
<pre><code>javascript// 示例：监听页面卸载事件
window.addEventListener(&#39;unload&#39;, function() {
    console.log(&#39;页面即将卸载&#39;);
});
</code></pre>
<h6 id='error-事件'>Error 事件</h6>
<p><strong>介绍：</strong> <code>error</code> 事件用于捕捉页面或资源加载过程中的错误，帮助调试和记录错误信息。</p>
<pre><code>javascript// 示例：捕捉图片加载错误事件
document.getElementById(&#39;myImage&#39;).addEventListener(&#39;error&#39;, function() {
    console.log(&#39;图片加载失败&#39;);
});
</code></pre>
<h6 id='resize-事件'>Resize 事件</h6>
<p><strong>介绍：</strong> <code>resize</code> 事件在窗口或元素大小改变时触发，可用于响应页面布局变化。</p>
<pre><code>javascript// 示例：监听窗口大小改变事件
window.addEventListener(&#39;resize&#39;, function() {
    console.log(&#39;窗口大小已改变&#39;);
});
</code></pre>
<h6 id='scroll-事件'>Scroll 事件</h6>
<p><strong>介绍：</strong> <code>scroll</code> 事件在页面滚动时触发，可用于实现滚动时的交互效果。</p>
<pre><code>javascript// 示例：监听页面滚动事件
window.addEventListener(&#39;scroll&#39;, function() {
    console.log(&#39;页面正在滚动&#39;);
});
</code></pre>
<h4 id='键盘事件'>键盘事件</h4>
<h5 id='keydown-事件'>Keydown 事件</h5>
<p><strong>介绍：</strong> <code>keydown</code> 事件在用户按下键盘上的任意键时触发。</p>
<pre><code>javascript// 示例：监听键盘按下事件
document.addEventListener(&#39;keydown&#39;, function(event) {
    console.log(&#39;键盘按下：&#39;, event.key);
});
</code></pre>
<h5 id='keyup-事件'>Keyup 事件</h5>
<p><strong>介绍：</strong> <code>keyup</code> 事件在用户释放键盘上的键时触发。</p>
<pre><code>javascript// 示例：监听键盘释放事件
document.addEventListener(&#39;keyup&#39;, function(event) {
    console.log(&#39;键盘释放：&#39;, event.key);
});
</code></pre>
<h5 id='keypress-事件'>Keypress 事件</h5>
<p><strong>介绍：</strong> <code>keypress</code> 事件在用户按下并释放键盘上的键时触发。</p>
<pre><code>javascript// 示例：监听键盘按下并释放事件
document.addEventListener(&#39;keypress&#39;, function(event) {
    console.log(&#39;键盘按下并释放：&#39;, event.key);
});
</code></pre>
<h4 id='鼠标事件'>鼠标事件</h4>
<h5 id='click-事件'>Click 事件</h5>
<p><strong>介绍：</strong> <code>click</code> 事件在鼠标点击元素时触发，通常用于处理用户的点击行为。</p>
<pre><code>javascript// 示例：监听元素被点击事件
document.getElementById(&#39;myButton&#39;).addEventListener(&#39;click&#39;, function() {
    console.log(&#39;按钮被点击了&#39;);
});
</code></pre>
<h5 id='double-click-事件'>Double Click 事件</h5>
<p><strong>介绍：</strong> <code>dblclick</code> 事件在鼠标双击元素时触发，用于处理双击行为。</p>
<pre><code>javascript// 示例：监听元素被双击事件
document.getElementById(&#39;myElement&#39;).addEventListener(&#39;dblclick&#39;, function() {
    console.log(&#39;元素被双击了&#39;);
});
</code></pre>
<h5 id='mouseup-事件'>Mouseup 事件</h5>
<p><strong>介绍：</strong> <code>mouseup</code> 事件在鼠标按键释放时触发，适用于处理鼠标按键释放的情况。</p>
<pre><code>javascript// 示例：监听鼠标按键释放事件
document.addEventListener(&#39;mouseup&#39;, function() {
    console.log(&#39;鼠标按键释放了&#39;);
});
</code></pre>
<h5 id='mousedown-事件'>Mousedown 事件</h5>
<p><strong>介绍：</strong> <code>mousedown</code> 事件在鼠标按键按下时触发，通常用于处理鼠标按键按下的情况。</p>
<pre><code>javascript// 示例：监听鼠标按键按下事件
document.addEventListener(&#39;mousedown&#39;, function() {
    console.log(&#39;鼠标按键按下了&#39;);
});
</code></pre>
<h5 id='mouseover-事件'>Mouseover 事件</h5>
<p><strong>介绍：</strong> <code>mouseover</code> 事件在鼠标移入元素时触发，可用于实现鼠标移入时的效果。</p>
<pre><code>javascript// 示例：监听鼠标移入事件
document.getElementById(&#39;myElement&#39;).addEventListener(&#39;mouseover&#39;, function() {
    console.log(&#39;鼠标移入了元素&#39;);
});
</code></pre>
<h5 id='mouseout-事件'>Mouseout 事件</h5>
<p><strong>介绍：</strong> <code>mouseout</code> 事件在鼠标移出元素时触发，适用于实现鼠标移出时的效果。</p>
<pre><code>javascript// 示例：监听鼠标移出事件
document.getElementById(&#39;myElement&#39;).addEventListener(&#39;mouseout&#39;, function() {
    console.log(&#39;鼠标移出了元素&#39;);
});
</code></pre>
<h5 id='mousemove-事件'>Mousemove 事件</h5>
<p><strong>介绍：</strong> <code>mousemove</code> 事件在鼠标在元素内移动时触发，可用于实现鼠标跟随效果等。</p>
<pre><code>javascript// 示例：监听鼠标移动事件
document.addEventListener(&#39;mousemove&#39;, function(event) {
    console.log(&#39;鼠标移动了，坐标：&#39;, event.clientX, event.clientY);
});
</code></pre>
<h4 id='焦点事件'>焦点事件</h4>
<h5 id='focus-事件'>Focus 事件</h5>
<p><strong>介绍：</strong> <code>focus</code> 事件在元素获得焦点时触发，可用于处理用户聚焦输入框或其他元素的情况。</p>
<pre><code>javascript// 示例：监听输入框获得焦点事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;focus&#39;, function() {
    console.log(&#39;输入框获得焦点&#39;);
});
</code></pre>
<h5 id='blur-事件'>Blur 事件</h5>
<p><strong>介绍：</strong> <code>blur</code> 事件在元素失去焦点时触发，通常用于处理用户离开输入框或其他元素的情况。</p>
<pre><code>javascript// 示例：监听输入框失去焦点事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;blur&#39;, function() {
    console.log(&#39;输入框失去焦点&#39;);
});
</code></pre>
<h4 id='表单事件'>表单事件</h4>
<h5 id='input-事件'>Input 事件</h5>
<p><strong>介绍：</strong> <code>input</code> 事件在用户输入内容时触发，可用于实时响应用户输入。</p>
<pre><code>javascript// 示例：监听输入框内容变化事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;input&#39;, function() {
    console.log(&#39;输入框内容变化：&#39;, this.value);
});
</code></pre>
<h5 id='change-事件'>Change 事件</h5>
<p><strong>介绍：</strong> <code>change</code> 事件在表单元素的值发生变化，并失去焦点时触发，适用于处理输入框、下拉列表等的变化。</p>
<pre><code>javascript// 示例：监听下拉列表变化事件
document.getElementById(&#39;mySelect&#39;).addEventListener(&#39;change&#39;, function() {
    console.log(&#39;下拉列表值变化：&#39;, this.value);
});
</code></pre>
<h5 id='submit-事件'>Submit 事件</h5>
<p><strong>介绍：</strong> <code>submit</code> 事件在表单提交时触发，可用于执行一些前端验证或在提交前进行操作。</p>
<pre><code>javascript// 示例：监听表单提交事件
document.getElementById(&#39;myForm&#39;).addEventListener(&#39;submit&#39;, function(event) {
    event.preventDefault(); // 阻止默认提交行为
    console.log(&#39;表单提交了&#39;);
    // 进行其他操作或验证
});
</code></pre>
<h5 id='reset-事件'>Reset 事件</h5>
<p><strong>介绍：</strong> <code>reset</code> 事件在表单重置时触发，适用于在重置前执行一些操作。</p>
<pre><code>javascript// 示例：监听表单重置事件
document.getElementById(&#39;myForm&#39;).addEventListener(&#39;reset&#39;, function() {
    console.log(&#39;表单被重置了&#39;);
});
</code></pre>
<h5 id='cutcopypaste-事件'>Cut、Copy、Paste 事件</h5>
<p><strong>介绍：</strong> <code>cut</code>、<code>copy</code>、<code>paste</code> 事件分别在用户剪切、复制、粘贴时触发，可用于对剪贴板操作进行监听。</p>
<pre><code>javascript// 示例：监听剪切事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;cut&#39;, function() {
    console.log(&#39;文本被剪切了&#39;);
});

// 示例：监听复制事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;copy&#39;, function() {
    console.log(&#39;文本被复制了&#39;);
});

// 示例：监听粘贴事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;paste&#39;, function() {
    console.log(&#39;文本被粘贴了&#39;);
});
</code></pre>
<h5 id='select-事件'>Select 事件</h5>
<p><strong>介绍：</strong> <code>select</code> 事件在用户选择文本时触发，可用于监听用户选择文本的操作。</p>
<pre><code>javascript// 示例：监听文本选择事件
document.getElementById(&#39;myInput&#39;).addEventListener(&#39;select&#39;, function() {
    console.log(&#39;文本被选择了&#39;);
});
</code></pre>
<h4 id='文档事件'>文档事件</h4>
<h5 id='domsubtreemodified-事件'>DOMSubtreeModified 事件</h5>
<p><strong>介绍：</strong> <code>DOMSubtreeModified</code> 事件在文档的某个子树结构发生变化时触发，可以用于监听DOM结构的变化。</p>
<pre><code>javascript// 示例：监听DOM子树结构变化事件
document.addEventListener(&#39;DOMSubtreeModified&#39;, function() {
    console.log(&#39;DOM子树结构发生变化&#39;);
});
</code></pre>
<h5 id='domnodeinserted-事件'>DOMNodeInserted 事件</h5>
<p><strong>介绍：</strong> <code>DOMNodeInserted</code> 事件在一个节点被插入到文档中时触发。</p>
<pre><code>javascript// 示例：监听节点插入事件
document.addEventListener(&#39;DOMNodeInserted&#39;, function(event) {
    console.log(&#39;节点被插入到文档中：&#39;, event.target);
});
</code></pre>
<h5 id='domnoderemoved-事件'>DOMNodeRemoved 事件</h5>
<p><strong>介绍：</strong> <code>DOMNodeRemoved</code> 事件在一个节点从文档中移除时触发。</p>
<pre><code>javascript// 示例：监听节点移除事件
document.addEventListener(&#39;DOMNodeRemoved&#39;, function(event) {
    console.log(&#39;节点被从文档中移除：&#39;, event.target);
});
</code></pre>
<h5 id='domnodeinsertedintodocument-事件'>DOMNodeInsertedIntoDocument 事件</h5>
<p><strong>介绍：</strong> <code>DOMNodeInsertedIntoDocument</code> 事件在一个节点被插入到文档中时触发，与 <code>DOMNodeInserted</code> 类似。</p>
<pre><code>javascript// 示例：监听节点插入到文档事件
document.addEventListener(&#39;DOMNodeInsertedIntoDocument&#39;, function(event) {
    console.log(&#39;节点插入到文档中：&#39;, event.target);
});
</code></pre>
<h5 id='domnoderemovedfromdocument-事件'>DOMNodeRemovedFromDocument 事件</h5>
<p><strong>介绍：</strong> <code>DOMNodeRemovedFromDocument</code> 事件在一个节点从文档中移除时触发，与 <code>DOMNodeRemoved</code> 类似。</p>
<pre><code>javascript// 示例：监听节点从文档中移除事件
document.addEventListener(&#39;DOMNodeRemovedFromDocument&#39;, function(event) {
    console.log(&#39;节点从文档中移除：&#39;, event.target);
});
</code></pre>
<h4 id='html事件'>HTML事件</h4>
<h5 id='domcontentloaded-事件'>DOMContentLoaded 事件</h5>
<p><strong>介绍：</strong> <code>DOMContentLoaded</code> 事件在文档解析完成且所有DOM节点都已经构建完成时触发，而无需等待样式表、图像和子框架的完成加载。</p>
<pre><code>javascript// 示例：监听DOM内容加载完成事件
document.addEventListener(&#39;DOMContentLoaded&#39;, function() {
    console.log(&#39;DOM内容加载完成&#39;);
});
</code></pre>
<h5 id='hashchange-事件'>Hashchange 事件</h5>
<p><strong>介绍：</strong> <code>hashchange</code> 事件在文档的片段标识符（URL 中的#后的部分）发生变化时触发。</p>
<pre><code>javascript// 示例：监听URL的片段标识符变化事件
window.addEventListener(&#39;hashchange&#39;, function() {
    console.log(&#39;URL的片段标识符发生变化&#39;);
});
</code></pre>
<h5 id='beforeunload-事件'>beforeunload 事件</h5>
<p><strong>介绍：</strong> <code>beforeunload</code> 事件在窗口即将关闭或刷新时触发，常用于在用户离开页面之前进行确认操作。</p>
<pre><code>javascript// 示例：监听窗口即将关闭或刷新事件
window.addEventListener(&#39;beforeunload&#39;, function(event) {
    // 在此添加确认操作，例如弹出确认框
    event.returnValue = &#39;确定离开页面吗？&#39;;
});
</code></pre>
<h3 id='触发'>触发</h3>
<p>在JavaScript中，有多种方式可以触发事件，以下是一些常见的方法：</p>
<h4 id='html事件处理程序不推荐）'>HTML事件处理程序（不推荐）</h4>
<p>这是一种将事件直接绑定到HTML元素的方法，不推荐使用，因为它将HTML和JavaScript代码混合在一起，不利于维护和阅读。</p>
<pre><code>html
&lt;input type=&quot;text&quot; id=&quot;username&quot; onblur=&quot;checkUsername()&quot; /&gt;
</code></pre>
<h4 id='传统的dom事件处理'>传统的DOM事件处理</h4>
<p>使用传统的DOM事件处理方式，直接将函数赋值给事件处理属性。</p>
<pre><code>jsfunction checkUsername() {
    // 进行用户名长度检查的代码
}

var el = document.getElementById(&#39;username&#39;);
el.onblur = checkUsername;
</code></pre>
<h4 id='第2级dom监听器'>第2级DOM监听器</h4>
<p>使用第二级DOM事件监听器，通过 <code>addEventListener</code> 方法来绑定事件。</p>
<pre><code>jsfunction checkUsername() {
    // 进行用户名长度检查的代码
}

var el = document.getElementById(&#39;username&#39;);
el.addEventListener(&#39;blur&#39;, checkUsername, false);
</code></pre>
<p>在这些示例中，<code>checkUsername</code> 函数表示事件触发后执行的逻辑代码。你可以根据需要替换这个函数来执行不同的操作。触发逻辑代码可以包含任何你想要在事件发生时执行的操作，例如表单验证、动画效果等。</p>
<h5 id='传参问题'>传参问题</h5>
<p>匿名函数封装</p>
<pre><code class='language-javascript' lang='javascript'>el.addEventListener (&#39;blur&#39;, function() {
checkUsername (5);
}, false);
</code></pre>
<h3 id='事件流'>事件流</h3>
<p>事件流描述的是从页面中接收事件的顺序。当页面中嵌套了多个元素，并且这些元素之间发生事件时，事件的传播顺序可以通过事件流来理解。</p>
<h4 id='事件冒泡'>事件冒泡</h4>
<p>在事件冒泡中，事件首先从最内层的元素开始触发，然后逐级向外传播至最外层的元素。如果你使用 <code>addEventListener</code> 来注册事件，可以将第三个参数设置为 <code>false</code>，表示使用事件冒泡。</p>
<pre><code>js// 事件冒泡示例
var outer = document.getElementById(&#39;outer&#39;);
var inner = document.getElementById(&#39;inner&#39;);

outer.addEventListener(&#39;click&#39;, function() {
    console.log(&#39;外层元素被点击&#39;);
}, false);

inner.addEventListener(&#39;click&#39;, function() {
    console.log(&#39;内层元素被点击&#39;);
}, false);
</code></pre>
<p>在上面的例子中，如果你点击内层元素（id为<code>inner</code>），事件将首先在内层元素上触发，然后冒泡到外层元素（id为<code>outer</code>）。</p>
<h4 id='事件捕获'>事件捕获</h4>
<p>在事件捕获中，事件从最外层的元素开始触发，然后逐级向内传播至最内层的元素。如果你使用 <code>addEventListener</code> 来注册事件，可以将第三个参数设置为 <code>true</code>，表示使用事件捕获。</p>
<pre><code>js// 事件捕获示例
var outer = document.getElementById(&#39;outer&#39;);
var inner = document.getElementById(&#39;inner&#39;);

outer.addEventListener(&#39;click&#39;, function() {
    console.log(&#39;外层元素被点击&#39;);
}, true);

inner.addEventListener(&#39;click&#39;, function() {
    console.log(&#39;内层元素被点击&#39;);
}, true);
</code></pre>
<p>在上面的例子中，如果你点击内层元素（id为<code>inner</code>），事件将首先在外层元素（id为<code>outer</code>）上捕获，然后传播到内层元素。</p>
<h3 id='事件对象'>事件对象</h3>
<p>事件对象（Event Object）是在事件触发时由浏览器传递给事件处理程序的对象。这个对象包含了与事件相关的信息，可以通过它来获取事件的各种属性和方法。</p>
<p>在事件处理程序中，通常将事件对象作为参数传递给事件处理函数。不同的事件类型可能有不同的事件对象，但它们都共享一些通用的属性和方法。</p>
<p>以下是一些常见的事件对象属性和方法：</p>
<h5 id='通用属性和方法'>通用属性和方法</h5>
<ol start='' >
<li><p><strong><code>type</code>：</strong> 表示事件的类型，如 <code>&#39;click&#39;</code>、<code>&#39;mouseover&#39;</code> 等。</p>
<pre><code>javascriptfunction handleClick(event) {
    console.log(&#39;事件类型：&#39;, event.type);
}
</code></pre>
</li>
<li><p><strong><code>target</code>：</strong> 表示触发事件的元素。</p>
<pre><code>javascriptfunction handleClick(event) {
    console.log(&#39;触发事件的元素：&#39;, event.target);
}
</code></pre>
</li>
<li><p><strong><code>currentTarget</code>：</strong> 表示当前事件处理程序正在处理事件的元素。</p>
<pre><code>javascriptfunction handleClick(event) {
    console.log(&#39;当前处理事件的元素：&#39;, event.currentTarget);
}
</code></pre>
</li>

</ol>
<h5 id='鼠标事件属性'>鼠标事件属性</h5>
<p>对于鼠标事件，事件对象还包含一些特定的属性：</p>
<ol start='' >
<li><p><strong><code>clientX</code> 和 <code>clientY</code>：</strong> 表示鼠标事件发生时鼠标指针相对于浏览器窗口的水平和垂直坐标。</p>
<pre><code>javascriptfunction handleMouseMove(event) {
    console.log(&#39;鼠标坐标：&#39;, event.clientX, event.clientY);
}
</code></pre>
</li>
<li><p><strong><code>button</code>：</strong> 表示按下或释放的鼠标按键的编码。</p>
<pre><code>javascriptfunction handleMouseClick(event) {
    console.log(&#39;鼠标按键编码：&#39;, event.button);
}
</code></pre>
</li>

</ol>
<h5 id='键盘事件属性'>键盘事件属性</h5>
<p>对于键盘事件，事件对象还包含一些特定的属性：</p>
<ol start='' >
<li><p><strong><code>keyCode</code> 和 <code>key</code>：</strong> 表示按下或释放的键的键码和键名。</p>
<pre><code>javascriptfunction handleKeyPress(event) {
    console.log(&#39;按键编码：&#39;, event.keyCode);
    console.log(&#39;按键名称：&#39;, event.key);
}
</code></pre>
</li>

</ol>
<p>&nbsp;</p>
<h2 id='jquery'>jQuery</h2>
<p>jQuery 是一个流行的 JavaScript 库，旨在简化处理 HTML 文档、事件处理、动画和 AJAX 的任务。通过使用 jQuery，你可以更轻松地选择和操作 HTML 元素，以及执行各种常见的前端开发任务。</p>
<p>以下是 jQuery 常用的一些功能和用法：</p>
<h4 id='选择元素'>选择元素</h4>
<p>通过使用类似 CSS 选择器的语法，可以轻松地选择和操作 HTML 元素。</p>
<pre><code>javascript// 选择所有段落元素
$(&#39;p&#39;).text(&#39;Hello, jQuery!&#39;);

// 选择具有特定类的元素
$(&#39;.myClass&#39;).css(&#39;color&#39;, &#39;red&#39;);

// 选择具有特定 ID 的元素
$(&#39;#myId&#39;).hide();
</code></pre>
<h4 id='高效开发'>高效开发</h4>
<p>jQuery 提供了许多简化开发的方法，比如处理事件、执行动画等。</p>
<h4 id='事件处理'>事件处理</h4>
<pre><code>javascript// 监听点击事件
$(&#39;#myButton&#39;).click(function() {
    alert(&#39;按钮被点击了！&#39;);
});

// 监听表单提交事件
$(&#39;form&#39;).submit(function() {
    alert(&#39;表单已提交！&#39;);
});
</code></pre>
<p>动画</p>
<pre><code>javascript// 淡入淡出效果
$(&#39;#myElement&#39;).fadeOut(1000).fadeIn(1000);

// 移动元素
$(&#39;#myElement&#39;).animate({ left: &#39;200px&#39;, top: &#39;200px&#39; }, 1000);
</code></pre>
<h3 id='引入-jquery'>引入 jQuery</h3>
<p>在你的 HTML 文件中引入 jQuery 库，可以通过下载 jQuery 文件并在 HTML 中引用，或者使用 CDN（内容分发网络）：</p>
<pre><code>html&lt;!-- 通过 CDN 引入 jQuery --&gt;
&lt;script src=&quot;https://code.jquery.com/jquery-3.6.4.min.js&quot;&gt;&lt;/script&gt;
</code></pre>
<p><strong>除了类似与css选择器的方式，jQuery还提供筛选器</strong></p>
<h3 id='筛选器'>筛选器</h3>
<ul>
<li><code>:not(selector)</code>: 选择不匹配给定选择器的元素。</li>

</ul>
<pre><code>javascript// 选择不含有类名为 &#39;exclude&#39; 的所有段落元素
$(&#39;p:not(.exclude)&#39;).css(&#39;color&#39;, &#39;green&#39;);
</code></pre>
<ul>
<li><code>:first</code>: 选择匹配的元素集合中的第一个元素。</li>

</ul>
<pre><code>javascript// 选择第一个段落元素
$(&#39;p:first&#39;).css(&#39;font-weight&#39;, &#39;bold&#39;);
</code></pre>
<ul>
<li><code>:last</code>: 选择匹配的元素集合中的最后一个元素。</li>

</ul>
<pre><code>javascript// 选择最后一个段落元素
$(&#39;p:last&#39;).css(&#39;font-style&#39;, &#39;italic&#39;);
</code></pre>
<ul>
<li><code>:even</code>: 选择匹配的元素集合中的偶数位置的元素（从 0 开始计数）。</li>

</ul>
<pre><code>javascript// 选择偶数位置的段落元素
$(&#39;p:even&#39;).css(&#39;background-color&#39;, &#39;lightblue&#39;);
</code></pre>
<ul>
<li><code>:odd</code>: 选择匹配的元素集合中的奇数位置的元素（从 0 开始计数）。</li>

</ul>
<pre><code>javascript// 选择奇数位置的段落元素
$(&#39;p:odd&#39;).css(&#39;background-color&#39;, &#39;lightyellow&#39;);
</code></pre>
<ul>
<li><code>:eq(index)</code>: 选择匹配的元素集合中指定索引位置的元素（从 0 开始计数）。</li>

</ul>
<pre><code>javascript// 选择第二个段落元素
$(&#39;p:eq(1)&#39;).css(&#39;text-decoration&#39;, &#39;underline&#39;);
</code></pre>
<ul>
<li><code>:gt(index)</code>: 选择匹配的元素集合中索引大于指定索引的所有元素。</li>

</ul>
<pre><code>javascript// 选择索引大于 2 的段落元素
$(&#39;p:gt(2)&#39;).css(&#39;color&#39;, &#39;purple&#39;);
</code></pre>
<ul>
<li><code>:lt(index)</code>: 选择匹配的元素集合中索引小于指定索引的所有元素。</li>

</ul>
<pre><code>javascript// 选择索引小于 3 的段落元素
$(&#39;p:lt(3)&#39;).css(&#39;color&#39;, &#39;orange&#39;);
</code></pre>
<ul>
<li><code>:header</code>: 选择所有标题元素 (<code>h1</code>, <code>h2</code>, <code>h3</code>, ..., <code>h6</code>)。</li>

</ul>
<pre><code>javascript// 选择所有标题元素
$(&#39;:header&#39;).css(&#39;border-bottom&#39;, &#39;2px solid black&#39;);
</code></pre>
<ul>
<li><code>:animated</code>: 选择当前正在执行动画的所有元素。</li>

</ul>
<pre><code>javascript// 选择当前正在执行动画的元素并停止动画
$(&#39;:animated&#39;).stop();
</code></pre>
<ul>
<li><code>:focus</code>: 选择当前获得焦点的元素。</li>

</ul>
<pre><code>javascript// 选择当前获得焦点的输入框
$(&#39;:focus&#39;).css(&#39;border&#39;, &#39;2px solid red&#39;);
</code></pre>
<ul>
<li><code>:contains(&#39;text&#39;)</code>: 选择包含指定文本的元素。</li>

</ul>
<pre><code>javascript// 选择包含文本 &quot;Hello&quot; 的段落元素
$(&#39;p:contains(&quot;Hello&quot;)&#39;).css(&#39;background-color&#39;, &#39;yellow&#39;);
</code></pre>
<ul>
<li><code>:empty</code>: 选择没有子元素或者文本的空元素。</li>

</ul>
<pre><code>javascript// 选择没有内容的 div 元素
$(&#39;div:empty&#39;).text(&#39;This div was empty!&#39;).css(&#39;border&#39;, &#39;1px solid black&#39;);
</code></pre>
<ul>
<li><code>:parent</code>: 选择至少含有一个子元素或文本的父元素。</li>

</ul>
<pre><code>javascript// 选择含有子元素的 div 元素
$(&#39;div:parent&#39;).css(&#39;border&#39;, &#39;2px solid blue&#39;);
</code></pre>
<ul>
<li><code>:has(selector)</code>: 选择至少含有一个匹配给定选择器的子元素的元素。</li>

</ul>
<pre><code>javascript// 选择含有类名为 &#39;highlight&#39; 的子元素的段落元素
$(&#39;p:has(.highlight)&#39;).css(&#39;font-weight&#39;, &#39;bold&#39;);
</code></pre>
<ul>
<li><code>:hidden</code>: 选择所有隐藏的元素。</li>

</ul>
<pre><code>javascript// 选择所有隐藏的输入框
$(&#39;input:hidden&#39;).show();
</code></pre>
<ul>
<li><code>:visible</code>: 选择所有可见的元素。</li>

</ul>
<pre><code>javascript// 选择所有可见的按钮元素
$(&#39;button:visible&#39;).css(&#39;background-color&#39;, &#39;green&#39;);
</code></pre>
<ul>
<li><code>:nth-child(expr)</code>: 选择其父元素的第 N 个子元素，其中 N 由表达式 <code>expr</code> 决定。</li>

</ul>
<pre><code>javascript// 选择每个父元素的第三个子元素
$(&#39;p:nth-child(3)&#39;).css(&#39;color&#39;, &#39;red&#39;);
</code></pre>
<ul>
<li><code>:first-child</code>: 选择其父元素的第一个子元素。</li>

</ul>
<pre><code>javascript// 选择每个父元素的第一个子元素
$(&#39;p:first-child&#39;).css(&#39;text-decoration&#39;, &#39;underline&#39;);
</code></pre>
<ul>
<li><code>:last-child</code>: 选择其父元素的最后一个子元素。</li>

</ul>
<pre><code>javascript// 选择每个父元素的最后一个子元素
$(&#39;p:last-child&#39;).css(&#39;font-style&#39;, &#39;italic&#39;);
</code></pre>
<ul>
<li><code>:only-child</code>: 选择其父元素中唯一的子元素。</li>

</ul>
<pre><code>javascript// 选择每个父元素中唯一的子元素
$(&#39;p:only-child&#39;).css(&#39;font-size&#39;, &#39;24px&#39;);
</code></pre>
<ul>
<li><code>[attribute]</code>: 选择具有指定属性的元素。</li>

</ul>
<pre><code>javascript// 选择具有 &#39;data-toggle&#39; 属性的按钮元素
$(&#39;button[data-toggle]&#39;).css(&#39;background-color&#39;, &#39;yellow&#39;);
</code></pre>
<ul>
<li><code>[attribute=&#39;value&#39;]</code>: 选择具有指定属性和属性值的元素。</li>

</ul>
<pre><code>javascript// 选择 &#39;src&#39; 属性为 &#39;image.jpg&#39; 的图像元素
$(&#39;img[src=&quot;image.jpg&quot;]&#39;).css(&#39;border&#39;, &#39;2px solid red&#39;);
</code></pre>
<ul>
<li><code>[attribute != &#39;value&#39;]</code>: 选择具有指定属性但属性值不等于给定值的元素。</li>

</ul>
<pre><code>javascript// 选择 &#39;type&#39; 属性不为 &#39;checkbox&#39; 的输入框元素
$(&#39;input[type!=&quot;checkbox&quot;]&#39;).css(&#39;color&#39;, &#39;blue&#39;);
</code></pre>
<ul>
<li><code>[attribute^=&#39;value&#39;]</code>: 选择具有指定属性且属性值以给定值开头的元素。</li>

</ul>
<pre><code>javascript// 选择 &#39;href&#39; 属性以 &#39;https://&#39; 开头的链接元素
$(&#39;a[href^=&quot;https://&quot;]&#39;).css(&#39;color&#39;, &#39;green&#39;);
</code></pre>
<ul>
<li><code>[attribute$=&#39;value&#39;]</code>: 选择具有指定属性且属性值以给定值结尾的元素。</li>

</ul>
<pre><code>javascript// 选择 &#39;src&#39; 属性以 &#39;.png&#39; 结尾的图像元素
$(&#39;img[src$=&quot;.png&quot;]&#39;).css(&#39;border&#39;, &#39;2px solid blue&#39;);
</code></pre>
<ul>
<li><code>[attribute*=&#39;value&#39;]</code>: 选择具有指定属性且属性值包含给定值的元素。</li>

</ul>
<pre><code>javascript// 选择 &#39;alt&#39; 属性包含 &#39;cat&#39; 的图像元素
$(&#39;img[alt*=&quot;cat&quot;]&#39;).css(&#39;border&#39;, &#39;2px solid pink&#39;);
</code></pre>
<ul>
<li><code>[attribute|=&#39;value&#39;]</code>: 选择具有指定属性且属性值以给定值开头，后跟一个连字符 <code>-</code> 或是与给定值完全相同的元素。</li>

</ul>
<pre><code>javascript// 选择 &#39;lang&#39; 属性值为 &#39;en&#39; 或以 &#39;en-&#39; 开头的元素
$(&#39;[lang|=&quot;en&quot;]&#39;).css(&#39;font-family&#39;, &#39;Arial, sans-serif&#39;);
</code></pre>
<ul>
<li><code>[attribute ~= &#39;value&#39;]</code>: 选择具有指定属性且属性值包含多个空格分隔的词，其中一个词与给定值相同的元素。</li>

</ul>
<pre><code>javascript// 选择 &#39;class&#39; 属性包含 &#39;active&#39; 的元素
$(&#39;.active&#39;).css(&#39;background-color&#39;, &#39;yellow&#39;);
</code></pre>
<ul>
<li><code>[attribute] [attribute2]</code>: 选择同时具有两个属性的元素，可以用空格分隔多个属性选择器。</li>

</ul>
<pre><code>javascript// 选择同时具有 &#39;data-toggle&#39; 和 &#39;data-target&#39; 属性的按钮元素
$(&#39;button[data-toggle][data-target]&#39;).css(&#39;color&#39;, &#39;purple&#39;);
</code></pre>
<ul>
<li><code>:input</code>: 选择所有的输入元素，包括文本框、复选框、单选按钮、提交按钮等。</li>

</ul>
<pre><code>javascript// 选择所有输入元素并设置它们的边框颜色
$(&#39;:input&#39;).css(&#39;border&#39;, &#39;1px solid gray&#39;);
</code></pre>
<ul>
<li><code>:text</code>: 选择所有文本框元素。</li>

</ul>
<pre><code>javascript// 选择所有文本框并设置它们的背景颜色
$(&#39;:text&#39;).css(&#39;background-color&#39;, &#39;lightyellow&#39;);
</code></pre>
<ul>
<li><code>:password</code>: 选择所有密码框元素。</li>

</ul>
<pre><code>javascript// 选择所有密码框并设置它们的边框颜色
$(&#39;:password&#39;).css(&#39;border&#39;, &#39;2px solid darkred&#39;);
</code></pre>
<ul>
<li><code>:radio</code>: 选择所有单选按钮元素。</li>

</ul>
<pre><code>javascript// 选择所有单选按钮并设置它们的字体颜色
$(&#39;:radio&#39;).css(&#39;color&#39;, &#39;green&#39;);
</code></pre>
<ul>
<li><code>:checkbox</code>: 选择所有复选框元素。</li>

</ul>
<pre><code>javascript// 选择所有复选框并设置它们的边框颜色
$(&#39;:checkbox&#39;).css(&#39;border&#39;, &#39;2px solid purple&#39;);
</code></pre>
<ul>
<li><code>:submit</code>: 选择所有提交按钮元素。</li>

</ul>
<pre><code>javascript// 选择所有提交按钮并设置它们的背景颜色
$(&#39;:submit&#39;).css(&#39;background-color&#39;, &#39;lightblue&#39;);
</code></pre>
<ul>
<li><code>:image</code>: 选择所有图像按钮元素。</li>

</ul>
<pre><code>javascript// 选择所有图像按钮并设置它们的边框颜色
$(&#39;:image&#39;).css(&#39;border&#39;, &#39;1px solid orange&#39;);
</code></pre>
<ul>
<li><code>:reset</code>: 选择所有重置按钮元素。</li>

</ul>
<pre><code>javascript// 选择所有重置按钮并设置它们的字体样式
$(&#39;:reset&#39;).css(&#39;font-style&#39;, &#39;italic&#39;);
</code></pre>
<ul>
<li><code>:button</code>: 选择所有按钮元素，包括提交按钮、重置按钮以及普通按钮。</li>

</ul>
<pre><code>javascript// 选择所有按钮并设置它们的颜色
$(&#39;:button&#39;).css(&#39;color&#39;, &#39;darkblue&#39;);
</code></pre>
<ul>
<li><code>:file</code>: 选择所有文件上传元素。</li>

</ul>
<pre><code>javascript// 选择所有文件上传元素并设置它们的背景颜色
$(&#39;:file&#39;).css(&#39;background-color&#39;, &#39;lightgreen&#39;);
</code></pre>
<ul>
<li><code>:selected</code>: 选择所有被选中的元素，通常用于 <code>select</code> 元素。</li>

</ul>
<pre><code>javascript// 选择所有被选中的选项并设置它们的颜色
$(&#39;option:selected&#39;).css(&#39;color&#39;, &#39;red&#39;);
</code></pre>
<ul>
<li><code>:enabled</code>: 选择所有可用的元素。</li>

</ul>
<pre><code>javascript// 选择所有可用的输入元素并设置它们的边框颜色
$(&#39;:enabled&#39;).css(&#39;border&#39;, &#39;1px solid green&#39;);
</code></pre>
<ul>
<li><code>:disabled</code>: 选择所有禁用的元素。</li>

</ul>
<pre><code>javascript// 选择所有禁用的输入元素并设置它们的背景颜色
$(&#39;:disabled&#39;).css(&#39;background-color&#39;, &#39;lightgray&#39;);
</code></pre>
<ul>
<li><code>:checked</code>: 选择所有被选中的复选框或单选按钮元素。</li>

</ul>
<pre><code>javascript// 选择所有被选中的复选框并设置它们的边框颜色
$(&#39;:checked&#39;).css(&#39;border&#39;, &#39;2px solid pink&#39;);
</code></pre>
<h3 id='方法'>方法</h3>
<h4 id='元素选择'>元素选择</h4>
<h5 id='获取更改'>获取/更改</h5>
<ol start='' >
<li><p><strong>.html():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于获取或设置元素的 HTML 内容。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>html
&lt;div id=&quot;myDiv&quot;&gt;原始内容&lt;/div&gt;
</code></pre>
<pre><code class='language-javascript' lang='javascript'>javascript// 获取HTML内容
var content = $(&quot;#myDiv&quot;).html();
console.log(content); // 输出: 原始内容

// 设置HTML内容
$(&quot;#myDiv&quot;).html(&quot;新的内容&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.text():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于获取或设置元素的纯文本内容。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;p id=&quot;myPara&quot;&gt;原始文本&lt;/p&gt;
</code></pre>
<pre><code>javascript// 获取文本内容
var textContent = $(&quot;#myPara&quot;).text();
console.log(textContent); // 输出: 原始文本

// 设置文本内容
$(&quot;#myPara&quot;).text(&quot;新的文本&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.replaceWith():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用一个或多个元素替换匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;original&quot;&gt;原始内容&lt;/div&gt;
&lt;div class=&quot;replacement&quot;&gt;替换的内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 替换元素
$(&quot;.original&quot;).replaceWith(&quot;&lt;p&gt;新的内容&lt;/p&gt;&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.remove():</strong></p>
<ul>
<li><p><strong>描述：</strong> 从DOM中移除匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;toBeRemoved&quot;&gt;要移除的内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 移除元素
$(&quot;#toBeRemoved&quot;).remove();
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='元素'>元素</h5>
<ol start='' >
<li><p><strong>.before():</strong></p>
<ul>
<li><p><strong>描述：</strong> 在每个匹配的元素之前插入指定的内容。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;p class=&quot;target&quot;&gt;目标元素&lt;/p&gt;
</code></pre>
<pre><code>javascript// 在目标元素之前插入新内容
$(&quot;.target&quot;).before(&quot;&lt;div&gt;新内容&lt;/div&gt;&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.after():</strong></p>
<ul>
<li><p><strong>描述：</strong> 在每个匹配的元素之后插入指定的内容。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;p class=&quot;target&quot;&gt;目标元素&lt;/p&gt;
</code></pre>
<pre><code>javascript// 在目标元素之后插入新内容
$(&quot;.target&quot;).after(&quot;&lt;div&gt;新内容&lt;/div&gt;&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.prepend():</strong></p>
<ul>
<li><p><strong>描述：</strong> 在每个匹配的元素内部的开始位置插入指定的内容。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 在目标元素内部的开始位置插入新内容
$(&quot;.target&quot;).prepend(&quot;&lt;p&gt;新内容&lt;/p&gt;&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.append():</strong></p>
<ul>
<li><p><strong>描述：</strong> 在每个匹配的元素内部的末尾位置插入指定的内容。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 在目标元素内部的末尾位置插入新内容
$(&quot;.target&quot;).append(&quot;&lt;p&gt;新内容&lt;/p&gt;&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.remove():</strong></p>
<ul>
<li><p><strong>描述：</strong> 从DOM中移除匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;toBeRemoved&quot;&gt;要移除的内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 移除元素
$(&quot;.toBeRemoved&quot;).remove();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.clone():</strong></p>
<ul>
<li><p><strong>描述：</strong> 复制匹配的元素，包括所有的子元素和事件处理程序。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;original&quot;&gt;原始内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 复制元素
var clone = $(&quot;.original&quot;).clone();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.unwrap():</strong></p>
<ul>
<li><p><strong>描述：</strong> 从DOM中移除匹配元素的父元素，保留匹配元素本身。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;wrapper&quot;&gt;&lt;p&gt;被包裹的内容&lt;/p&gt;&lt;/div&gt;
</code></pre>
<pre><code>javascript// 移除包裹元素
$(&quot;p&quot;).unwrap();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.detach():</strong></p>
<ul>
<li><p><strong>描述：</strong> 从DOM中移除匹配的元素，但保留元素的数据和事件处理程序。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;toBeDetached&quot;&gt;要移除但保留数据的内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 移除元素但保留数据
$(&quot;.toBeDetached&quot;).detach();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.empty():</strong></p>
<ul>
<li><p><strong>描述：</strong> 从匹配的元素中移除所有子元素和内容。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;toBeEmptied&quot;&gt;&lt;p&gt;要清空的内容&lt;/p&gt;&lt;/div&gt;
</code></pre>
<pre><code>javascript// 清空元素内容
$(&quot;.toBeEmptied&quot;).empty();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.add():</strong></p>
<ul>
<li><p><strong>描述：</strong> 将元素添加到当前集合中。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;existing&quot;&gt;已有的元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 将新元素添加到已有元素集合中
var newElement = $(&quot;&lt;p&gt;新元素&lt;/p&gt;&quot;);
$(&quot;.existing&quot;).add(newElement);
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='属性-2'>属性</h5>
<ol start='' >
<li><p><strong>.attr():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于获取或设置匹配元素的属性。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;img id=&quot;myImage&quot; src=&quot;oldImage.jpg&quot; alt=&quot;Old Image&quot;&gt;
</code></pre>
<pre><code>javascript// 获取属性值
var srcValue = $(&quot;#myImage&quot;).attr(&quot;src&quot;);
console.log(srcValue); // 输出: oldImage.jpg

// 设置属性值
$(&quot;#myImage&quot;).attr(&quot;src&quot;, &quot;newImage.jpg&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.removeAttr():</strong></p>
<ul>
<li><p><strong>描述：</strong> 从匹配的元素中移除属性。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;input type=&quot;text&quot; id=&quot;myInput&quot; value=&quot;Some text&quot;&gt;
</code></pre>
<pre><code>javascript// 移除属性
$(&quot;#myInput&quot;).removeAttr(&quot;value&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.addClass():</strong></p>
<ul>
<li><p><strong>描述：</strong> 向匹配的元素添加一个或多个类。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot; class=&quot;oldClass&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 添加类
$(&quot;#myDiv&quot;).addClass(&quot;newClass&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.removeClass():</strong></p>
<ul>
<li><p><strong>描述：</strong> 从匹配的元素中移除一个或多个类。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot; class=&quot;oldClass newClass&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 移除类
$(&quot;#myDiv&quot;).removeClass(&quot;oldClass&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.css():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取或设置匹配元素的样式属性。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取样式属性值
var backgroundColor = $(&quot;#myDiv&quot;).css(&quot;background-color&quot;);
console.log(backgroundColor); // 输出: 样式属性值

// 设置样式属性值
$(&quot;#myDiv&quot;).css(&quot;color&quot;, &quot;blue&quot;);
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='表单'>表单</h5>
<ol start='' >
<li><p><strong>.val():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于获取或设置表单元素的值。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;input type=&quot;text&quot; id=&quot;myInput&quot; value=&quot;默认值&quot;&gt;
</code></pre>
<pre><code>javascript// 获取输入框的值
var inputValue = $(&quot;#myInput&quot;).val();
console.log(inputValue); // 输出: 默认值

// 设置输入框的值
$(&quot;#myInput&quot;).val(&quot;新的值&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.isNumeric():</strong></p>
<ul>
<li><p><strong>描述：</strong> 判断给定的值是否为数字。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 检查是否为数字
var numericValue = 42;
var isNumeric = $.isNumeric(numericValue);
console.log(isNumeric); // 输出: true

// 非数字情况
var stringValue = &quot;Not a number&quot;;
var isNotNumeric = $.isNumeric(stringValue);
console.log(isNotNumeric); // 输出: false
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='一般方法'>一般方法</h5>
<ol start='' >
<li><p><strong>.find():</strong></p>
<ul>
<li><p><strong>描述：</strong> 在匹配的元素中查找后代元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;container&quot;&gt;
  &lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 查找后代元素
var descendantElement = $(&quot;.container&quot;).find(&quot;.target&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.closest():</strong></p>
<ul>
<li><p><strong>描述：</strong> 在匹配的元素及其祖先元素中，找到最近的一个匹配选择器的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;container&quot;&gt;
  &lt;div class=&quot;inner&quot;&gt;
    &lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
  &lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 找到最近的匹配元素
var closestElement = $(&quot;.target&quot;).closest(&quot;.container&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.parent():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的父元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;parent&quot;&gt;
  &lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取父元素
var parentElement = $(&quot;.target&quot;).parent();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.parents():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的所有祖先元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;grandparent&quot;&gt;
  &lt;div class=&quot;parent&quot;&gt;
    &lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
  &lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取所有祖先元素
var ancestorElements = $(&quot;.target&quot;).parents();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.children():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的所有子元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;parent&quot;&gt;
  &lt;div class=&quot;child&quot;&gt;子元素&lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取所有子元素
var childElements = $(&quot;.parent&quot;).children();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.siblings():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的所有同级元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;sibling&quot;&gt;同级元素 1&lt;/div&gt;
&lt;div class=&quot;sibling&quot;&gt;同级元素 2&lt;/div&gt;
&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取所有同级元素
var siblingElements = $(&quot;.target&quot;).siblings();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.next():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的下一个同级元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
&lt;div class=&quot;next-sibling&quot;&gt;下一个同级元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取下一个同级元素
var nextElement = $(&quot;.target&quot;).next();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.nextAll():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素之后的所有同级元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
&lt;div class=&quot;next-sibling&quot;&gt;下一个同级元素 1&lt;/div&gt;
&lt;div class=&quot;next-sibling&quot;&gt;下一个同级元素 2&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取之后的所有同级元素
var nextAllElements = $(&quot;.target&quot;).nextAll();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.prev():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的上一个同级元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;prev-sibling&quot;&gt;上一个同级元素&lt;/div&gt;
&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取上一个同级元素
var prevElement = $(&quot;.target&quot;).prev();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.prevAll():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素之前的所有同级元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;prev-sibling&quot;&gt;上一个同级元素 2&lt;/div&gt;
&lt;div class=&quot;prev-sibling&quot;&gt;上一个同级元素 1&lt;/div&gt;
&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取之前的所有同级元素
var prevAllElements = $(&quot;.target&quot;).prevAll();
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='筛选器测试'>筛选器/测试</h5>
<ol start='' >
<li><p><strong>.filter():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于筛选匹配元素集合中满足指定条件的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;ul&gt;
  &lt;li&gt;Item 1&lt;/li&gt;
  &lt;li class=&quot;selected&quot;&gt;Item 2&lt;/li&gt;
  &lt;li&gt;Item 3&lt;/li&gt;
&lt;/ul&gt;
</code></pre>
<pre><code>javascript// 筛选出有特定类的元素
var selectedItems = $(&quot;li&quot;).filter(&quot;.selected&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.not():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于筛选匹配元素集合中不满足指定条件的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;ul&gt;
  &lt;li&gt;Item 1&lt;/li&gt;
  &lt;li class=&quot;exclude&quot;&gt;Item 2&lt;/li&gt;
  &lt;li&gt;Item 3&lt;/li&gt;
&lt;/ul&gt;
</code></pre>
<pre><code>javascript// 筛选出没有特定类的元素
var nonExcludedItems = $(&quot;li&quot;).not(&quot;.exclude&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.has():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于筛选匹配元素集合中包含特定后代的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div class=&quot;container&quot;&gt;
  &lt;p&gt;包含段落的元素&lt;/p&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 筛选出包含特定后代的元素
var containerWithParagraph = $(&quot;.container&quot;).has(&quot;p&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.is():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于检查匹配元素集合中的元素是否匹配指定的选择器、元素或 jQuery 对象。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div class=&quot;target&quot;&gt;目标元素&lt;/div&gt;
</code></pre>
<pre><code>javascript// 检查元素是否有特定类
var hasClass = $(&quot;.target&quot;).is(&quot;.target&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>:contains():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于选择包含指定文本的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;ul&gt;
  &lt;li&gt;Item 1&lt;/li&gt;
  &lt;li&gt;Item 2 contains text&lt;/li&gt;
  &lt;li&gt;Item 3&lt;/li&gt;
&lt;/ul&gt;
</code></pre>
<pre><code>javascript// 选择包含特定文本的元素
var containsText = $(&quot;li:contains(&#39;contains text&#39;)&quot;);
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='元素选中顺序索引）'>元素选中顺序（索引）</h5>
<ol start='' >
<li><p><strong>.eq():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于选择匹配元素集合中指定索引位置的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;ul&gt;
  &lt;li&gt;Item 1&lt;/li&gt;
  &lt;li&gt;Item 2&lt;/li&gt;
  &lt;li&gt;Item 3&lt;/li&gt;
&lt;/ul&gt;
</code></pre>
<pre><code>javascript// 选择第二个 li 元素（索引从 0 开始）
var secondItem = $(&quot;li&quot;).eq(1);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>:lt():</strong></p>
<ul>
<li><p><strong>描述：</strong> 选择匹配元素集合中所有位置小于给定索引的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;ul&gt;
  &lt;li&gt;Item 1&lt;/li&gt;
  &lt;li&gt;Item 2&lt;/li&gt;
  &lt;li&gt;Item 3&lt;/li&gt;
&lt;/ul&gt;
</code></pre>
<pre><code>javascript// 选择索引小于 2 的元素
var itemsBeforeIndex2 = $(&quot;li:lt(2)&quot;);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>:gt():</strong></p>
<ul>
<li><p><strong>描述：</strong> 选择匹配元素集合中所有位置大于给定索引的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;ul&gt;
  &lt;li&gt;Item 1&lt;/li&gt;
  &lt;li&gt;Item 2&lt;/li&gt;
  &lt;li&gt;Item 3&lt;/li&gt;
&lt;/ul&gt;
</code></pre>
<pre><code>javascript// 选择索引大于 0 的元素
var itemsAfterIndex0 = $(&quot;li:gt(0)&quot;);
</code></pre>
</li>

</ul>
</li>

</ol>
<h4 id='内容操作'>内容操作</h4>
<h5 id='尺寸'>尺寸</h5>
<ol start='' >
<li><p><strong>.height():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取或设置匹配元素的高度。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素的高度
var elementHeight = $(&quot;#myDiv&quot;).height();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.width():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取或设置匹配元素的宽度。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素的宽度
var elementWidth = $(&quot;#myDiv&quot;).width();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.innerHeight():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的高度，包括内边距但不包括边框和外边距。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素的内部高度
var innerHeight = $(&quot;#myDiv&quot;).innerHeight();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.innerWidth():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的宽度，包括内边距但不包括边框和外边距。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素的内部宽度
var innerWidth = $(&quot;#myDiv&quot;).innerWidth();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.outerHeight():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的高度，包括内边距和边框，但不包括外边距。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素的外部高度
var outerHeight = $(&quot;#myDiv&quot;).outerHeight();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.outerWidth():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素的宽度，包括内边距和边框，但不包括外边距。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素的外部宽度
var outerWidth = $(&quot;#myDiv&quot;).outerWidth();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>$(document).height():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取文档的高度。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 获取文档的高度
var documentHeight = $(document).height();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>$(document).width():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取文档的宽度。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 获取文档的宽度
var documentWidth = $(document).width();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>$(window).height():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取浏览器窗口的高度。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 获取窗口的高度
var windowHeight = $(window).height();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>$(window).width():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取浏览器窗口的宽度。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 获取窗口的宽度
var windowWidth = $(window).width();
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='位置'>位置</h5>
<ol start='' >
<li><p><strong>.offset():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素相对于文档的偏移。</p>
</li>
<li><p>例子：</p>
<pre><code>html
&lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素的文档偏移
var elementOffset = $(&quot;#myDiv&quot;).offset();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.position():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取匹配元素相对于其最近的定位祖先的偏移。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div id=&quot;parent&quot; style=&quot;position: relative;&quot;&gt;
  &lt;div id=&quot;myDiv&quot;&gt;内容&lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取元素相对于定位祖先的偏移
var elementPosition = $(&quot;#myDiv&quot;).position();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.scrollLeft():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取或设置匹配元素的水平滚动位置。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div id=&quot;scrollContainer&quot; style=&quot;overflow-x: scroll; white-space: nowrap;&quot;&gt;
  &lt;!-- 长内容 --&gt;
  &lt;div id=&quot;scrollContent&quot; style=&quot;width: 1000px;&quot;&gt;滚动内容&lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取水平滚动位置
var scrollLeftValue = $(&quot;#scrollContainer&quot;).scrollLeft();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.scrollTop():</strong></p>
<ul>
<li><p><strong>描述：</strong> 获取或设置匹配元素的垂直滚动位置。</p>
</li>
<li><p>例子：</p>
<pre><code>html&lt;div id=&quot;scrollContainer&quot; style=&quot;overflow-y: scroll; height: 200px;&quot;&gt;
  &lt;!-- 长内容 --&gt;
  &lt;div id=&quot;scrollContent&quot; style=&quot;height: 500px;&quot;&gt;滚动内容&lt;/div&gt;
&lt;/div&gt;
</code></pre>
<pre><code>javascript// 获取垂直滚动位置
var scrollTopValue = $(&quot;#scrollContainer&quot;).scrollTop();
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='特效和动画'>特效和动画</h5>
<h6 id='一般'>一般</h6>
<ol start='' >
<li><p><strong>.show():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于显示匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 显示元素
$(&quot;#myElement&quot;).show();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.hide():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于隐藏匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 隐藏元素
$(&quot;#myElement&quot;).hide();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.toggle():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于在显示和隐藏之间切换匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 切换元素的显示和隐藏状态
$(&quot;#myElement&quot;).toggle();
</code></pre>
</li>

</ul>
</li>

</ol>
<h6 id='淡出'>淡出</h6>
<ol start='' >
<li><p><strong>.fadeIn():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于淡入匹配的元素，逐渐使元素从不透明到透明。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 淡入元素
$(&quot;#myElement&quot;).fadeIn();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.fadeOut():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于淡出匹配的元素，逐渐使元素从透明到不透明。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 淡出元素
$(&quot;#myElement&quot;).fadeOut();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.fadeTo():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于将匹配元素的不透明度渐变到指定值。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 渐变元素的不透明度到0.5
$(&quot;#myElement&quot;).fadeTo(&quot;slow&quot;, 0.5);
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.fadeToggle():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于在淡入和淡出之间切换匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 切换元素的淡入和淡出状态
$(&quot;#myElement&quot;).fadeToggle();
</code></pre>
</li>

</ul>
</li>

</ol>
<h6 id='滑动'>滑动</h6>
<ol start='' >
<li><p><strong>.slideDown():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于滑动显示匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 滑动显示元素
$(&quot;#myElement&quot;).slideDown();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.slideUp():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于滑动隐藏匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 滑动隐藏元素
$(&quot;#myElement&quot;).slideUp();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.slideToggle():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于在滑动显示和滑动隐藏之间切换匹配的元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 切换元素的滑动显示和隐藏状态
$(&quot;#myElement&quot;).slideToggle();
</code></pre>
</li>

</ul>
</li>

</ol>
<h6 id='自定义'>自定义</h6>
<ol start='' >
<li><p><strong>.delay():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于设置动画开始之前的延迟。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 在动画开始之前延迟500毫秒
$(&quot;#myElement&quot;).delay(500).fadeIn();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.stop():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于停止当前正在运行的动画。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 停止当前元素的所有动画
$(&quot;#myElement&quot;).stop();
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.animate():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于创建自定义的动画效果。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript// 自定义动画
$(&quot;#myElement&quot;).animate({
  opacity: 0.5,
  width: &quot;50%&quot;
}, 1000);
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='文档'>文档</h5>
<ol start='' >
<li><p><strong>.ready():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于在文档加载完成后执行函数。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript
$(document).ready(function() {
  // 在文档加载完成后执行的代码
  console.log(&quot;文档加载完成！&quot;);
});
</code></pre>
<p>或简写为：</p>
<pre><code>javascript
$(function() {
  // 在文档加载完成后执行的代码
  console.log(&quot;文档加载完成！&quot;);
});
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.load():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于在元素加载完成后执行函数。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript
$(&quot;#myImage&quot;).load(function() {
  // 图片加载完成后执行的代码
  console.log(&quot;图片加载完成！&quot;);
});
</code></pre>
</li>

</ul>
</li>
<li><p><strong>.on():</strong></p>
<ul>
<li><p><strong>描述：</strong> 用于附加一个或多个事件处理程序到匹配元素。</p>
</li>
<li><p>例子：</p>
<pre><code>javascript
$(&quot;button&quot;).on(&quot;click&quot;, function() {
  // 按钮被点击时执行的代码
  console.log(&quot;按钮被点击！&quot;);
});
</code></pre>
</li>

</ul>
</li>

</ol>
<h5 id='遍历'>遍历</h5>
<p><code>.each()</code> 方法是 jQuery 提供的用于迭代处理集合中的元素的方法。它可以用于循环遍历数组、对象或 jQuery 对象中的元素，执行指定的函数。</p>
<p>以下是 <code>.each()</code> 方法的基本语法：</p>
<pre><code>$.each(collection, function(index, value) {
  // 处理每个元素的代码
});
</code></pre>
<h4 id='链式操作'>链式操作</h4>
<p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>$(&#39;li[id != &quot;one&quot;]&#39;) .hide ().delay (500) . fadeIn (1400) ;
</code></pre>
<p>## </p>
<h2 id='运行调试与错误处理'>运行调试与错误处理</h2>
<h3 id='执行顺序'>执行顺序</h3>
<h4 id='1-执行上下文'>1. 执行上下文</h4>
<ul>
<li><p><strong>内容介绍：</strong> 执行上下文是JavaScript代码执行的环境，包括变量、函数、this等信息。了解执行上下文的创建和执行过程对于理解代码执行流程至关重要。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>console.log(x); // 输出 undefined，但不报错
var x = 5;
</code></pre>
</li>

</ul>
<h4 id='2-堆栈'>2. 堆栈</h4>
<ul>
<li><p><strong>内容介绍：</strong> JavaScript使用调用栈（执行栈）来管理执行上下文。学习调用栈的概念有助于理解代码的执行顺序和调用关系。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>function foo() {
  console.log(&#39;foo&#39;);
}
function bar() {
  foo();
  console.log(&#39;bar&#39;);
}
bar();
</code></pre>
</li>

</ul>
<h4 id='3-准备阶段'>3. 准备阶段</h4>
<ul>
<li><p><strong>内容介绍：</strong> 在代码执行之前，JavaScript会进行准备工作，包括创建新的作用域、变量、函数和参数，以及确定this关键字的值。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>console.log(a); // 输出 undefined，不会报错
var a = 10;
</code></pre>
</li>

</ul>
<h4 id='4-执行阶段'>4. 执行阶段</h4>
<ul>
<li><p><strong>内容介绍：</strong> 一旦准备阶段完成，JavaScript开始执行代码，包括给变量赋值、引用函数来执行其代码以及执行语句。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>function multiply(x, y) {
  return x * y;
}
console.log(multiply(3, 4)); // 输出 12
</code></pre>
</li>

</ul>
<h3 id='变量作用域与性能'>变量作用域与性能</h3>
<h4 id='1-作用域链'>1. 作用域链</h4>
<ul>
<li><p><strong>内容介绍：</strong> JavaScript中的作用域链决定了变量的访问范围。深入了解作用域链有助于更好地组织和理解代码。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>function outer() {
  var x = 10;
  function inner() {
    console.log(x);
  }
  inner();
}
outer(); // 输出 10
</code></pre>
</li>

</ul>
<h4 id='2-闭包'>2. 闭包</h4>
<ul>
<li><p><strong>内容介绍：</strong> 闭包是指函数能够访问其词法作用域外部的变量。了解闭包的概念和使用场景对于优化代码结构和性能至关重要。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>function outer() {
  var x = 10;
  function inner() {
    console.log(x);
  }
  return inner;
}
var closureFn = outer();
closureFn(); // 输出 10
</code></pre>
</li>

</ul>
<h3 id='错误理解和处理'>错误理解和处理</h3>
<h4 id='1-异常机制'>1. 异常机制</h4>
<ul>
<li><p><strong>内容介绍：</strong> JavaScript中的异常是指运行时错误，可能导致代码无法正常执行。了解异常的机制有助于及时发现和处理错误。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>try {
  // 可能会引发异常的代码
} catch (error) {
  // 异常处理代码
  console.error(error.message);
} finally {
    // 最终执行的必须执行的代码
}
</code></pre>
</li>

</ul>
<h4 id='2-error-对象'>2. Error 对象</h4>
<ul>
<li><p><strong>内容介绍：</strong> Error 对象是 JavaScript 中用于表示错误的基础对象，它包含了多个属性用于描述错误的详细信息。</p>
</li>
<li><p>属性：</p>
<ul>
<li><strong>name：</strong> 错误名称</li>
<li><strong>message：</strong> 错误消息</li>
<li><strong>stack：</strong> 错误堆栈信息</li>

</ul>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>try {
  // 可能会引发异常的代码
} catch (error) {
  console.error(error.name); // 输出错误名称
  console.error(error.message); // 输出错误消息
  console.error(error.stack); // 输出错误堆栈信息
}
</code></pre>
</li>

</ul>
<h4 id='3-内置错误类型'>3. 内置错误类型</h4>
<ul>
<li><p><strong>内容介绍：</strong> JavaScript内置了多种错误类型，每种类型代表不同的错误情况，包括但不限于语法错误、引用错误、类型错误、范围错误、URI错误和评估错误。</p>
</li>
<li><p>内置错误类型：</p>
<ul>
<li><strong>Error：</strong> 通用错误对象</li>
<li><strong>SyntaxError：</strong> 语法错误</li>
<li><strong>ReferenceError：</strong> 引用错误</li>
<li><strong>TypeError：</strong> 类型错误</li>
<li><strong>RangeError：</strong> 范围错误</li>
<li><strong>URIError：</strong> URI错误</li>
<li><strong>EvalError：</strong> 评估错误</li>

</ul>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>try {
  // 可能会引发不同类型的错误的代码
} catch (error) {
  if (error instanceof SyntaxError) {
    console.error(&#39;语法错误&#39;);
  } else if (error instanceof ReferenceError) {
    console.error(&#39;引用错误&#39;);
  } else if (error instanceof TypeError) {
    console.error(&#39;类型错误&#39;);
  }
  // 其他错误类型的处理
}
</code></pre>
</li>

</ul>
<p>以上是关于错误理解和处理的基本大纲，通过了解异常机制、Error 对象和内置错误类型，你可以更有效地调试和处理JavaScript代码中的错误。</p>
<h3 id='调试'>调试</h3>
<h4 id='1-浏览器开发者工具和-console'>1. 浏览器开发者工具和 Console</h4>
<ul>
<li><p><strong>内容介绍：</strong> 浏览器开发者工具是调试JavaScript代码的重要工具之一，而Console是其中一个强大的组件，用于输出日志和进行交互性的调试。</p>
</li>
<li><p><strong>使用开发者工具：</strong> 打开浏览器开发者工具，切换到“Console”选项卡。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>// 使用不同的 console 方法输出日志
console.log(&#39;普通日志&#39;);
console.info(&#39;信息日志&#39;);
console.warn(&#39;警告日志&#39;);
console.error(&#39;错误日志&#39;);

// 使用 group 和 groupEnd 创建日志分组
console.group(&#39;日志分组&#39;);
console.log(&#39;分组内的日志&#39;);
console.groupEnd();

// 使用 table 打印表格形式的日志
const data = [{ name: &#39;John&#39;, age: 28 }, { name: &#39;Alice&#39;, age: 24 }];
console.table(data);

// 使用 assert 进行断言，如果条件不满足则输出错误信息
console.assert(1 === 2, &#39;断言失败，输出错误信息&#39;);
</code></pre>
</li>

</ul>
<h3 id='断点调试'>断点调试</h3>
<h4 id='1-断点'>1. 断点</h4>
<ul>
<li><p><strong>内容介绍：</strong> 断点是调试过程中的标记，它允许你在代码执行到特定位置时停止执行，方便你逐步检查代码。</p>
</li>
<li><p><strong>设置断点：</strong> 在开发者工具的“Sources”或“Debugger”选项卡中，找到要设置断点的代码行，点击行号左侧即可设置断点。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>function exampleFunction() {
  let x = 10;
  let y = 20;
  let result = x + y; // 设置断点
  console.log(result);
}
exampleFunction();
</code></pre>
</li>

</ul>
<h4 id='2-条件断点'>2. 条件断点</h4>
<ul>
<li><p><strong>内容介绍：</strong> 条件断点是一种特殊的断点，只有当指定条件满足时才会触发断点停止执行。</p>
</li>
<li><p><strong>设置条件断点：</strong> 在设置断点后，右键点击断点图标，选择“Edit Breakpoint”，然后可以输入条件表达式。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>let i = 0;
while (i &lt; 5) {
  console.log(i);
  i++;
}
</code></pre>
<p>在上述代码中，你可以设置一个条件断点，条件为 </p>
<pre><code class='language-javascript' lang='javascript'>i === 3
</code></pre>
<p>，这样当 i 等于 3 时会触发断点。</p>
</li>

</ul>
<h4 id='3-执行方式'>3. 执行方式</h4>
<ul>
<li><p><strong>内容介绍：</strong> 在调试过程中，你可以选择不同的执行方式，如单步执行、继续执行等，以便更灵活地控制调试流程。</p>
</li>
<li><p>执行方式：</p>
<ul>
<li><strong>单步执行（Step Over）：</strong> 逐行执行代码，不进入函数内部。</li>
<li><strong>进入函数（Step Into）：</strong> 如果当前行包含函数调用，进入函数内部执行。</li>
<li><strong>跳出函数（Step Out）：</strong> 执行完当前函数的剩余代码，并跳回到调用该函数的地方。</li>
<li><strong>继续执行（Resume）：</strong> 从当前位置继续执行，直到下一个断点或程序结束。</li>

</ul>
</li>
<li><p><strong>例子：</strong> 在调试器的“Debugger”选项卡中，你可以使用上述执行方式按钮来控制代码的逐步执行。</p>
</li>

</ul>
<h3 id='错误'>错误</h3>
<h3 id='错误处理'>错误处理</h3>
<h4 id='1-捕获错误'>1. 捕获错误</h4>
<ul>
<li><p><strong>内容介绍：</strong> 在JavaScript中，通过使用 <code>try</code>、<code>catch</code>、<code>finally</code> 关键字来捕获和处理错误，从而使程序能够更加健壮。</p>
</li>
<li><p>使用方式：</p>
<pre><code class='language-javascript' lang='javascript'>try {
  // 可能会引发异常的代码
} catch (error) {
  // 异常处理代码
  console.error(error.message);
} finally {
  // 最终执行的代码，无论是否发生异常都会执行
}
</code></pre>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>try {
  let result = x / y; // 如果y为0，将抛出除以零的错误
  console.log(result);
} catch (error) {
  console.error(&#39;发生错误：&#39; + error.message);
} finally {
  console.log(&#39;最终执行的代码&#39;);
}
</code></pre>
</li>

</ul>
<h4 id='2-抛出错误'>2. 抛出错误</h4>
<ul>
<li><p><strong>内容介绍：</strong> 在JavaScript中，通过 <code>throw</code> 关键字可以手动抛出一个错误，可以是内置的Error对象或自定义的错误对象。</p>
</li>
<li><p>使用方式：</p>
<pre><code class='language-javascript' lang='javascript'>
throw new Error(&#39;错误消息&#39;);
</code></pre>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>function divide(x, y) {
  if (y === 0) {
    throw new Error(&#39;除数不能为零&#39;);
  }
  return x / y;
}

try {
  let result = divide(10, 0);
  console.log(result);
} catch (error) {
  console.error(&#39;发生错误：&#39; + error.message);
}
</code></pre>
</li>

</ul>
<p>以上是关于错误的捕获和抛出的基本介绍。通过使用 <code>try</code>、<code>catch</code>、<code>finally</code> 可以有效地处理代码中可能出现的异常，而通过 <code>throw</code> 可以手动引发错误。这些机制有助于提高代码的健壮性和可维护性。</p>
<h4 id='常见错误'>常见错误</h4>
<ol start='' >
<li><p><strong>SyntaxError（语法错误）:</strong></p>
<ul>
<li><p><strong>描述：</strong> 代码中存在语法错误，违反了JavaScript语法规则。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>let x = 10;
if (x == 10 {  // 缺少右括号
  console.log(&#39;x 等于 10&#39;);
}
</code></pre>
</li>

</ul>
</li>
<li><p><strong>ReferenceError（引用错误）:</strong></p>
<ul>
<li><p><strong>描述：</strong> 尝试访问未声明的变量或未定义的对象属性。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>console.log(y); // y未定义
</code></pre>
</li>

</ul>
</li>
<li><p><strong>TypeError（类型错误）:</strong></p>
<ul>
<li><p><strong>描述：</strong> 变量或参数的类型不符合预期，无法执行特定的操作。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>let num = &#39;abc&#39;;
console.log(num.toUpperCase()); // num 不是字符串类型，无法调用 toUpperCase 方法
</code></pre>
</li>

</ul>
</li>
<li><p><strong>RangeError（范围错误）:</strong></p>
<ul>
<li><p><strong>描述：</strong> 数值超出有效范围，例如数组长度为负数。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>let arr = new Array(-1); // 数组长度不能为负数
</code></pre>
</li>

</ul>
</li>
<li><p><strong>URIError（URI错误）:</strong></p>
<ul>
<li><p><strong>描述：</strong> 与 URI 相关的函数（比如 decodeURIComponent）使用了无效的参数。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>decodeURIComponent(&#39;%&#39;); // 无效的 URI 编码
</code></pre>
</li>

</ul>
</li>
<li><p><strong>EvalError（评估错误）:</strong></p>
<ul>
<li><p><strong>描述：</strong> 在使用全局函数 eval() 时发生的错误（在现代 JavaScript 中，很少会遇到这个错误）。</p>
</li>
<li><p>例子：</p>
<pre><code class='language-javascript' lang='javascript'>
eval(&#39;alert(&quot;Hello, World!&quot;)&#39;); // 在严格模式下可能会抛出 EvalError
</code></pre>
</li>

</ul>
</li>

</ol>
<p>&nbsp;</p>
</body>
