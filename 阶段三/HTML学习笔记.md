# HTML学习笔记

**HTML(HyperText Markup Language)是用来描述网页的一种语言，是一种在Web上使用的通用标记语言。HTML允许你格式化文本，添加图片，创建链接，输入表单、框架和表格等等，并可将之存为文本文件，浏览器即可读取与显示。**

---

* HTML 不是一种编程语言，而是一种标记语言
* 标记语言是一套**标记标签**(markup tag)
* HTML 使用标记标签来**描述**网页
* HTML 文档包含了HTML **标签**及**文本**内容
* HTML 文档也叫作 **web**页面

---

#### HTML 语法规范

1. HTML 标签是由尖括号包围的关键字，比如<html>
2. HTML 标签通常是成对出现的，由一个开始标签和一个结束标签组成，也就是双标签，比如<html></html>
3. 有些特殊的标签必须是单个标签，也就是单标签，比如<br/>
4. 双标签可以分为两类：包含关系和并列关系

#### 包含关系

```
<head>
  <title></title>
</head>
```

#### 并列关系

```
<head></head>
<body></body>
```





































































html全称是hypertext markup language（超文本标记语言），通过一系列的标签来定义文本、图像、链接等等，HTML标签是由尖括号包围的关键字。

HTML属性

他们定义元素的行为和外观，以及与其他元素的关系

基本语法：<开始标签 属性名=“属性值”>

属性名称不区分大小写，属性值对大小写敏感

标签通常成对出现，包括开始标签和结束标签，内容位于这两个标签之间

<p>这是一个段落。</p>

<h1>这是一个标题。</h1>

<a href="#">这是一个超链接。</a>

除了双标签，也有单标签

<input type="text"> <br> <hr>

这两个的区别是，单标签用于没有内容的元素，双标签用于有内容的元素。

标题标签

<h1>一级标题标签</h1>

<h2>二级标题标签</h2>

<h6>六级标题标签</h6>

段落标签

<p>一个段落标签</p>

文本标签

<p>更改文本样式：<b>字体加粗</b>、<l>斜体</l>、<u>下划线</u>、<s>删除线</s></p>

换行标签<br></br>

水平分割线<hr></hr>

<a></a>

创建链接到其他的网页或位置

href属性定义了链接到的目标

target属性定义链接的打开方式

无序列表

<ul>

<li>无序列表元素1</li>

<li>无序列表元素2</li>

<li>无序列表元素3</li>

</ul>

有序列表

<ol>

<li>有序列表元素1</li>

<li>有序列表元素2</li>

<li>有序列表元素3</li>

</ol>

<div>标签

导航栏

<div class="nav">

<a href="#">链接1</a>

<a href="#">链接2</a>

<a href="#">链接3</a>

内容部分

</div>

<div class="contentv">

<h1>文章标题</h1>

<p>文章内容</p>

</div>

块元素与行内元素

块元素（block）

用于组织和布局页面的主要结构和内容，例如段落、标题、列表、表格等，用于创建页面的主要部分，将内容分隔成逻辑块

通常从新行开始，并占据整行的宽度

可以包含其他块级元素和行内元素

常见的有<div><p><h1><table><form>等

行内元素（inline）

通常用于添加文本样式或为文本中的一部分应用样式，可以在文本中插入小的元素，如超链接、强调文本等。

通常在同一行内呈现，不会独占一行。

只占据其内容所需的宽度，而不是整行的宽度。

不能包含块级元素，但可以包含其他行内元素。

常见的有<span><a><strong><img>

html样式

background-color 属性为元素定义了背景颜色

```
<body style="background-color:yellow">
<h2 style="background-color:red">This is a heading</h2>
<p style="background-color:green">This is a paragraph.</p>
```



font-family、color 以及 font-size 属性分别定义元素中文本的字体系列、颜色和字体尺寸

```
<h1 style="font-family:verdana">A heading</h1>
<p style="font-family:arial;color:red;font-size:20px;">A paragraph.</p>
```

