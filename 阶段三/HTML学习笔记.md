





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

#### 结构标签

| 标签名 |    定义    | 作用                                           |
| :----: | :--------: | :--------------------------------------------- |
|  html  |  HTML标签  | 页面中最大的标签，常称为根标签                 |
|  head  | 文档的头部 | 注意在head标签中我们必须设置title标签          |
| title  | 文档的标题 | 页面的网页标题                                 |
|  body  | 文档的主体 | 包含文档的所有内容，页面的内容都要卸载body里面 |

---

HTML属性 他们定义元素的行为和外观，以及与其他元素的关系

基本语法：<开始标签 属性名=“属性值”> 

属性名称不区分大小写，属性值对大小写敏感

标签通常成对出现，包括开始标签和结束标签，内容位于这两个标签之间



**在vscode中打开 .html 文件，！+ 回车 可以直接弹出 HTML基本结构**

![](https://github.com/Null-07/Photos/blob/main/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-03-31%20001859.png?raw=true)

---

#### 常用文本标签

<p>这是一个段落标签</p>

<h1>一级标题标签</h1>

<h2>二级标题标签</h2>

<h3>三级标题标签</h3>

<p>更改文本样式：<b>字体加粗</b>、<i>斜体</i>、<u>下划线</u>、<s>删除线</s></p>

<a href="https://docs.geeksman.com">这是一个超链接</a>

换行标签<br></br>水平分割线<hr></hr>

 <a></a>

创建链接到其他的网页或位置

href属性定义了链接到的目标

target属性定义链接的打开方式

**无序列表**

<ul>	

​	<li>无序列表元素1</li> 

​	<li>无序列表元素2</li>

​	<li>无序列表元素3</li> 



**有序列表**

<ol>     

​	<li>有序列表元素1</li>

​	<li>有序列表元素2</li>

​	<li>有序列表元素3</li>

**列表**

<table border="1">
    <tr>
        <th>列标题1</th>
        <th>列标题2</th>
        <th>列标题3</th>   
    </tr>
    <tr>
        <td>元素1</td>
        <td>元素2</td>
        <td>元素3</td>
    </tr>
</table>
<div>标签

导航栏

<div class="nav"><a href="#">链接1</a>
<a href="#">链接2</a>

<a href="#">链接3</a>

内容部分

</div><div class="contentv">


<h1>文章标题</h1>

<p>文章内容</p>

</div>

---

## 块元素与行内元素

* 块元素（block）

用于组织和布局页面的主要结构和内容，例如段落、标题、列表、表格等，用于创建页面的主要部分，将内容分隔成逻辑块

通常从新行开始，并占据整行的宽度

可以包含其他块级元素和行内元素

![](https://github.com/Null-07/Photos/blob/main/%E5%9D%97%E5%85%83%E7%B4%A0.png?raw=true)

* 行内元素（inline）

通常用于添加文本样式或为文本中的一部分应用样式，可以在文本中插入小的元素，如超链接、强调文本等。

通常在同一行内呈现，不会独占一行。

只占据其内容所需的宽度，而不是整行的宽度。

不能包含块级元素，但可以包含其他行内元素。

![](https://github.com/Null-07/Photos/blob/main/%E8%A1%8C%E5%86%85%E5%85%83%E7%B4%A0.png?raw=true)

---

### HTML样式标签

<!DOCTYPE html>
<html>
<head>
<title>HTML Style Tag</title>
  <style>
  </style>
</head>
<body>

</body>
</html>

  <div>
      <h1>HTML Style Tag</h1>
  </div>
<style>
   div {
     height: 50px;
     width: 300px;
     background: yellow;
  }
</style>

这样就可以更改背景颜色

