---
title: Easy CSS
date: 2023-11-05 09:05:06
tags: web
categories:
- 学习
- 计算机
- 前端
cover: https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQuXXqnhoPvHQ9kWgT-CuvhO1DJDMM4Bj3WkA&usqp=CAU
---

<body>
<p>CSS，从入门到？
<!-- more --></p>
<div>[TOC]</div>
<p>&nbsp;</p>
<h2 id='qa'>Q&amp;A</h2>
<h3 id='css-core'>CSS Core?</h3>
<p>核心的 CSS 概念之一是“盒子模型”（Box Model），它是 CSS 中用于布局的基本原理。盒子模型描述了 HTML 元素是如何在页面上布局的，每个元素都被看作是一个矩形的“盒子”，包含了内容、内边距、边框和外边距。</p>
<h4 id='盒子模型的组成部分'>盒子模型的组成部分</h4>
<ol start='' >
<li><strong>内容区域（Content Area）</strong>：元素的实际内容，比如文本、图像等。</li>
<li><strong>内边距区域（Padding Area）</strong>：内容区域周围的空白区域，通过 <code>padding</code> 属性控制。</li>
<li><strong>边框区域（Border Area）</strong>：内边距区域外围的边框，通过 <code>border</code> 属性控制。</li>
<li><strong>外边距区域（Margin Area）</strong>：边框区域外的空白区域，通过 <code>margin</code> 属性控制。</li>

</ol>
<h4 id='如何设置盒子模型的属性'>如何设置盒子模型的属性</h4>
<ul>
<li><p><strong>设置盒子尺寸：</strong> 使用 <code>width</code> 和 <code>height</code> 属性设置元素的宽度和高度。</p>
<pre><code>div {
  width: 200px;
  height: 100px;
}
</code></pre>
</li>
<li><p><strong>设置内边距：</strong> 使用 <code>padding</code> 属性设置元素的内边距。</p>
<pre><code>div {
  padding: 20px;
}
</code></pre>
</li>
<li><p><strong>设置边框：</strong> 使用 <code>border</code> 属性设置元素的边框。</p>
<pre><code>div {
  border: 2px solid #000;
}
</code></pre>
</li>
<li><p><strong>设置外边距：</strong> 使用 <code>margin</code> 属性设置元素的外边距。</p>
<pre><code>div {
  margin: 10px;
}
</code></pre>
</li>

</ul>
<h4 id='盒子模型的计算方式'>盒子模型的计算方式</h4>
<ul>
<li><strong>标准盒子模型：</strong> 在标准盒子模型中，元素的宽度和高度仅包括内容区域（不包括内边距、边框和外边距）。</li>
<li><strong>IE 盒子模型：</strong> 在 IE 盒子模型中，元素的宽度和高度包括了内边距和边框，但不包括外边距。</li>

</ul>
<p>你可以通过设置 <code>box-sizing</code> 属性来指定使用哪种盒子模型。例如：</p>
<pre><code>div {
  box-sizing: border-box; /*使用 IE 盒子模型*/
}
</code></pre>
<p>总的来说，盒子模型是 CSS 中布局的基础，了解和熟练使用盒子模型的相关属性是掌握 CSS 核心概念的关键之一。</p>
<h3 id='what-can-css-do'>What can CSS Do?</h3>
<p>CSS（层叠样式表）是一种强大的样式语言，使得Web开发人员能够控制网页上HTML元素的呈现和布局。以下是CSS能够实现的一些功能，特别是在“盒子及其内部”这个背景下：</p>
<ol start='' >
<li><p><strong>布局和定位：</strong></p>
<ul>
<li><strong>盒子模型：</strong> CSS允许通过盒子模型来控制元素的布局。这包括设置元素的宽度、高度、内边距、边框和外边距。</li>
<li><strong>定位：</strong> CSS提供了相对定位、绝对定位、固定定位和粘性定位等不同的定位方案，以精确控制元素在页面上的位置。</li>

</ul>
</li>
<li><p><strong>样式和装饰：</strong></p>
<ul>
<li><strong>颜色和背景：</strong> CSS允许设置文本和背景的颜色，包括使用渐变和图像作为背景。</li>
<li><strong>边框和圆角：</strong> 您可以为元素应用不同样式和宽度的边框，并使用 <code>border-radius</code> 创建圆角。</li>
<li><strong>阴影：</strong> CSS可以使用 <code>box-shadow</code> 属性为元素创建阴影效果。</li>

</ul>
</li>
<li><p><strong>排版：</strong></p>
<ul>
<li><strong>字体样式：</strong> CSS允许您控制文本的字体系列、大小、粗细、样式等属性。</li>
<li><strong>文本对齐和装饰：</strong> 您可以对齐文本，给文本加下划线或删除线等装饰。</li>
<li><strong>字母和单词间距：</strong> 使用 <code>letter-spacing</code> 和 <code>word-spacing</code> 属性调整字母和单词之间的间距。</li>

</ul>
</li>
<li><p><strong>响应式设计：</strong></p>
<ul>
<li><strong>媒体查询：</strong> CSS通过使用媒体查询根据设备的特性（如屏幕宽度）应用样式，从而实现响应式设计。</li>

</ul>
</li>
<li><p><strong>变换和过渡：</strong></p>
<ul>
<li><strong>变换：</strong> CSS提供缩放、旋转、倾斜和平移等变换，可以用于调整元素的外观。</li>
<li><strong>过渡：</strong> 使用CSS过渡，可以在一段时间内平滑地动画属性的变化。</li>

</ul>
</li>
<li><p><strong>Flexbox 和 Grid 布局：</strong></p>
<ul>
<li><strong>Flexbox：</strong> CSS的Flexbox是一种布局模型，可以更有效地设计复杂的布局，特别是在分配空间和对齐项目方面。</li>
<li><strong>Grid 布局：</strong> CSS Grid提供了一个二维布局系统，更容易创建基于网格的设计。</li>

</ul>
</li>
<li><p><strong>伪类和伪元素：</strong></p>
<ul>
<li><strong>伪类：</strong> 通过伪类（如 <code>:hover</code>、<code>:active</code>、<code>:focus</code>）选择和样式元素的不同状态。</li>
<li><strong>伪元素：</strong> 样式元素的特定部分，例如 <code>::before</code> 和 <code>::after</code>。</li>

</ul>
</li>
<li><p><strong>动画：</strong></p>
<ul>
<li><strong>关键帧动画：</strong> CSS支持关键帧动画，通过定义关键帧并将其应用于元素，可以创建复杂的动画效果。</li>

</ul>
</li>
<li><p><strong>自定义和主题化：</strong></p>
<ul>
<li><strong>变量：</strong> CSS变量（<code>--variable-name</code>）允许创建可重用和可自定义的样式。</li>
<li><strong>@media规则：</strong> 使用 <code>@media</code> 规则根据输出设备的特性应用不同的样式。</li>

</ul>
</li>

</ol>
<p>总的来说，CSS是Web开发人员控制网页视觉呈现的重要工具，提供了广泛的功能，用于创建美观且响应式的设计。&quot;盒子及其内部&quot;的概念强调HTML元素被视为盒子，并且CSS提供了在文档中样式和排列这些盒子的手段。</p>
<h3 id='how'>How?</h3>
<h4 id='selector-and-declarationattribution-and-value'>Selector and declaration(attribution and value)</h4>
<ol start='' >
<li>在CSS中，样式规则由选择器和声明组成。每个样式规则定义了页面上特定元素的样式，包括元素应用的属性和属性的值。下面是关于选择器和声明的基本概念：</li>

</ol>
<h4 id='选择器selectors）'>选择器（Selectors）</h4>
<p>   选择器用于选择页面上要样式化的元素。它告诉浏览器应该应用哪些样式规则。以下是一些常见的选择器类型：</p>
<ol start='' >
<li><p><strong>元素选择器（Element Selector）：</strong> 根据元素的名称选择元素。</p>
<pre><code>p {
  /*样式规则 */
}
</code></pre>
</li>
<li><p><strong>类选择器（Class Selector）：</strong> 根据元素的类名选择元素。</p>
<pre><code>.highlight {
  /* 样式规则 */
}
</code></pre>
</li>
<li><p><strong>ID 选择器（ID Selector）：</strong> 根据元素的 ID 选择元素。</p>
<pre><code>#header {
  /* 样式规则 */
}
</code></pre>
</li>
<li><p><strong>属性选择器（Attribute Selector）：</strong> 根据元素的属性选择元素。</p>
<pre><code>input[type=&quot;text&quot;] {
  /* 样式规则 */
}
</code></pre>
</li>
<li><p><strong>伪类选择器（Pseudo-class Selector）：</strong> 根据元素的状态或位置选择元素。</p>
<pre><code>a:hover {
  /* 样式规则 */
}
</code></pre>
</li>
<li><p><strong>伪元素选择器（Pseudo-element Selector）：</strong> 选择元素的特定部分。</p>
<pre><code>p::first-line {
  /* 样式规则*/
}
</code></pre>
</li>

</ol>
<h4 id='声明declarations）'>声明（Declarations）</h4>
<p>   声明由属性和属性值组成。每个声明指定了要应用于选择的元素的一种样式。以下是声明的基本结构：</p>
<pre><code>selector {
  property: value;
}
</code></pre>
<ul>
<li><strong>属性（Property）：</strong> 指定要设置的样式的类型，比如 <code>color</code>、<code>font-size</code>、<code>margin</code> 等。</li>
<li><strong>值（Value）：</strong> 指定给属性的具体值，比如 <code>red</code>、<code>16px</code>、<code>10px 20px</code>。</li>

</ul>
<p>   例如，将段落文字颜色设置为红色：</p>
<pre><code>p {
  color: red;
}
</code></pre>
<p>   或者将标题的字体大小设置为16像素：</p>
<pre><code>h1 {
  font-size: 16px;
}
</code></pre>
<p>   多个声明可以组合在一个样式规则中：</p>
<pre><code>h2 {
  color: blue;
  font-size: 18px;
  margin-bottom: 10px;
}
</code></pre>
<p>   通过选择器和声明，你可以有效地控制页面上各个元素的外观和布局。CSS的强大之处在于其层叠性质，允许多个样式规则同时应用到一个元素上，最终形成最终的样式。</p>
<h3 id='add-css'>Add CSS</h3>
<p>在HTML文档中添加CSS样式的常见方法有两种：使用<code>&lt;link&gt;</code>元素和<code>&lt;style&gt;</code>元素。</p>
<h4 id='1-使用-link-元素'>1. 使用 <code>&lt;link&gt;</code> 元素</h4>
<p><code>&lt;link&gt;</code> 元素用于将外部样式表链接到HTML文档。它通常位于HTML文档的 <code>&lt;head&gt;</code> 部分。以下是添加CSS样式的基本语法：</p>
<pre><code>html&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;en&quot;&gt;
&lt;head&gt;
  &lt;meta charset=&quot;UTF-8&quot;&gt;
  &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
  &lt;title&gt;Document&lt;/title&gt;
  
  &lt;!-- 使用 link 元素引入外部样式表 --&gt;
  &lt;link rel=&quot;stylesheet&quot; type=&quot;text/css&quot; href=&quot;styles.css&quot;&gt;
&lt;/head&gt;
&lt;body&gt;
  &lt;!-- 页面内容 --&gt;
&lt;/body&gt;
&lt;/html&gt;
</code></pre>
<p>在上面的例子中，<code>href</code> 属性指定了外部样式表的文件路径，<code>type</code> 属性指定了样式表的类型为CSS，<code>rel</code> 属性表示关系为样式表。</p>
<h4 id='2-使用-style-元素'>2. 使用 <code>&lt;style&gt;</code> 元素</h4>
<style> 元素用于在HTML文档中嵌入CSS样式。可以将其放置在文档的 <head> 部分或 <body> 部分。以下是在文档头部添加嵌入式CSS样式的基本语法：</body></style>
<pre><code>html&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;en&quot;&gt;
&lt;head&gt;
  &lt;meta charset=&quot;UTF-8&quot;&gt;
  &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
  &lt;title&gt;Document&lt;/title&gt;
  
  &lt;!-- 使用 style 元素嵌入CSS样式 --&gt;
  &lt;style type=&quot;text/css&quot;&gt;
    /*CSS 样式规则*/
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
    }

    h1 {
      color: blue;
    }
  &lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;
  &lt;!-- 页面内容 --&gt;
&lt;/body&gt;
&lt;/html&gt;
</code></pre>
<p>在上面的例子中，<code>&lt;style&gt;</code> 元素的 <code>type</code> 属性指定了样式表的类型为CSS。在 <code>&lt;style&gt;</code> 元素内部，可以编写CSS样式规则，就像在外部样式表或独立的CSS文件中一样。</p>
<p><strong>注意：</strong></p>
<ul>
<li>使用外部样式表的优势在于样式可以在多个页面之间共享，并且使得HTML文档更为清晰和可维护。</li>
<li>使用嵌入式样式表的优势在于它将HTML和CSS放在同一个文件中，适用于较小规模的项目或需要特定样式的单个页面。</li>

</ul>
<h3 id='how-selector-works'>How Selector Works?</h3>
<ol start='' >
<li>CSS选择器（Selector）用于选择要应用样式的HTML元素。选择器的工作原理是根据选择器的类型和匹配规则，选择文档中的特定元素。以下是一些常见的CSS选择器及其工作原理：</li>

</ol>
<h4 id='1-通用选择器-'>1. 通用选择器 <code>*</code></h4>
<p>   <code>*</code> 选择器匹配文档中的所有元素。</p>
<pre><code>*{
  /* 应用于所有元素的样式规则 */
}
</code></pre>
<h4 id='2-标签选择器-tag'>2. 标签选择器 <code>tag</code></h4>
<p>   标签选择器选择特定类型的元素。</p>
<pre><code>p {
  /* 应用于所有 &lt;p&gt; 元素的样式规则 */
}
</code></pre>
<h4 id='3-类选择器-class标签与类选择器-tagclass'>3. 类选择器 <code>.class</code>、标签与类选择器 <code>tag.class</code></h4>
<p>   类选择器选择具有特定类的元素，标签与类选择器选择特定标签下带有特定类的元素。</p>
<pre><code>.button {
  /* 应用于所有类为 button 的元素的样式规则 */
}

h1.title {
  /*应用于所有 &lt;h1&gt; 标签且类为 title 的元素的样式规则*/
}
</code></pre>
<h4 id='4-id-选择器-id'>4. ID 选择器 <code>#id</code></h4>
<p>   ID选择器选择具有特定ID的元素。</p>
<pre><code>#header {
  /*应用于 ID 为 header 的元素的样式规则 */
}
</code></pre>
<h4 id='5-子元素选择器-parent--sub'>5. 子元素选择器 <code>parent &gt; sub</code></h4>
<p>   子元素选择器选择作为指定父元素的直接子元素的元素。</p>
<pre><code>nav &gt; ul {
  /* 应用于所有 &lt;ul&gt; 元素，但仅在其直接位于 &lt;nav&gt; 下时生效 */
}
</code></pre>
<h4 id='6-后代元素选择器-parent-nestedtag'>6. 后代元素选择器 <code>parent nestedtag</code></h4>
<p>   后代元素选择器选择指定祖先元素内的所有后代元素。</p>
<pre><code>article p {
  /* 应用于所有 &lt;p&gt; 元素，但仅在其位于 &lt;article&gt; 元素内时生效 */
}
</code></pre>
<h4 id='7-相邻兄弟选择器-tagnexttag'>7. 相邻兄弟选择器 <code>tag+nexttag</code></h4>
<p>   相邻兄弟选择器选择紧接在指定元素后的相邻元素。</p>
<pre><code>h2 + p {
  /* 应用于紧接在 &lt;h2&gt; 元素后的第一个 &lt;p&gt; 元素 */
}
</code></pre>
<h4 id='8-通用兄弟选择器-tagsiblingtag'>8. 通用兄弟选择器 <code>tag~siblingtag</code></h4>
<p>   通用兄弟选择器选择指定元素之后的所有兄弟元素。</p>
<pre><code>h2 ~ p {
  /* 应用于 &lt;h2&gt; 元素后的所有 &lt;p&gt; 兄弟元素 */
}
</code></pre>
<h4 id='9-属性选择器-tagattribute'>9. 属性选择器 <code>tag[attribute]</code></h4>
<p>   属性选择器选择具有指定属性的元素。</p>
<pre><code>input[type] {
  /* 应用于所有带有 type 属性的 &lt;input&gt; 元素 */
}
</code></pre>
<h4 id='10-属性值选择器-tagattributevalue'>10. 属性值选择器 <code>tag[attribute=value]</code></h4>
<p>   属性值选择器选择具有指定属性和属性值的元素。</p>
<pre><code>a[href=&quot;https://example.com&quot;] {
  /* 应用于所有链接到 &quot;https://example.com&quot; 的 &lt;a&gt; 元素 */
}
</code></pre>
<h4 id='11-包含属性值选择器-tagattributevalue'>11. 包含属性值选择器 <code>tag[attribute~=value]</code></h4>
<p>   包含属性值选择器选择具有指定属性，并且该属性的值包含指定词汇的元素。</p>
<pre><code>p[class~=&quot;important&quot;] {
  /* 应用于所有类属性中包含 &quot;important&quot; 的 &lt;p&gt; 元素 */
}
</code></pre>
<h4 id='12-属性值前缀选择器-tagattributevalue'>12. 属性值前缀选择器 <code>tag[attribute^=value]</code></h4>
<p>   属性值前缀选择器选择具有以指定值开头的属性值的元素。</p>
<pre><code>a[href^=&quot;https://&quot;] {
  /* 应用于所有链接到以 &quot;https://&quot; 开头的地址的 &lt;a&gt; 元素 */
}
</code></pre>
<h4 id='13-属性值后缀选择器-tagattributevalue'>13. 属性值后缀选择器 <code>tag[attribute$=value]</code></h4>
<p>   属性值后缀选择器选择具有以指定值结尾的属性值的元素。</p>
<pre><code>img[src$=&quot;.png&quot;] {
  /* 应用于所有引用以 &quot;.png&quot; 结尾的图片的 &lt;img&gt; 元素 */
}
</code></pre>
<h4 id='14-属性值包含选择器-tagattributevalue'>14. 属性值包含选择器 <code>tag[attribute*=value]</code></h4>
<p>   属性值包含选择器选择具有包含指定值的属性值的元素。</p>
<pre><code>a[href*=&quot;example&quot;] {
  /* 应用于所有链接到包含 &quot;example&quot; 的地址的 &lt;a&gt; 元素*/
}
</code></pre>
<p>   CSS选择器的灵活性允许开发人员以多种方式选择和定位页面中的元素，从而实现对页面样式的精确控制。</p>
<h2 id='颜色color）'>颜色（Color）</h2>
<h4 id='颜色属性color-properties）'>颜色属性（Color Properties）</h4>
<ul>
<li><p><strong>文本颜色（Text Color）</strong>：通过 <code>color</code> 属性设置文本的颜色。可以使用颜色名称、十六进制值、RGB 值等表示。例如：</p>
<pre><code>p {
  color: red;
}
</code></pre>
</li>
<li><p><strong>背景颜色（Background Color）</strong>：通过 <code>background-color</code> 属性设置元素的背景颜色。同样，可以使用不同的表示方法。例如：</p>
<pre><code>div {
  background-color: #f0f0f0;
}
</code></pre>
</li>

</ul>
<h4 id='透明度opacity）'>透明度（Opacity）</h4>
<ul>
<li><p><strong>透明度（Opacity）</strong>：通过 <code>opacity</code> 属性设置元素的透明度。值为 0.0 到 1.0 之间的数字，0.0 表示完全透明，1.0 表示完全不透明。例如：</p>
<pre><code>div {
  opacity: 0.7;
}
</code></pre>
</li>
<li><p><strong>RGBA 颜色表示</strong>：使用 <code>rgba</code> 函数表示颜色，其中 <code>a</code> 代表 alpha 通道（透明度）。例如：</p>
<pre><code>div {
  background-color: rgba(255, 0, 0, 0.5); /*半透明红色背景*/
}
</code></pre>
</li>

</ul>
<h4 id='hsl-和-hsla-表示法'>HSL 和 HSLA 表示法</h4>
<ul>
<li><p><strong>HSL 颜色表示</strong>：使用 <code>hsl</code> 函数表示颜色，分别设置色相（Hue）、饱和度（Saturation）、亮度（Lightness）。例如：</p>
<pre><code>div {
  background-color: hsl(120, 100%, 50%); /*绿色背景 */
}
</code></pre>
</li>
<li><p><strong>HSLA 颜色表示</strong>：在 <code>hsl</code> 的基础上增加 alpha 通道。例如：</p>
<pre><code>div {
  background-color: hsla(120, 100%, 50%, 0.7); /* 半透明绿色背景*/
}
</code></pre>
</li>

</ul>
<p>以上是关于颜色的一些常见CSS技术，通过灵活运用这些属性，可以创建丰富多彩的界面效果。</p>
<h2 id='文本和字体text-and-font）'>文本和字体（Text and Font）</h2>
<h4 id='字体族font-family）'>字体族（Font Family）</h4>
<p><code>font-family</code> 属性用于设置文本的字体族。可以指定多个字体，以备选项的形式存在，以确保在用户计算机上始终能够找到合适的字体。例如：</p>
<pre><code>body {
  font-family: &#39;Arial&#39;, &#39;Helvetica&#39;, sans-serif;
}
</code></pre>
<h4 id='字体大小font-size）'>字体大小（Font Size）</h4>
<p><code>font-size</code> 属性用于设置文本的大小，可以使用像素（px）、百分比（%）、相对长度单位（em）等。例如：</p>
<pre><code>p {
  font-size: 16px;
}
</code></pre>
<h4 id='字体引入font-face）'>字体引入（@font-face）</h4>
<p><code>@font-face</code> 规则允许自定义字体文件，以便在网页上使用。例如：</p>
<pre><code>@font-face {
  font-family: &#39;CustomFont&#39;;
  src: url(&#39;custom-font.woff&#39;) format(&#39;woff&#39;);
}
body {
  font-family: &#39;CustomFont&#39;, sans-serif;
}
</code></pre>
<h4 id='字体粗细font-weight）'>字体粗细（Font Weight）</h4>
<p><code>font-weight</code> 属性用于设置文本的粗细，可以是数字值，也可以是关键字如 <code>normal</code> 或 <code>bold</code>。例如：</p>
<pre><code>strong {
  font-weight: bold;
}
</code></pre>
<h4 id='字体样式font-style）'>字体样式（Font Style）</h4>
<p><code>font-style</code> 属性用于设置文本的样式，如斜体。例如：</p>
<pre><code>em {
  font-style: italic;
}
</code></pre>
<h4 id='字体变形text-transform）'>字体变形（Text Transform）</h4>
<p><code>text-transform</code> 属性用于控制文本的大小写。例如：</p>
<pre><code>span {
  text-transform: uppercase;
}
</code></pre>
<h4 id='文本装饰text-decoration）'>文本装饰（Text Decoration）</h4>
<p><code>text-decoration</code> 属性用于控制文本的装饰效果，如下划线、删除线等。例如：</p>
<pre><code>a {
  text-decoration: none;
}
</code></pre>
<h4 id='行高line-height）'>行高（Line Height）</h4>
<p><code>line-height</code> 属性用于设置行高，最好使用相对长度单位（如 em）以提高可伸缩性。例如：</p>
<pre><code>p {
  line-height: 1.5;
}
</code></pre>
<h4 id='字母和单词间距letter-and-word-spacing）'>字母和单词间距（Letter and Word Spacing）</h4>
<ul>
<li><p><strong>字母间距（Letter Spacing）</strong>：<code>letter-spacing</code> 属性用于设置字母之间的间距。例如：</p>
<pre><code>h1 {
  letter-spacing: 2px;
}
</code></pre>
</li>
<li><p><strong>单词间距（Word Spacing）</strong>：<code>word-spacing</code> 属性用于设置单词之间的间距。例如：</p>
<pre><code>p {
  word-spacing: 5px;
}
</code></pre>
</li>

</ul>
<h4 id='文本对齐text-align）'>文本对齐（Text Align）</h4>
<p><code>text-align</code> 属性用于设置文本的对齐方式，如左对齐、右对齐、居中等。例如：</p>
<pre><code>div {
  text-align: center;
}
</code></pre>
<h4 id='垂直对齐vertical-align）'>垂直对齐（Vertical Align）</h4>
<p><code>vertical-align</code> 属性用于设置内联元素的垂直对齐方式。例如：</p>
<pre><code>img {
  vertical-align: middle;
}
</code></pre>
<h4 id='文本缩进text-indent）'>文本缩进（Text Indent）</h4>
<p><code>text-indent</code> 属性用于设置文本的首行缩进。例如：</p>
<pre><code>p {
  text-indent: 20px;
}
</code></pre>
<h4 id='文本阴影text-shadow）'>文本阴影（Text Shadow）</h4>
<p><code>text-shadow</code> 属性用于设置文本的阴影效果，包括阴影方向、偏移、大小和颜色。例如：</p>
<pre><code>h1 {
  text-shadow: 2px 2px 4px #999999;
}
</code></pre>
<h4 id='伪元素pseudo-elements）'>伪元素（Pseudo Elements）</h4>
<ul>
<li><code>:first-letter</code>：用于选择文本的第一个字母。</li>
<li><code>:first-line</code>：用于选择文本的第一行。</li>

</ul>
<pre><code>p:first-letter {
  font-size: 150%;
}

p:first-line {
  color: blue;
}
</code></pre>
<h4 id='伪类pseudo-classes）-1'>伪类（Pseudo Classes）</h4>
<ul>
<li><code>:link</code> 和 <code>:visited</code>：分别用于选择未访问和已访问的链接。</li>
<li><code>:hover</code>、 <code>:active</code>、 <code>:focus</code>：用于响应用户的鼠标悬停、激活和焦点状态。</li>

</ul>
<pre><code>a:link {
  color: blue;
}

a:hover {
  color: red;
}

a:visited {
  color: purple;
}
</code></pre>
<p>以上是一些关于文本和字体样式的常见CSS技术，它们对于创建吸引人的页面内容至关重要。</p>
<h2 id='盒子模型box-model）'>盒子模型（Box Model）</h2>
<h4 id='尺寸属性dimension-properties）'>尺寸属性（Dimension Properties）</h4>
<ul>
<li><p><code>width</code>、<code>min-width</code>、<code>max-width</code>：分别用于设置元素的宽度、最小宽度和最大宽度。例如：</p>
<pre><code>div {
  width: 300px;
  min-width: 100px;
  max-width: 500px;
}
</code></pre>
</li>
<li><p><code>height</code>、<code>min-height</code>、<code>max-height</code>：分别用于设置元素的高度、最小高度和最大高度。例如：</p>
<pre><code>div {
  height: 200px;
  min-height: 50px;
  max-height: 300px;
}
</code></pre>
</li>

</ul>
<h4 id='溢出处理overflow）'>溢出处理（Overflow）</h4>
<p><code>overflow</code> 属性用于控制当内容溢出容器时的处理方式。例如：</p>
<pre><code>div {
  overflow: hidden; /*或者 overflow: scroll;*/
}
</code></pre>
<h4 id='内边距边框外边距padding-border-margin）'>内边距、边框、外边距（Padding, Border, Margin）</h4>
<ul>
<li><p><strong>内边距（Padding）</strong>：<code>padding</code> 属性用于设置元素内部内容与边框之间的空白区域。可以分别设置上、右、下、左的内边距。例如：</p>
<pre><code>div {
  padding: 10px 20px 15px 5px;
}
</code></pre>
</li>
<li><p><strong>边框（Border）</strong>：<code>border</code> 属性用于设置元素的边框，包括宽度、样式和颜色。例如：</p>
<pre><code>div {
  border: 2px solid #000;
}
</code></pre>
<ul>
<li><p><strong>边框样式（Border Style）</strong>：<code>border-style</code> 属性定义边框的样式，如实线、虚线等。例如：</p>
<pre><code>div {
  border-style: dashed;
}
</code></pre>
</li>
<li><p><strong>边框颜色（Border Color）</strong>：<code>border-color</code> 属性定义边框的颜色。例如：</p>
<pre><code>div {
  border-color: #00f;
}
</code></pre>
</li>

</ul>
</li>
<li><p><strong>外边距（Margin）</strong>：<code>margin</code> 属性用于设置元素与相邻元素之间的空白区域。可以分别设置上、右、下、左的外边距。例如：</p>
<pre><code>div {
  margin: 10px 20px 15px 5px;
}
</code></pre>
</li>

</ul>
<h4 id='显示属性display-properties）'>显示属性（Display Properties）</h4>
<p><code>display</code> 属性用于设置元素的显示方式，包括块级元素、内联元素、内联块级元素等。例如：</p>
<pre><code>div {
  display: block; /*或者 display: inline;*/
}
</code></pre>
<ul>
<li><p><strong>可见性（Visibility）</strong>：<code>visibility</code> 属性用于控制元素的可见性，可以是隐藏或可见。例如：</p>
<pre><code>div {
  visibility: hidden;
}
</code></pre>
</li>

</ul>
<h4 id='边框图片border-image）'>边框图片（Border Image）</h4>
<p><code>border-image</code> 属性用于设置边框的图片样式，包括URL、拉伸、重复等。例如：</p>
<pre><code>div {
  border-image: url(&#39;border-image.png&#39;) 30 30 round;
}
</code></pre>
<h4 id='盒子阴影和圆角box-shadow-and-border-radius）'>盒子阴影和圆角（Box Shadow and Border Radius）</h4>
<ul>
<li><p><strong>盒子阴影（Box Shadow）</strong>：<code>box-shadow</code> 属性用于创建元素的阴影效果。例如：</p>
<pre><code>div {
  box-shadow: 5px 5px 10px #888888;
}
</code></pre>
</li>
<li><p><strong>圆角（Border Radius）</strong>：<code>border-radius</code> 属性用于设置元素的边框角的圆角程度。可以分别设置水平和垂直方向的圆角半径。例如：</p>
<pre><code>div {
  border-radius: 10px 20px;
}
</code></pre>
</li>

</ul>
<p>以上是有关盒子模型的一些常见CSS技术，它们对于布局和样式设计中起到了关键的作用。</p>
<h2 id='列表表格和表单list-table-and-form）'>列表、表格和表单（List, Table, and Form）</h2>
<h4 id='列表样式list-style）'>列表样式（List Style）</h4>
<p>列表样式用于定义列表项的外观。它包括以下属性：</p>
<ul>
<li><p><code>list-style-type</code>：指定列表项的标志类型，如圆点、数字、字母等。例如：</p>
<pre><code>ul {
  list-style-type: circle;
}
</code></pre>
</li>
<li><p><code>list-style-image</code>：用图像替代列表项的标志。例如：</p>
<pre><code>ul {
  list-style-image: url(&#39;bullet.png&#39;);
}
</code></pre>
</li>
<li><p><code>list-style-position</code>：控制列表项标志的位置，可以是内部或外部。例如：</p>
<pre><code>ul {
  list-style-position: inside;
}
</code></pre>
</li>

</ul>
<h4 id='空单元格处理empty-cells）'>空单元格处理（Empty Cells）</h4>
<p><code>empty-cells</code> 属性用于控制表格中空单元格的显示。例如：</p>
<pre><code>table {
  empty-cells: hide;
}
</code></pre>
<h4 id='表格边框和间距border-and-spacing-in-tables）'>表格边框和间距（Border and Spacing in Tables）</h4>
<ul>
<li><p><code>border-spacing</code>：设置相邻单元格之间的边框间距。例如：</p>
<pre><code>table {
  border-spacing: 5px;
}
</code></pre>
</li>
<li><p><code>border-collapse</code>：定义表格的边框模型，可以是分离的（separate）或合并的（collapse）。例如：</p>
<pre><code>table {
  border-collapse: collapse;
}
</code></pre>
</li>

</ul>
<h4 id='表单布局form-layout）'>表单布局（Form Layout）</h4>
<p>表单元素的布局可以通过不同的CSS属性来实现。以下是一些常用的属性：</p>
<ul>
<li><p><code>float</code>：通过浮动来布局表单元素。例如：</p>
<pre><code>input {
  float: left;
}
</code></pre>
</li>
<li><p><code>cursor</code>：定义鼠标悬停在表单元素上时的光标形状。例如：</p>
<pre><code>button {
  cursor: pointer;
}
</code></pre>
</li>
<li><p><code>auto</code>：浏览器设置默认的光标形状。例如：</p>
<pre><code>input {
  cursor: auto;
}
</code></pre>
</li>
<li><p><code>crosshair</code>、<code>default</code>、<code>pointer</code>、<code>move</code>、<code>text</code>、<code>wait</code>、<code>help</code>：分别设置光标形状为十字线、默认、指针、移动、文本输入、等待、帮助。例如：</p>
<pre><code>a {
  cursor: pointer;
}
</code></pre>
</li>
<li><p><code>url(&quot;&quot;)</code>：通过指定自定义光标的URL来设置光标形状。例如：</p>
<pre><code>a {
  cursor: url(&#39;custom-cursor.png&#39;), auto;
}
</code></pre>
</li>

</ul>
<p>以上是一些与列表、表格和表单相关的常见CSS技术，它们有助于定制化这些元素的外观和布局。</p>
<h2 id='布局和定位layout-and-position）'>布局和定位（Layout and Position）</h2>
<h4 id='静态流动static）'>静态流动（Static）</h4>
<p>静态流动是元素默认的定位方式。块级元素（block）会独占一行，而行内元素（inline）则在同一行内排列。例如：</p>
<pre><code>div {
  display: block; /*或者 display: inline;*/
}
</code></pre>
<h4 id='相对定位relative）'>相对定位（Relative）</h4>
<p>相对定位是相对于元素在文档流中的原始位置进行定位。通过使用 <code>position: relative;</code> 属性，你可以使用 <code>top</code>、<code>right</code>、<code>bottom</code> 和 <code>left</code> 属性来调整元素的位置。例如：</p>
<pre><code>div {
  position: relative;
  top: 10px;
  left: 20px;
}
</code></pre>
<h4 id='绝对定位absolute）'>绝对定位（Absolute）</h4>
<p>绝对定位是相对于最近的非静态定位祖先元素进行定位，如果没有这样的祖先元素，它将相对于文档的初始包含块。例如：</p>
<pre><code>div {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</code></pre>
<h5 id='绝对定位的变种'>绝对定位的变种</h5>
<ul>
<li><p><strong>跟随页面滚动（Absolute）</strong></p>
<p>当页面滚动时，元素保持在相对于视口的固定位置。例如：</p>
<pre><code>div {
  position: absolute;
  top: 10px;
  left: 10px;
}
</code></pre>
</li>
<li><p><strong>固定位置（Fixed Position）</strong></p>
<p>元素相对于视口固定，不随页面滚动而变化。例如：</p>
<pre><code>div {
  position: fixed;
  top: 0;
  left: 0;
}
</code></pre>
</li>

</ul>
<h4 id='浮动定位float-position）'>浮动定位（Float Position）</h4>
<p>浮动是一种使元素脱离正常文档流，向左或向右移动的布局方式。在浮动元素周围的文本和内联元素将围绕着它。例如：</p>
<pre><code>img {
  float: left;
}
</code></pre>
<h4 id='层叠顺序z-index）'>层叠顺序（Z-Index）</h4>
<p><code>z-index</code> 属性用于控制元素的层叠顺序。具有较高 <code>z-index</code> 值的元素将显示在具有较低 <code>z-index</code> 值的元素之上。例如：</p>
<pre><code>div {
  z-index: 1;
}
</code></pre>
<h4 id='清除浮动clear）'>清除浮动（Clear）</h4>
<p><code>clear</code> 属性用于控制元素的浮动行为。它指定了在元素旁边不允许浮动元素的一侧。例如：</p>
<pre><code>div {
  clear: both;
}
</code></pre>
<p>以上是有关布局和定位的一些常见CSS技术，它们对于创建灵活和响应式的页面布局至关重要。</p>
<h2 id='图片image）'>图片（Image）</h2>
<h4 id='尺寸size）'>尺寸（Size）</h4>
<p>在CSS中，你可以使用 <code>width</code> 和 <code>height</code> 属性来设置图像的尺寸。例如：</p>
<pre><code>img {
  width: 100px;
  height: 100px;
}
</code></pre>
<h4 id='对齐align）'>对齐（Align）</h4>
<p>通过使用 <code>float</code> 或 <code>display: flex</code>，你可以控制图像在其容器中的对齐方式。例如：</p>
<pre><code>img {
  float: left;
  /*或者使用 flexbox */
  display: flex;
  align-items: center;
  justify-content: center;
}
</code></pre>
<h3 id='背景background）'>背景（Background）</h3>
<h4 id='背景图像background-image）'>背景图像（Background Image）</h4>
<p>使用 <code>background-image</code> 属性可以设置元素的背景图像。例如：</p>
<pre><code>div {
  background-image: url(&#39;example.jpg&#39;);
}
</code></pre>
<h4 id='背景颜色background-color）'>背景颜色（Background Color）</h4>
<p>通过 <code>background-color</code> 属性，你可以设置元素的背景颜色。例如：</p>
<pre><code>div {
  background-color: #f0f0f0;
}
</code></pre>
<h4 id='背景重复background-repeat）'>背景重复（Background Repeat）</h4>
<p>使用 <code>background-repeat</code> 属性可以控制背景图像的重复方式。例如：</p>
<pre><code>div {
  background-repeat: repeat-x; /* 水平重复*/
}
</code></pre>
<h4 id='背景附着background-attachment）'>背景附着（Background Attachment）</h4>
<p>通过 <code>background-attachment</code> 属性，你可以设置背景图像是随着页面滚动还是固定在一个位置。例如：</p>
<pre><code>div {
  background-attachment: fixed;
}
</code></pre>
<h4 id='线性渐变linear-gradient）'>线性渐变（Linear Gradient）</h4>
<p>使用 <code>linear-gradient</code> 属性，你可以创建线性渐变的背景。例如：</p>
<pre><code>div {
  background: linear-gradient(to right, #ff0000, #00ff00);
}
</code></pre>
<h2 id='伪类pseudo-classes）-2'>伪类（Pseudo-classes）</h2>
<h4 id='悬停状态hover）'>悬停状态（:hover）</h4>
<p><code>:hover</code> 伪类用于在用户悬停在元素上时应用样式。例如：</p>
<pre><code>a:hover {
  color: #ff0000;
}
</code></pre>
<h4 id='激活状态active）'>激活状态（:active）</h4>
<p><code>:active</code> 伪类用于在用户点击并按住鼠标按钮时应用样式。例如：</p>
<pre><code>button:active {
  background-color: #00ff00;
}
</code></pre>
<p>这些是CSS中一些常见的图像和背景处理技术，以及一些常用的伪类，它们有助于创建吸引人的界面和交互效果。</p>
<h2 id='补充和进阶'>补充和进阶</h2>
<h2 id='伪类'>伪类</h2>
<p>在CSS（层叠样式表）中，伪类（pseudo-class）是一种用于选择元素的特殊选择器。伪类不是实际存在于文档中的元素，而是表示元素的特定状态或位置关系。它们允许你选择不同状态下的元素，而无需修改HTML结构。</p>
<p>以下是一些常见的CSS伪类：</p>
<ol start='' >
<li><p><strong>:hover</strong> - 鼠标悬停在元素上时应用的样式。</p>
<pre><code>a:hover {
  color: red;
}
</code></pre>
</li>
<li><p><strong>:active</strong> - 用户点击元素但尚未释放鼠标按钮时应用的样式。</p>
<pre><code>button:active {
  background-color: yellow;
}
</code></pre>
</li>
<li><p><strong>:focus</strong> - 元素获得焦点时应用的样式，通常用于表单元素。</p>
<pre><code>input:focus {
  border: 2px solid blue;
}
</code></pre>
</li>
<li><p><strong>:first-child</strong> - 选择元素的第一个子元素。</p>
<pre><code>li:first-child {
  font-weight: bold;
}
</code></pre>
</li>
<li><p><strong>:last-child</strong> - 选择元素的最后一个子元素。</p>
<pre><code>div p:last-child {
  margin-bottom: 0;
}
</code></pre>
</li>
<li><p><strong>:nth-child(n)</strong> - 选择元素的第 n 个子元素。</p>
<pre><code>li:nth-child(odd) {
  background-color: lightgray;
}
</code></pre>
<p>在这个例子中，奇数位置的 <code>li</code> 元素会有灰色背景。</p>
</li>
<li><p><strong>:nth-of-type(n)</strong> - 选择相同类型的元素中的第 n 个元素。</p>
<pre><code>p:nth-of-type(2) {
  color: red;
}
</code></pre>
<p>在这个例子中，文档中的第二个 <code>p</code> 元素文本颜色会变为红色。</p>
</li>

</ol>
<p>这些只是一些常见的伪类，还有其他伪类可用于更复杂的选择。伪类是CSS中强大而灵活的工具，它们使得可以根据元素的状态或位置更精确地选择和样式化元素。</p>
<p>CSS伪类可以分为几个不同类型，其中之一是“状态型”伪类。这些伪类基于元素的状态或用户与元素的交互来选择元素。以下是一些常见的状态型伪类：</p>
<ol start='' >
<li><p><strong>:hover</strong>：当用户将鼠标悬停在元素上时应用的样式。常用于创建交互式效果，例如按钮在鼠标悬停时改变颜色。</p>
<pre><code>button:hover {
  background-color: #3498db;
  color: #fff;
}
</code></pre>
</li>
<li><p><strong>:active</strong>：当元素处于活动（被点击但尚未释放）状态时应用的样式。通常用于创建按钮被点击时的样式。</p>
<pre><code>button:active {
  background-color: #e74c3c;
  color: #fff;
}
</code></pre>
</li>
<li><p><strong>:focus</strong>：当元素获得焦点时应用的样式。常用于增强表单元素的可访问性，使用户知道当前哪个输入字段处于焦点状态。</p>
<pre><code>input:focus {
  border: 2px solid #3498db;
}
</code></pre>
</li>
<li><p><strong>:visited</strong>：选择已被访问的链接。这使得可以为已访问和未访问的链接应用不同的样式。</p>
<pre><code>a:visited {
  color: purple;
}
</code></pre>
</li>
<li><p><strong>:link</strong> 和 <strong>:visited</strong>：分别选择未被访问的链接和已被访问的链接。这两者通常与<code>:hover</code>和<code>:active</code>一起使用，以创建链接的完整状态样式。</p>
<pre><code>a:link {
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
</code></pre>
</li>

</ol>
<p>这些状态型伪类允许你根据用户的交互或元素的状态动态地应用样式，以改变页面的外观和行为。</p>
<ol start='' >
<li><p><strong>:hover</strong>：</p>
<ul>
<li>描述：当用户将鼠标悬停在元素上时应用的样式。</li>
<li>用例：用于创建交互式效果，例如在悬停时改变链接或按钮的颜色。</li>

</ul>
<pre><code>button:hover {
  background-color: #3498db;
  color: #fff;
}
</code></pre>
</li>
<li><p><strong>:active</strong>：</p>
<ul>
<li>描述：当元素处于活动状态（被点击但尚未释放）时应用的样式。</li>
<li>用例：用于创建按钮被点击时的样式。</li>

</ul>
<pre><code>button:active {
  background-color: #e74c3c;
  color: #fff;
}
</code></pre>
</li>
<li><p><strong>:focus</strong>：</p>
<ul>
<li>描述：当元素获得焦点时应用的样式。通常用于增强表单元素的可访问性。</li>
<li>用例：用于突出当前输入字段。</li>

</ul>
<pre><code>input:focus {
  border: 2px solid #3498db;
}
</code></pre>
</li>
<li><p><strong>:visited</strong>：</p>
<ul>
<li>描述：选择已被访问的链接。</li>
<li>用例：用于为已访问和未访问的链接应用不同的样式。</li>

</ul>
<pre><code>a:visited {
  color: purple;
}
</code></pre>
</li>
<li><p><strong>:checked</strong>：</p>
<ul>
<li>描述：选择被选中的表单元素，如复选框或单选按钮。</li>
<li>用例：用于在选择某个选项时应用样式。</li>

</ul>
<pre><code>input[type=&quot;checkbox&quot;]:checked {
  background-color: #2ecc71;
}
</code></pre>
</li>
<li><p><strong>:enabled</strong>：</p>
<ul>
<li>描述：选择处于启用状态的表单元素。</li>
<li>用例：用于在表单元素启用时应用样式。</li>

</ul>
<pre><code>input:enabled {
  border: 1px solid #3498db;
}
</code></pre>
</li>
<li><p><strong>:disabled</strong>：</p>
<ul>
<li>描述：选择处于禁用状态的表单元素。</li>
<li>用例：用于在表单元素禁用时应用样式。</li>

</ul>
<pre><code>input:disabled {
  background-color: #ecf0f1;
}
</code></pre>
</li>

</ol>
<p>这些伪类使得可以根据元素的状态或用户与元素的交互来动态地应用样式，从而增加页面的交互性和可访问性。</p>
<ol start='' >
<li><p><strong>::before</strong>：</p>
<ul>
<li>描述：在元素的内容之前插入生成的内容。</li>
<li>用例：用于在元素前面添加装饰性内容，例如图标或引用符号。</li>

</ul>
<pre><code>p::before {
  content: &quot;\201C&quot;; /*左双引号*/
}
</code></pre>
</li>
<li><p><strong>::after</strong>：</p>
<ul>
<li>描述：在元素的内容之后插入生成的内容。</li>
<li>用例：用于在元素后面添加额外的内容，比如清除浮动或添加尾随图标。</li>

</ul>
<pre><code>p::after {
  content: &quot;\201D&quot;; /*右双引号*/
}
</code></pre>
</li>
<li><p><strong>::first-line</strong>：</p>
<ul>
<li>描述：选择元素的第一行并应用样式。</li>
<li>用例：用于改变段落的首行样式，如字体大小或颜色。</li>

</ul>
<pre><code>p::first-line {
  font-weight: bold;
}
</code></pre>
</li>
<li><p><strong>::first-letter</strong>：</p>
<ul>
<li>描述：选择元素的第一个字母并应用样式。</li>
<li>用例：用于创建首字母大写或添加特殊样式的效果。</li>

</ul>
<pre><code>p::first-letter {
  font-size: 1.5em;
  color: #3498db;
}
</code></pre>
</li>
<li><p><strong>::selection</strong>：</p>
<ul>
<li>描述：选择用户选择的文本部分并应用样式。</li>
<li>用例：用于自定义用户选择文本时的背景和文本颜色。</li>

</ul>
<pre><code>::selection {
  background-color: #3498db;
  color: #fff;
}
</code></pre>
</li>

</ol>
<p>这些伪元素允许你选择元素的特定部分并对其应用样式，从而提供更多样式化的可能性。每个伪元素都有其独特的应用场景和效果。</p>
<h2 id='transform'>Transform</h2>
<p>在CSS中，<code>transform</code>属性用于对元素进行平移（translate）、缩放（scale）、旋转（rotate）、扭曲（skew）和透视（perspective）等变换操作。这些变换可以单独应用或组合在一起，以创建各种视觉效果。下面是对每个变换的简要说明：</p>
<ol start='' >
<li><p><strong>平移（Translate）</strong>：</p>
<ul>
<li>描述：通过指定元素在水平和垂直方向上的偏移来移动元素。</li>
<li>语法：<code>translate(x, y)</code>，其中 <code>x</code> 和 <code>y</code> 分别是水平和垂直方向上的偏移值。</li>

</ul>
<pre><code>.box {
  transform: translate(50px, 20px);
}
</code></pre>
</li>
<li><p><strong>缩放（Scale）</strong>：</p>
<ul>
<li>描述：通过指定元素在水平和垂直方向上的缩放比例来调整元素的大小。</li>
<li>语法：<code>scale(x, y)</code>，其中 <code>x</code> 和 <code>y</code> 分别是水平和垂直方向上的缩放比例。</li>

</ul>
<pre><code>.box {
  transform: scale(1.5, 2);
}
</code></pre>
</li>
<li><p><strong>旋转（Rotate）</strong>：</p>
<ul>
<li>描述：通过指定元素的旋转角度来旋转元素。</li>
<li>语法：<code>rotate(angle)</code>，其中 <code>angle</code> 是旋转的角度。</li>

</ul>
<pre><code>.box {
  transform: rotate(45deg);
}
</code></pre>
</li>
<li><p><strong>扭曲（Skew）</strong>：</p>
<ul>
<li>描述：通过指定元素在水平和垂直方向上的倾斜角度来扭曲元素。</li>
<li>语法：<code>skew(x-angle, y-angle)</code>，其中 <code>x-angle</code> 和 <code>y-angle</code> 分别是水平和垂直方向上的倾斜角度。</li>

</ul>
<pre><code>.box {
  transform: skew(30deg, 20deg);
}
</code></pre>
</li>
<li><p><strong>透视（Perspective）</strong>：</p>
<ul>
<li>描述：通过指定透视距离来创建透视效果，影响 3D 变换的效果。</li>
<li>语法：<code>perspective(length)</code>，其中 <code>length</code> 是透视距离。</li>

</ul>
<pre><code>.container {
  perspective: 1000px;
}
</code></pre>
</li>

</ol>
<p>这些变换可以单独使用，也可以组合在一起。例如，可以在一个规则中同时使用 <code>translate</code>、<code>rotate</code> 和 <code>scale</code> 来实现多个变换效果。CSS变换为Web开发者提供了强大的工具，用于实现各种交互和动画效果。</p>
<h4 id='transision'>Transision</h4>
<p>在CSS中，<code>transition</code>是一种用于在元素状态发生变化时平滑过渡效果的属性。通过使用<code>transition</code>属性，可以定义元素的属性在发生变化时应用过渡效果，而不是突然改变。</p>
<p><code>transition</code>属性通常与伪类（例如<code>:hover</code>）一起使用，以在元素状态变化时提供平滑的过渡。以下是<code>transition</code>属性的基本语法：</p>
<pre><code>selector {
  transition: property duration timing-function delay;
}
</code></pre>
<ul>
<li><code>property</code>：要过渡的CSS属性，如<code>color</code>、<code>opacity</code>、<code>transform</code>等。</li>
<li><code>duration</code>：过渡的持续时间，以秒（s）或毫秒（ms）为单位。</li>
<li><code>timing-function</code>：过渡的时间函数，控制过渡的速度曲线（例如线性、ease-in、ease-out等）。</li>
<li><code>delay</code>：过渡开始之前的延迟时间，以秒（s）或毫秒（ms）为单位。</li>

</ul>
<p>以下是一个简单的示例，演示了当鼠标悬停在一个按钮上时，背景颜色会平滑过渡变化：</p>
<pre><code>button {
  background-color: #3498db;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #e74c3c;
}
</code></pre>
<p>在这个例子中，当鼠标悬停在按钮上时，<code>background-color</code>属性将以<code>ease</code>的时间函数在0.3秒内从蓝色平滑过渡到红色。</p>
<p>通过使用<code>transition</code>属性，可以增强用户体验，使页面元素状态变化更加流畅和自然。此属性广泛用于实现按钮、链接和其他用户界面元素的动画效果。</p>
<h2 id='动画'>动画</h2>
<p>在CSS中，<code>@keyframes</code> 和 <code>animation</code> 属性用于创建和应用动画。<code>@keyframes</code>规则定义动画的关键帧，而 <code>animation</code> 属性用于指定动画的名称、持续时间、时间函数、延迟、迭代次数、方向和填充模式等。</p>
<h3 id='keyframes-规则'>@keyframes 规则</h3>
<p><code>@keyframes</code> 规则用于定义动画的关键帧，即在动画过程中的不同阶段。它的基本语法如下：</p>
<pre><code>@keyframes animationName {
  from {
    /*styles at the beginning of the animation*/
  }

  to {
    /*styles at the end of the animation*/
  }

  /*or use percentage for intermediate keyframes */
  25% {
    /* styles at 25% of the animation*/
  }

  /*additional keyframes as needed*/
}
</code></pre>
<h3 id='animation-属性'>animation 属性</h3>
<p><code>animation</code> 属性用于将动画应用于元素。其基本语法如下：</p>
<pre><code>selector {
  animation: name duration timing-function delay iteration-count direction fill-mode;
}
</code></pre>
<ul>
<li><code>name</code>：指定要应用的 <code>@keyframes</code> 规则的名称。</li>
<li><code>duration</code>：动画的持续时间，以秒（s）或毫秒（ms）为单位。</li>
<li><code>timing-function</code>：动画的时间函数，控制动画的速度曲线（例如 <code>ease</code>、<code>linear</code>、<code>ease-in</code> 等）。</li>
<li><code>delay</code>：动画开始前的延迟时间，以秒（s）或毫秒（ms）为单位。</li>
<li><code>iteration-count</code>：动画的迭代次数，可以是具体次数或 <code>infinite</code> 表示无限次。</li>
<li><code>direction</code>：动画的播放方向，可以是 <code>normal</code>（正常播放）、<code>reverse</code>（反向播放）、<code>alternate</code>（交替正反播放）等。</li>
<li><code>fill-mode</code>：动画执行前和执行后的样式，可以是 <code>forwards</code>、<code>backwards</code>、<code>both</code> 或 <code>none</code>。</li>

</ul>
<p>以下是一个简单的例子，演示了一个使用 <code>@keyframes</code> 和 <code>animation</code> 属性的动画：</p>
<pre><code>@keyframes slide-in {
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
</code></pre>
<p>在这个例子中，一个名为 <code>slide-in</code> 的关键帧规则定义了一个元素从左侧滑入的动画，然后通过 <code>.slide-in</code> 类将这个动画应用到特定的元素上。</p>
<h2 id='字库'>字库</h2>
<pre><code>@font-face {
  font-family: fnt;
  src: url(../remixicon.woff) format(&quot;woff&quot;);
}
</code></pre>
<ul>
<li><code>@font-face</code> 规则是用于定义字体的规则，使得你可以使用自定义字体。</li>
<li><code>font-family</code> 属性定义了字体的名称，这个名称可以在后续的 CSS 规则中使用。</li>
<li><code>src</code> 属性指定了字体文件的路径和格式。在这个例子中，字体文件是 <code>remixicon.woff</code>，它使用 WOFF 格式（Web Open Font Format）。</li>

</ul>
<p>然后，你可以在其他地方的样式规则中使用 <code>font-family: fnt;</code> 来引用这个自定义字体，例如：</p>
<pre><code>body {
  font-family: fnt, sans-serif;
}
</code></pre>
<p>这会将 <code>fnt</code> 字体应用于页面的主体文本，如果字体不可用，那么将回退到系统默认的 sans-serif 字体。</p>
<h2 id='css-结构规划'>CSS 结构规划</h2>
<p>CSS的结构规划对于项目的可维护性和团队协作至关重要。以下是一些关于引入方式、作用域和团队协作的考虑：</p>
<h3 id='引入方式'>引入方式</h3>
<ol start='' >
<li><p><strong>内联样式（Inline Styles）：</strong></p>
<ul>
<li><strong>语法：</strong> <code>style=&quot;...&quot;</code>。</li>
<li><strong>特点：</strong> 样式与HTML元素直接关联，不推荐在大型项目中使用，因为难以维护。</li>

</ul>
<pre><code>html
&lt;p style=&quot;color: red; font-size: 16px;&quot;&gt;This is a paragraph.&lt;/p&gt;
</code></pre>
</li>
<li><p><strong>嵌入样式（Embedded Styles）：</strong></p>
<ul>
<li><strong>语法：</strong> <code>&lt;style&gt;...&lt;/style&gt;</code>。</li>
<li><strong>特点：</strong> 样式写在HTML文档的头部，适用于小型项目或需要页面特定样式的情况。</li>

</ul>
<pre><code>html&lt;head&gt;
  &lt;style&gt;
    p {
      color: blue;
      font-size: 18px;
    }
  &lt;/style&gt;
&lt;/head&gt;
</code></pre>
</li>
<li><p><strong>外部样式表（External Stylesheet）：</strong></p>
<ul>
<li><strong>语法：</strong> <code>&lt;link rel=&quot;stylesheet&quot; type=&quot;text/css&quot; href=&quot;style.css&quot;&gt;</code>。</li>
<li><strong>特点：</strong> 样式定义在独立的CSS文件中，适用于大型项目和样式共享。</li>

</ul>
<pre><code>html&lt;head&gt;
  &lt;link rel=&quot;stylesheet&quot; type=&quot;text/css&quot; href=&quot;style.css&quot;&gt;
&lt;/head&gt;
</code></pre>
</li>

</ol>
<h3 id='作用域'>作用域</h3>
<ol start='' >
<li><p><strong>类选择器 <code>.class</code> vs ID 选择器 <code>#id</code> vs 属性选择器 <code>[...]</code>：</strong></p>
<ul>
<li><strong>类选择器：</strong> 适用于多个元素共享相似样式的情况。</li>
<li><strong>ID 选择器：</strong> 应该避免过度使用，因为ID在整个页面中是唯一的，可能导致样式不可复用，容易发生命名冲突。</li>
<li><strong>属性选择器：</strong> 适用于根据元素的属性选择样式，例如 <code>[disabled]</code>。</li>

</ul>
<pre><code>.highlight {
  color: red;
}

# header {
  font-size: 20px;
}

[disabled] {
  opacity: 0.5;
}
</code></pre>
</li>
<li><p><strong>路径限制作用域：</strong></p>
<ul>
<li>通过合理的CSS选择器路径，限制样式的作用域，避免全局定义。</li>
<li>避免过于宽泛的选择器，以免影响到其他模块的样式。</li>

</ul>
<pre><code>.section1 .content {
  /*样式规则*/
}
</code></pre>
</li>

</ol>
<h3 id='团队协作'>团队协作</h3>
<ol start='' >
<li><p><strong>规范和命名约定：</strong></p>
<ul>
<li>制定明确的CSS规范和命名约定，确保团队成员有一致的样式书写风格。</li>
<li>使用有意义的类名和ID，避免单个字母或缩写，提高代码可读性。</li>

</ul>
</li>
<li><p><strong>模块化和组件化：</strong></p>
<ul>
<li>将样式分为模块或组件，使其易于维护和复用。</li>
<li>可以考虑使用CSS预处理器（如Sass或Less）来实现模块化。</li>

</ul>
</li>
<li><p><strong>版本控制：</strong></p>
<ul>
<li>使用版本控制系统（如Git）管理样式表，确保团队成员能够协同工作并追踪变更历史。</li>

</ul>
</li>
<li><p><strong>代码审查：</strong></p>
<ul>
<li>定期进行代码审查，确保符合团队规范，并且样式表的结构清晰、合理。</li>

</ul>
</li>
<li><p><strong>文档和注释：</strong></p>
<ul>
<li>添加注释和文档，解释样式表的结构、作用和用法，方便团队成员理解和使用。</li>

</ul>
</li>

</ol>
<p>综合考虑引入方式、作用域和团队协作，可以建立一个清晰、可维护且协作良好的CSS结构，提高项目的开发效率和代码质量。</p>
<h2 id='css-浏览器私有前缀'>CSS 浏览器私有前缀</h2>
<p>浏览器私有前缀是为了兼容不同浏览器的特定CSS属性和规则。不同浏览器厂商在实现新的CSS属性或规则时可能存在一些差异，为了确保网页在不同浏览器中都能正常显示，开发者可以使用浏览器私有前缀。以下是一些主要浏览器的私有前缀：</p>
<ul>
<li><p><strong>WebKit（Chrome、Safari）:</strong></p>
<ul>
<li><code>-webkit-</code></li>

</ul>
</li>
<li><p><strong>Mozilla Firefox:</strong></p>
<ul>
<li><code>-moz-</code></li>

</ul>
</li>
<li><p><strong>Internet Explorer:</strong></p>
<ul>
<li><code>-ms-</code></li>

</ul>
</li>
<li><p><strong>Opera:</strong></p>
<ul>
<li><code>-o-</code></li>

</ul>
</li>

</ul>
<h3 id='css浏览器版本兼容方式'>CSS浏览器版本兼容方式</h3>
<p>在写CSS样式时，通常会使用带有浏览器私有前缀的规则，以确保在各种浏览器中都能正确渲染。一种通用的方式是使用带前缀和不带前缀的规则，例如：</p>
<pre><code>.transition {
  -webkit-transition: all .5s; /*Chrome, Safari */
  -moz-transition: all .5s;    /* Firefox */
  -o-transition: all .5s;      /* Opera */
  transition: all .5s;         /* Standard*/
}
</code></pre>
<p>在这个例子中，<code>.transition</code> 类使用了带有不同私有前缀和不带前缀的 <code>transition</code> 属性。浏览器会选择解析符合其规范的属性，并忽略不认识的属性。这样，无论用户使用哪种浏览器，都能保证过渡效果的兼容性。当浏览器逐渐支持标准的写法时，可以逐步去掉私有前缀。</p>
</body>
