---
title: node.js
date: 2023-11-21 13:12:12
cover: https://www.freecodecamp.org/news/content/images/2022/11/What-is.png
tags: 后端技术
categories:
- 学习
- 计算机
- 后端
---

<body>
<p>只把前端做后端
<!-- more --></p><h1 id='nodejs'>Node.js</h1>
<h2 id='1-nodejs基础概念'>1. <strong>Node.js基础概念</strong></h2>
<h3 id='11-了解nodejs是什么以及它的特点'>1.1 了解Node.js是什么以及它的特点</h3>
<ul>
<li><p><strong>Node.js是什么：</strong> Node.js是一个基于Chrome V8引擎的JavaScript运行时，用于构建高性能的网络应用程序。它使得能够使用JavaScript在服务器端运行代码，而不仅仅局限于浏览器中。</p>
</li>
<li><p><strong>Node.js的特点：</strong></p>
<ul>
<li><strong>非阻塞I/O：</strong> Node.js采用事件驱动、非阻塞I/O模型，使得能够处理大量并发请求，适用于实时性要求较高的应用。</li>
<li><strong>单线程：</strong> 尽管Node.js是单线程的，但它通过事件循环机制和异步操作实现了高并发，避免了传统多线程模型中的锁和线程切换的开销。</li>
<li><strong>跨平台：</strong> Node.js可在多个操作系统上运行，具有很好的跨平台性，适用于开发各种类型的应用。</li>
<li><strong>模块化：</strong> 使用CommonJS模块系统，能够将代码组织为模块，方便复用和维护。</li>

</ul>
</li>

</ul>
<h3 id='12-安装nodejs和npmnode包管理器）'>1.2 安装Node.js和npm（Node包管理器）</h3>
<ul>
<li><p><strong>安装Node.js：</strong></p>
<ol start='' >
<li>访问 <a href='https://nodejs.org/'>Node.js官方网站</a>。</li>
<li>下载适合你操作系统的Node.js安装包。</li>
<li>执行安装包，按照提示进行安装。</li>

</ol>
</li>
<li><p><strong>安装npm：</strong></p>
<p>npm是Node.js的包管理器，通常随Node.js一同安装。</p>
<ol start='' >
<li><p>打开终端（命令行工具）。</p>
</li>
<li><p>输入以下命令验证Node.js和npm的安装：</p>
<pre><code class='language-shell' lang='shell'>bashnode -v
npm -v
</code></pre>
<p>如果安装成功，将显示Node.js和npm的版本信息。</p>
</li>

</ol>
</li>

</ul>
<h3 id='13-创建和运行第一个nodejs应用程序'>1.3 创建和运行第一个Node.js应用程序</h3>
<ul>
<li><p><strong>创建第一个Node.js应用程序：</strong></p>
<ol start='' >
<li><p>创建一个新文件，例如<code>app.js</code>。</p>
</li>
<li><p>编写简单的Node.js代码：</p>
<pre><code class='language-javascript' lang='javascript'>javascript// app.js
console.log(&#39;Hello, Node.js!&#39;);
</code></pre>
</li>
<li><p>保存文件。</p>
</li>

</ol>
</li>
<li><p><strong>运行应用程序：</strong></p>
<ol start='' >
<li><p>打开终端。</p>
</li>
<li><p>切换到包含<code>app.js</code>的目录。</p>
</li>
<li><p>输入以下命令运行应用程序：</p>
<pre><code class='language-shell' lang='shell'>bash
node app.js
</code></pre>
</li>
<li><p>如果一切正常，终端将输出<code>Hello, Node.js!</code>，表示应用程序成功运行。</p>
</li>

</ol>
</li>

</ul>
<h2 id='2-nodejs核心模块'>2. <strong>Node.js核心模块</strong></h2>
<h3 id='21-模块系统requireexports）'>2.1 模块系统（require、exports）</h3>
<h4 id='211-模块概念'>2.1.1 模块概念</h4>
<p>在Node.js中，每个文件都被视为一个模块，模块系统允许你将代码组织成可重用的部分。这些模块可以包含变量、函数、对象等，而且可以通过<code>require</code>和<code>exports</code>来实现模块之间的交互。</p>
<h4 id='212-require'>2.1.2 require</h4>
<ul>
<li><p><strong>概念：</strong> <code>require</code>是Node.js中用于加载模块的关键字。通过<code>require</code>，你可以在一个模块中引入另一个模块的功能。</p>
</li>
<li><p><strong>使用示例：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascript// 模块A：a.js
const message = &quot;Hello from Module A&quot;;
module.exports = message;
</code></pre>
<pre><code class='language-javascript' lang='javascript'>javascript// 模块B：b.js
const messageFromModuleA = require(&#39;./a.js&#39;);
console.log(messageFromModuleA);  // 输出: Hello from Module A
</code></pre>
</li>

</ul>
<h4 id='213-exports'>2.1.3 exports</h4>
<ul>
<li><p><strong>概念：</strong> <code>exports</code> 是模块系统用于导出模块中的变量、函数或对象的对象。</p>
</li>
<li><p><strong>使用示例：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascript// 模块C：c.js
const add = (a, b) =&gt; a + b;
const subtract = (a, b) =&gt; a - b;

exports.add = add;
exports.subtract = subtract;
</code></pre>
<pre><code class='language-javascript' lang='javascript'>javascript// 模块D：d.js
const mathOperations = require(&#39;./c.js&#39;);

console.log(mathOperations.add(5, 3));       // 输出: 8
console.log(mathOperations.subtract(10, 4));  // 输出: 6
</code></pre>
</li>

</ul>
<h4 id='214-moduleexports-vs-exports'>2.1.4 module.exports vs exports</h4>
<ul>
<li><p><strong>概念：</strong> <code>module.exports</code> 和 <code>exports</code> 都用于导出模块中的内容，但它们有一些差异。</p>
</li>
<li><p><strong>使用示例：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascript// 模块E：e.js
const greetings = {
  sayHello: () =&gt; console.log(&#39;Hello&#39;),
  sayGoodbye: () =&gt; console.log(&#39;Goodbye&#39;)
};

// 使用 module.exports
module.exports = greetings;
</code></pre>
<pre><code class='language-javascript' lang='javascript'>javascript// 模块F：f.js
const greetings = require(&#39;./e.js&#39;);

greetings.sayHello();    // 输出: Hello
greetings.sayGoodbye();  // 输出: Goodbye
</code></pre>
<p>在这个例子中，如果使用 <code>exports</code> 而不是 <code>module.exports</code>，它将不会正常工作，因为<code>exports</code>只是<code>module.exports</code>的一个引用，当你为<code>exports</code>分配一个新值时，它将不再指向<code>module.exports</code>。</p>
</li>

</ul>
<h3 id='22-文件系统模块fs）'>2.2 文件系统模块（fs）</h3>
<h4 id='221-文件系统模块概述'>2.2.1 文件系统模块概述</h4>
<p>在Node.js中，文件系统模块 (<code>fs</code>) 允许你与文件系统进行交互，执行文件读取、写入、删除等操作。该模块提供了异步和同步的文件操作方法，使得能够有效地处理文件相关的任务。</p>
<h4 id='222-常用文件系统操作'>2.2.2 常用文件系统操作</h4>
<ul>
<li><p><strong>异步读取文件：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascript
const fs = require(&#39;fs&#39;);

fs.readFile(&#39;example.txt&#39;, &#39;utf8&#39;, (err, data) =&gt; {
  if (err) throw err;
  console.log(data);
});
</code></pre>
</li>
<li><p><strong>异步写入文件：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascript
const fs = require(&#39;fs&#39;);

fs.writeFile(&#39;example.txt&#39;, &#39;Hello, Node.js!&#39;, &#39;utf8&#39;, (err) =&gt; {
  if (err) throw err;
  console.log(&#39;File has been written.&#39;);
});
</code></pre>
</li>
<li><p><strong>同步读取文件：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascript
const fs = require(&#39;fs&#39;);

try {
  const data = fs.readFileSync(&#39;example.txt&#39;, &#39;utf8&#39;);
  console.log(data);
} catch (err) {
  console.error(err);
}
</code></pre>
</li>
<li><p><strong>同步写入文件：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascriptconst fs = require(&#39;fs&#39;);

try {
  fs.writeFileSync(&#39;example.txt&#39;, &#39;Hello, Node.js!&#39;, &#39;utf8&#39;);
  console.log(&#39;File has been written.&#39;);
} catch (err) {
  console.error(err);
}
</code></pre>
</li>
<li><p><strong>检查文件是否存在：</strong></p>
<pre><code class='language-javascript' lang='javascript'>javascriptconst fs = require(&#39;fs&#39;);

fs.access(&#39;example.txt&#39;, fs.constants.F_OK, (err) =&gt; {
  if (err) {
    console.error(&#39;File does not exist.&#39;);
  } else {
    console.log(&#39;File exists.&#39;);
  }
});
</code></pre>
</li>

</ul>
<h4 id='223-文件系统模块注意事项'>2.2.3 文件系统模块注意事项</h4>
<ul>
<li>在进行文件操作时，使用异步操作可以提高程序的性能，避免阻塞。</li>
<li>了解回调函数的使用，以处理异步文件操作的结果。</li>
<li>文件路径可以是相对路径或绝对路径，相对路径是相对于执行 Node.js 进程的当前工作目录而言的。</li>

</ul>
<p>文件系统模块 (<code>fs</code>) 提供了丰富的功能，可用于处理文件的读写、删除、创建等操作。在实际应用中，根据需求选择适当的文件操作方式，并使用错误处理机制确保程序的稳定性。</p>
<h3 id='23-http模块创建简单的http服务器）'>2.3 HTTP模块（创建简单的HTTP服务器）</h3>
<p>Node.js提供了HTTP模块，允许你创建和处理HTTP服务器。下面是一个简单的例子，演示如何使用HTTP模块创建一个基本的HTTP服务器。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
// 引入HTTP模块
const http = require(&#39;http&#39;);

// 创建HTTP服务器并定义请求处理函数
const server = http.createServer((req, res) =&gt; {
  // 设置响应头
  res.writeHead(200, { &#39;Content-Type&#39;: &#39;text/plain&#39; });

  // 发送响应数据
  res.end(&#39;Hello, Node.js HTTP Server!\n&#39;);
});

// 指定服务器监听的端口号和主机地址
const PORT = 3000;
const HOST = &#39;localhost&#39;;

// 启动服务器并监听指定端口
server.listen(PORT, HOST, () =&gt; {
  console.log(`Server running at http://${HOST}:${PORT}/`);
});
</code></pre>
<h4 id='解释'>解释：</h4>
<ol start='' >
<li><strong>引入HTTP模块：</strong> 使用<code>require</code>语句引入Node.js的HTTP模块。</li>
<li><strong>创建HTTP服务器：</strong> 使用<code>createServer</code>方法创建一个HTTP服务器，该方法接受一个回调函数，这个回调函数会在每次有HTTP请求时被调用。</li>
<li><strong>请求处理函数：</strong> 请求处理函数接收<code>req</code>（请求）和<code>res</code>（响应）两个参数。在这个例子中，简单设置响应头并返回一条Hello消息。</li>
<li><strong>指定服务器监听的端口和主机：</strong> 使用<code>listen</code>方法指定服务器监听的端口号和主机地址。</li>
<li><strong>启动服务器：</strong> 服务器通过<code>listen</code>方法启动，并在控制台输出启动信息。</li>
<li><strong>访问服务器：</strong> 在浏览器中访问 <code>http://localhost:3000/</code>，将会看到&quot;Hello, Node.js HTTP Server!&quot;的响应。</li>

</ol>
<h3 id='24-事件模块events）'>2.4 事件模块（events）</h3>
<p>Node.js的事件模块是建立在观察者模式的基础上的，允许对象触发和监听事件。核心模块 <code>events</code> 提供了 <code>EventEmitter</code> 类，用于实现事件的注册、触发和处理。</p>
<h4 id='241-基本概念'>2.4.1 基本概念</h4>
<ul>
<li><p><strong>引入events模块：</strong> 使用<code>require</code>语句引入Node.js的events模块。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
const EventEmitter = require(&#39;events&#39;);
</code></pre>
</li>
<li><p><strong>创建事件发射器：</strong> 实例化<code>EventEmitter</code>类以创建事件发射器。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
const myEmitter = new EventEmitter();
</code></pre>
</li>
<li><p><strong>注册事件监听器：</strong> 使用<code>on</code>方法注册事件监听器，监听器是一个回调函数。</p>
<pre><code class='language-javascript' lang='javascript'>javascriptmyEmitter.on(&#39;eventName&#39;, () =&gt; {
  console.log(&#39;Event triggered!&#39;);
});
</code></pre>
</li>
<li><p><strong>触发事件：</strong> 使用<code>emit</code>方法触发事件。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
myEmitter.emit(&#39;eventName&#39;);
</code></pre>
</li>

</ul>
<h4 id='242-示例'>2.4.2 示例</h4>
<pre><code class='language-javascript' lang='javascript'>javascript
const EventEmitter = require(&#39;events&#39;);

// 创建事件发射器实例
const myEmitter = new EventEmitter();

// 注册事件监听器
myEmitter.on(&#39;greet&#39;, (name) =&gt; {
  console.log(`Hello, ${name}!`);
});

// 触发事件，并传递参数
myEmitter.emit(&#39;greet&#39;, &#39;John&#39;);
</code></pre>
<p>在这个例子中，我们创建了一个事件发射器实例 <code>myEmitter</code>，并注册了一个名为 <code>greet</code> 的事件监听器。当事件被触发时，监听器将输出类似 &quot;Hello, John!&quot; 的消息。</p>
<h4 id='243-处理一次性事件'>2.4.3 处理一次性事件</h4>
<pre><code class='language-javascript' lang='javascript'>javascript
const EventEmitter = require(&#39;events&#39;);

// 创建事件发射器实例
const myEmitter = new EventEmitter();

// 注册一次性事件监听器
myEmitter.once(&#39;greetOnce&#39;, () =&gt; {
  console.log(&#39;Hello, one time!&#39;);
});

// 触发事件
myEmitter.emit(&#39;greetOnce&#39;);  // 输出: Hello, one time!
myEmitter.emit(&#39;greetOnce&#39;);  // 该事件监听器只会执行一次，这次不会输出任何内容
</code></pre>
<p>通过使用 <code>once</code> 方法，你可以注册一个一次性的事件监听器，它只会在第一次触发事件时执行。</p>
<p>事件模块在Node.js中广泛用于实现异步操作和处理回调函数，特别是在处理I/O操作和构建可扩展的应用程序时非常有用。</p>
<h3 id='25-全局对象global）'>2.5 全局对象（global）</h3>
<p>在Node.js中，全局对象 <code>global</code> 是全局作用域的一部分，允许在任何地方访问。与浏览器环境中的 <code>window</code> 不同，Node.js中的全局对象是 <code>global</code>。</p>
<h4 id='251-使用全局对象'>2.5.1 使用全局对象</h4>
<p>在Node.js中，不需要使用 <code>global</code> 关键字即可访问全局对象。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
// 全局变量
global.myVariable = &#39;This is a global variable&#39;;
console.log(myVariable);  // 输出: This is a global variable
</code></pre>
<h4 id='252-全局对象的属性和方法'>2.5.2 全局对象的属性和方法</h4>
<p>全局对象 <code>global</code> 包含一些常用的属性和方法，例如：</p>
<ul>
<li><p><strong><code>console</code>：</strong> 用于在控制台输出信息。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
global.console.log(&#39;Hello, global!&#39;);
</code></pre>
</li>
<li><p><strong><code>setTimeout</code> 和 <code>clearTimeout</code>：</strong> 用于设置和清除定时器。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
const myTimer = setTimeout(() =&gt; {
  console.log(&#39;Timer expired!&#39;);
}, 1000);

// 清除定时器
clearTimeout(myTimer);
</code></pre>
</li>
<li><p><strong><code>setInterval</code> 和 <code>clearInterval</code>：</strong> 用于设置和清除周期性定时器。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
const myInterval = setInterval(() =&gt; {
  console.log(&#39;Interval triggered!&#39;);
}, 1000);

// 清除周期性定时器
clearInterval(myInterval);
</code></pre>
</li>
<li><p><strong><code>__dirname</code> 和 <code>__filename</code>：</strong> 分别返回当前脚本所在目录和文件的绝对路径。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
console.log(__dirname);   // 输出: 当前脚本所在目录的绝对路径
console.log(__filename);  // 输出: 当前脚本的绝对路径
</code></pre>
</li>

</ul>
<p>全局对象的其他属性和方法可在Node.js官方文档中找到。</p>
<h4 id='253-注意事项'>2.5.3 注意事项</h4>
<ul>
<li>全局变量和对象的滥用可能导致命名冲突和不可预测的行为。在实际应用中，尽量避免过度使用全局对象。</li>
<li>在模块中声明的变量不会成为全局变量，除非显式地使用 <code>global</code> 关键字。</li>

</ul>
<p>全局对象 <code>global</code> 在Node.js中有其用途，但应谨慎使用，以避免潜在的命名冲突和代码维护问题。</p>
<h2 id='3-异步编程'>3. <strong>异步编程</strong></h2>
<h3 id='31-了解javascript中的异步编程概念'>3.1 了解JavaScript中的异步编程概念</h3>
<p>在JavaScript中，异步编程是一种编程范式，用于处理需要等待的操作，例如网络请求、文件读取、定时器等。异步编程允许程序在等待操作完成的同时继续执行其他任务，而不必阻塞整个程序。</p>
<h4 id='311-javascript中的同步和异步'>3.1.1 JavaScript中的同步和异步</h4>
<ul>
<li><p><strong>同步（Synchronous）：</strong> 操作按照顺序逐一执行，每个操作完成后才进行下一个操作。这可能导致程序在等待某个操作完成时停滞。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
console.log(&#39;Start&#39;);
// 同步操作
console.log(&#39;Middle&#39;);
// 同步操作
console.log(&#39;End&#39;);
</code></pre>
</li>
<li><p><strong>异步（Asynchronous）：</strong> 操作不按照顺序执行，而是通过回调函数、Promise、async/await等机制来处理。程序在等待异步操作完成时可以继续执行其他任务。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
console.log(&#39;Start&#39;);
// 异步操作
setTimeout(() =&gt; {
  console.log(&#39;Middle&#39;);
}, 1000);
console.log(&#39;End&#39;);
</code></pre>
</li>

</ul>
<h4 id='312-异步编程的解决方案'>3.1.2 异步编程的解决方案</h4>
<ol start='' >
<li><p><strong>回调函数（Callback）：</strong> 通过将函数作为参数传递给其他函数，以便在异步操作完成时调用。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
function fetchData(callback) {
  // 模拟异步操作
  setTimeout(() =&gt; {
    const data = &#39;Async data&#39;;
    callback(data);
  }, 1000);
}

fetchData((result) =&gt; {
  console.log(result);
});
</code></pre>
</li>
<li><p><strong>Promise：</strong> 提供了更清晰的异步编程方式，通过链式调用 <code>.then()</code> 和 <code>.catch()</code> 处理异步操作的结果和错误。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
function fetchData() {
  return new Promise((resolve, reject) =&gt; {
    // 模拟异步操作
    setTimeout(() =&gt; {
      const data = &#39;Async data&#39;;
      resolve(data);
    }, 1000);
  });
}

fetchData()
  .then((result) =&gt; {
    console.log(result);
  })
  .catch((error) =&gt; {
    console.error(error);
  });
</code></pre>
</li>
<li><p><strong>async/await：</strong> 基于Promise的语法糖，提供了更直观的方式编写异步代码。</p>
<pre><code class='language-javascript' lang='javascript'>javascript
async function fetchData() {
  return new Promise((resolve, reject) =&gt; {
    // 模拟异步操作
    setTimeout(() =&gt; {
      const data = &#39;Async data&#39;;
      resolve(data);
    }, 1000);
  });
}

async function getData() {
  try {
    const result = await fetchData();
    console.log(result);
  } catch (error) {
    console.error(error);
  }
}

getData();
</code></pre>
</li>

</ol>
<p>异步编程在处理JavaScript中的异步操作时至关重要，它使得程序能够更高效地利用等待时间，提高了程序的性能和响应性。在现代JavaScript中，Promise和async/await是处理异步编程的主要工具。</p>
<h3 id='32-回调函数和事件驱动编程'>3.2 回调函数和事件驱动编程</h3>
<h4 id='321-回调函数callback）'>3.2.1 回调函数（Callback）</h4>
<p>在JavaScript中，回调函数是一种常见的异步编程方式。回调函数是在一个函数执行完毕后执行的函数，用于处理异步操作的结果。</p>
<pre><code class='language-javascript' lang='javascript'>function fetchData(callback) {
  // 模拟异步操作
  setTimeout(() =&gt; {
    const data = &#39;Async data&#39;;
    callback(null, data); // 通常第一个参数是错误对象，第二个参数是操作结果
  }, 1000);
}

// 使用回调函数
fetchData((err, result) =&gt; {
  if (err) {
    console.error(err);
  } else {
    console.log(result);
  }
});
</code></pre>
<p>在上面的例子中，<code>fetchData</code> 函数接受一个回调函数作为参数，在异步操作完成后调用该回调函数。回调函数的第一个参数通常用于传递错误信息，第二个参数用于传递操作结果。</p>
<h4 id='322-事件驱动编程'>3.2.2 事件驱动编程</h4>
<p>事件驱动编程是一种异步编程的范式，它基于事件和事件监听器的概念。Node.js中的核心模块 <code>events</code> 提供了 <code>EventEmitter</code> 类，用于实现事件的注册、触发和处理。</p>
<pre><code class='language-javascript' lang='javascript'>const EventEmitter = require(&#39;events&#39;);

// 创建事件发射器实例
const myEmitter = new EventEmitter();

// 注册事件监听器
myEmitter.on(&#39;greet&#39;, (name) =&gt; {
  console.log(`Hello, ${name}!`);
});

// 触发事件，并传递参数
myEmitter.emit(&#39;greet&#39;, &#39;John&#39;);
</code></pre>
<p>在这个例子中，我们创建了一个事件发射器实例 <code>myEmitter</code>，注册了一个名为 <code>greet</code> 的事件监听器。当事件被触发时，监听器将输出类似 &quot;Hello, John!&quot; 的消息。</p>
<p>事件驱动编程适用于需要响应外部事件、处理用户输入等异步场景。它提供了一种松耦合的方式来组织代码，使得代码更加可维护和可扩展。</p>
<h4 id='323-区别与应用场景'>3.2.3 区别与应用场景</h4>
<ul>
<li><p><strong>回调函数：</strong></p>
<ul>
<li>使用场景：适用于处理一次性的异步操作，如读取文件、发送HTTP请求等。</li>
<li>优点：简单直观，易于理解。</li>
<li>缺点：容易陷入回调地狱（Callback Hell），不方便处理多个异步操作的协同工作。</li>

</ul>
</li>
<li><p><strong>事件驱动编程：</strong></p>
<ul>
<li>使用场景：适用于需要处理多个异步事件、构建可扩展的应用程序的情况。</li>
<li>优点：松耦合，代码更具灵活性和可维护性，适合构建事件驱动的应用。</li>
<li>缺点：相对于简单的回调函数而言，有一些额外的复杂性。</li>

</ul>
</li>

</ul>
<p>在实际应用中，根据具体需求选择适当的编程方式，有时也会结合使用，例如使用Promise和async/await结合回调函数或事件驱动的方式。3.3 Promise和async/await</p>
<h3 id='33-promise-和-asyncawait'>3.3 Promise 和 async/await</h3>
<h4 id='331-promise'>3.3.1 Promise</h4>
<p>Promise 是一种用于处理异步操作的对象，它表示一个异步操作的最终完成或失败，以及其结果值。Promise对象具有三个状态：<code>pending</code>（进行中）、<code>fulfilled</code>（已成功）和<code>rejected</code>（已失败）。</p>
<pre><code class='language-javascript' lang='javascript'>const myPromise = new Promise((resolve, reject) =&gt; {
  // 模拟异步操作
  setTimeout(() =&gt; {
    const success = true;
    if (success) {
      resolve(&#39;Async data&#39;);
    } else {
      reject(&#39;Error&#39;);
    }
  }, 1000);
});

// 使用Promise
myPromise
  .then((result) =&gt; {
    console.log(result);
  })
  .catch((error) =&gt; {
    console.error(error);
  });
</code></pre>
<p>在上面的例子中，<code>myPromise</code> 是一个Promise对象，通过 <code>resolve</code> 和 <code>reject</code> 参数，可以控制Promise对象的状态。使用 <code>.then()</code> 处理成功状态，<code>.catch()</code> 处理失败状态。</p>
<h4 id='332-asyncawait'>3.3.2 async/await</h4>
<p><code>async/await</code> 是 ES2017（ES8）引入的一种异步编程的语法糖，它使得异步代码的写法更加类似同步代码，提高了代码的可读性。</p>
<pre><code>function fetchData() {
  return new Promise((resolve, reject) =&gt; {
    // 模拟异步操作
    setTimeout(() =&gt; {
      const success = true;
      if (success) {
        resolve(&#39;Async data&#39;);
      } else {
        reject(&#39;Error&#39;);
      }
    }, 1000);
  });
}

// 使用async/await
async function getData() {
  try {
    const result = await fetchData();
    console.log(result);
  } catch (error) {
    console.error(error);
  }
}

getData();
</code></pre>
<p>在上面的例子中，<code>async</code> 关键字用于定义异步函数，而 <code>await</code> 关键字用于等待一个Promise对象的解决。在 <code>getData</code> 函数中，通过 <code>await fetchData()</code> 实现了等待异步操作完成的效果。</p>
<h4 id='333-区别与应用场景'>3.3.3 区别与应用场景</h4>
<ul>
<li><p><strong>Promise：</strong></p>
<ul>
<li>使用场景：适用于处理单个异步操作，或需要串行执行多个异步操作的情况。</li>
<li>优点：提供了一种规范化的异步处理方式，避免了回调地狱。</li>
<li>缺点：对于一些复杂的异步流程，仍然可能使代码变得复杂。</li>

</ul>
</li>
<li><p><strong>async/await：</strong></p>
<ul>
<li>使用场景：适用于异步操作相对简单的情况，提高了异步代码的可读性，特别是在处理多个异步操作时更容易理解。</li>
<li>优点：语法更直观，类似同步代码；可以有效地处理异步代码的异常。</li>
<li>缺点：相对于Promise，可能在一些特殊场景下性能略差。</li>

</ul>
</li>

</ul>
<p>在实际项目中，Promise和async/await通常是结合使用的，通过Promise构建异步操作，然后在需要的地方使用async/await语法糖来简化代码。选择使用哪种方式取决于项目的需求和个人/团队的编码风格。</p>
<h3 id='34-处理异步错误'>3.4 处理异步错误</h3>
<p>处理异步错误是异步编程中非常重要的一部分，以确保程序的稳定性和可靠性。以下是一些常见的处理异步错误的方法：</p>
<h3 id='1-回调函数方式'>1. 回调函数方式</h3>
<p>使用回调函数时，通常约定将错误作为回调函数的第一个参数传递，然后在回调函数中检查错误。</p>
<pre><code>function fetchData(callback) {
  setTimeout(() =&gt; {
    const success = false;
    if (success) {
      callback(null, &#39;Async data&#39;);
    } else {
      callback(&#39;Error&#39;);
    }
  }, 1000);
}

fetchData((err, result) =&gt; {
  if (err) {
    console.error(err);
  } else {
    console.log(result);
  }
});
</code></pre>
<h3 id='2-promise-方式'>2. Promise 方式</h3>
<p>在Promise中，通过 <code>.catch()</code> 方法捕获异步操作的错误。</p>
<pre><code>const myPromise = new Promise((resolve, reject) =&gt; {
  setTimeout(() =&gt; {
    const success = false;
    if (success) {
      resolve(&#39;Async data&#39;);
    } else {
      reject(&#39;Error&#39;);
    }
  }, 1000);
});

myPromise
  .then((result) =&gt; {
    console.log(result);
  })
  .catch((error) =&gt; {
    console.error(error);
  });
</code></pre>
<h3 id='3-asyncawait-方式'>3. async/await 方式</h3>
<p>使用 <code>try...catch</code> 结构可以捕获 <code>async/await</code> 中的异步错误。</p>
<pre><code>function fetchData() {
  return new Promise((resolve, reject) =&gt; {
    setTimeout(() =&gt; {
      const success = false;
      if (success) {
        resolve(&#39;Async data&#39;);
      } else {
        reject(&#39;Error&#39;);
      }
    }, 1000);
  });
}

async function getData() {
  try {
    const result = await fetchData();
    console.log(result);
  } catch (error) {
    console.error(error);
  }
}

getData();
</code></pre>
<h3 id='4-全局错误处理'>4. 全局错误处理</h3>
<p>可以通过监听 <code>unhandledRejection</code> 事件来全局捕获未处理的Promise rejection。</p>
<pre><code>process.on(&#39;unhandledRejection&#39;, (reason, promise) =&gt; {
  console.error(&#39;Unhandled Rejection at:&#39;, promise, &#39;reason:&#39;, reason);
  // 可以选择退出程序
  // process.exit(1);
});
</code></pre>
<p>在实际应用中，根据项目的需求和代码结构选择合适的方式来处理异步错误。细致的错误处理有助于更好地追踪和解决问题，并提高程序的可靠性。</p>
<h2 id='npm包管理器'>NPM包管理器</h2>
<h3 id='41-理解npm的基本用法'>4.1 理解npm的基本用法</h3>
<p><strong>npm（Node Package Manager）</strong> 是 Node.js 的包管理工具，用于下载、安装和管理 JavaScript 包。以下是一些常见的 npm 基本用法：</p>
<ol start='' >
<li><p><strong>初始化项目：</strong> 在项目根目录运行以下命令，创建 <code>package.json</code> 文件，该文件包含项目的配置信息。</p>
<pre><code>
npm init
</code></pre>
<p>通过回答一些问题，你可以配置项目的名称、版本、描述等信息。</p>
</li>
<li><p><strong>安装包：</strong> 使用 <code>npm install</code> 命令安装依赖包。</p>
<pre><code>
npm install package-name
</code></pre>
<p>也可以使用 <code>-g</code> 选项全局安装包。</p>
<pre><code>
npm install -g package-name
</code></pre>
</li>
<li><p><strong>查看安装的包：</strong> 使用 <code>npm ls</code> 或 <code>npm list</code> 命令查看已安装的包。</p>
<pre><code>
npm ls
</code></pre>
</li>
<li><p><strong>查看包信息：</strong> 使用 <code>npm info</code> 命令查看包的详细信息。</p>
<pre><code>
npm info package-name
</code></pre>
</li>
<li><p><strong>查找包：</strong> 使用 <code>npm search</code> 命令查找包。</p>
<pre><code>
npm search package-name
</code></pre>
</li>
<li><p><strong>更新包：</strong> 使用 <code>npm update</code> 命令更新包。</p>
<pre><code>
npm update package-name
</code></pre>
</li>
<li><p><strong>查看已过时的包：</strong> 使用 <code>npm outdated</code> 命令查看已过时的包。</p>
<pre><code>
npm outdated
</code></pre>
</li>
<li><p><strong>卸载包：</strong> 使用 <code>npm uninstall</code> 命令卸载包。</p>
<pre><code>
npm uninstall package-name
</code></pre>
</li>

</ol>
<h3 id='42-安装卸载和更新包'>4.2 安装、卸载和更新包</h3>
<h4 id='安装包'>安装包：</h4>
<p>使用 <code>npm install</code> 命令安装依赖包。可以通过以下方式之一：</p>
<pre><code>
npm install package-name
</code></pre>
<p>或者在 <code>package.json</code> 文件中添加依赖，并运行 <code>npm install</code>：</p>
<pre><code>
npm install
</code></pre>
<h4 id='卸载包'>卸载包：</h4>
<p>使用 <code>npm uninstall</code> 命令卸载包。可以通过以下方式之一：</p>
<pre><code>
npm uninstall package-name
</code></pre>
<p>或者在 <code>package.json</code> 文件中移除依赖，并运行 <code>npm uninstall</code>：</p>
<pre><code>
npm uninstall
</code></pre>
<h4 id='更新包'>更新包：</h4>
<p>使用 <code>npm update</code> 命令更新包。可以通过以下方式之一：</p>
<pre><code>
npm update package-name
</code></pre>
<p>或者运行以下命令更新所有依赖包：</p>
<pre><code>
npm update
</code></pre>
<h3 id='43-创建和管理自己的npm包'>4.3 创建和管理自己的npm包</h3>
<p>如果你有意向创建自己的 npm 包，可以按照以下步骤：</p>
<ol start='' >
<li><p><strong>创建项目：</strong> 创建一个新的文件夹，并在文件夹内初始化一个新的 Node.js 项目。</p>
<pre><code>
npm init
</code></pre>
<p>这将引导你填写项目信息，生成 <code>package.json</code> 文件。</p>
</li>
<li><p><strong>编写代码：</strong> 编写你的 JavaScript 代码并确保它正常工作。</p>
</li>
<li><p><strong>创建入口文件：</strong> 在项目中创建一个入口文件，通常命名为 <code>index.js</code>。</p>
</li>
<li><p><strong>发布包：</strong> 登录 npm 账号（使用 <code>npm login</code> 命令），然后发布你的包。</p>
<pre><code>
npm publish
</code></pre>
<p>请确保你的包名是唯一的。第一次发布时可能需要确认邮箱。</p>
</li>
<li><p><strong>更新包：</strong> 如果你对包进行了修改并希望发布新版本，可以先更新版本号（在 <code>package.json</code> 中），然后重新发布。</p>
<pre><code>npm version &lt;update_type&gt;
npm publish
</code></pre>
<p><code>&lt;update_type&gt;</code> 可以是 <code>patch</code>、<code>minor</code> 或 <code>major</code>，用于指定版本更新的类型。</p>
</li>

</ol>
<p>以上是创建和管理 npm 包的基本流程，更详细的信息可以在 <a href='https://docs.npmjs.com/'>npm 官方文档</a> 中找到。创建并分享自己的 npm 包是社区参与的好方法，也能为其他开发者提供有用的工具和库。</p>
<h2 id='5-express框架'>5. <strong>Express框架</strong></h2>
<p>5.1 理解Express框架的作用和优势</p>
<p>5.2 创建基本的Express应用程序</p>
<p>5.3 路由和中间件的使用</p>
<p>5.4 处理请求和响应</p>
<h2 id='6-数据库连接'>6. <strong>数据库连接</strong></h2>
<p>6.1 使用Node.js连接数据库（例如MongoDB、MySQL）</p>
<p>6.2 执行基本的数据库操作（增删改查）</p>
<h2 id='7-restful-api设计'>7. <strong>RESTful API设计</strong></h2>
<p>7.1 了解RESTful API的概念</p>
<p>7.2 使用Express构建RESTful API</p>
<h2 id='8-websocket'>8. <strong>WebSocket</strong></h2>
<p>8.1 了解WebSocket的概念和用途</p>
<p>8.2 使用WebSocket实现实时通信</p>
<h2 id='9-测试和调试'>9. <strong>测试和调试</strong></h2>
<p>9.1 使用断言库进行测试</p>
<p>9.2 使用Node.js调试工具</p>
<h2 id='10-部署和维护'>10. <strong>部署和维护</strong></h2>
<p>10.1 部署Node.js应用到服务器</p>
<p>10.2 监控和日志</p>
<p>10.3 安全性考虑</p>
<h2 id='11-其他nodejs工具和框架'>11. <strong>其他Node.js工具和框架</strong></h2>
<p>11.1 学习其他流行的Node.js工具和框架（如Socket.io、GraphQL）</p>
<h2 id='12-实际项目'>12. <strong>实际项目</strong></h2>
<p>12.1 应用所学知识创建一个小型项目</p>
<p>12.2 尝试解决真实问题并优化应用</p>
<ul>
<li><ul>
<li></li>

</ul>
</li>

</ul>
</body>