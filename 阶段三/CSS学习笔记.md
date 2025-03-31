

# CSS 学习笔记

**css全名是cascading style sheets，意为层叠样式表，用于定义网页样式和布局的样式表语言。通过css可以指定页面中各个元素的颜色、字体、大小、间距、边框、背景等样式，从而实现更精确的页面设计。**

---

使用CSS是为了：

* 实现内容与样式的分离，便于团队的开发
* 样式复用，便于网站的后期维护
* 页面的精准控制，让页面更精美

---

## 基本语法

css由选择器以及一条或多条声明组成

选择器通常是需要改变样式的 HTML 元素。每条声明由一个属性和一个值组成。

属性是您希望设置的样式属性。每个属性有一个值。属性和值被冒号分开

选择器的声明可以写无数条属性

声明的每一行属性，都要以英文分号结尾

<head>
	<style>
		选择器{
			属性名：属性值;
			属性名：属性值;
		}
	</style>
</head>

---

## CSS应用方式

也称为CSS引用方式，有三种方式：

内部样式、行内样式、外部样式

1. **内部样式**
   也称为内嵌样式，在页面头部通过style标签定义

   对当前页面中所有符合样式选择器的标签都起作用

2. **行内样式**
   也称为嵌入样式，使用HTML标签的style属性定义

   只对设置style属性的标签起作用

3. 外部样式
   使用单独的 .CSS 文件定义，然后在页面中使用 link标签 或 @import指令 引入

---

## 选择器

* ### 类选择器

用于描述一组元素的样式

类选择器以一个点 **.** 号显示

.center {text-align:center;}

*  ### 元素选择器

选择并设置所有

元素的样式：

```
p
{ 
background-color:yellow;
}
```



* ### id 选择器

  可以为标有特定 id 的 HTML 元素指定特定的样式，id 选择器以 "#" 来定义。

\#para1 { text-align:center; color:red; }

* ### 通用选择器

选择所有元素，并设置它们的背景色：

```
*
{ 
background-color:yellow;
}
```

**优先级：id > 类 > 元素 > 通用**

---

#### 设置元素基础样式  
通过 CSS 属性控制元素的视觉表现：  
- **大小**：`width`、`height`（如 `div { width: 200px; }`）  
- **颜色**：`color`（文字颜色）、`background-color`（背景颜色）
- **字体**：`font-family`（字体类型）、`font-size`（字号）  
- **其他**：`border`（边框）、`padding`（内边距）、`margin`（外边距）

---

### 盒子模型

- **Margin(外边距)** - 清除边框外的区域，外边距是透明的。
- **Border(边框)** - 围绕在内边距和内容外的边框。
- **Padding(内边距)** - 清除内容周围的区域，内边距是透明的。
- **Content(内容)** - 盒子的内容，显示文本和图像。

![](https://pic4.zhimg.com/v2-1c7edd49c7111272bb68402ecd202812_r.jpg)



#### outline

| 属性                                                         | 说明                           | 值                                                           |
| ------------------------------------------------------------ | ------------------------------ | ------------------------------------------------------------ |
| [outline](https://www.runoob.com/cssref/pr-outline.html)     | 在一个声明中设置所有的轮廓属性 | *outline-color outline-style outline-width *inherit          |
| [outline-color](https://www.runoob.com/cssref/pr-outline-color.html) | 设置轮廓的颜色                 | *color-name hex-number rgb-number *invert inherit            |
| [outline-style](https://www.runoob.com/cssref/pr-outline-style.html) | 设置轮廓的样式                 | none dotted dashed solid double groove ridge inset outset inherit |
| [outline-width](https://www.runoob.com/cssref/pr-outline-width.html) | 设置轮廓的宽度                 | thin medium thick *length *inherit                           |

#### border-style值

none: 默认无边框

dotted: 定义一个点线边框

dashed: 定义一个虚线边框

solid: 定义实线边框

double: 定义两个边框。 两个边框的宽度和 border-width 的值相同

groove: 定义3D沟槽边框。效果取决于边框的颜色值

ridge: 定义3D脊边框。效果取决于边框的颜色值

inset:定义一个3D的嵌入边框。效果取决于边框的颜色值

outset: 定义一个3D突出边框。 效果取决于边框的颜色值



**盒模型类型**：  

- 标准盒模型：`width` 仅指内容宽度（默认）。  
- IE 盒模型：`width` 包含内容、内边距和边框（通过 `box-sizing: border-box` 设置）。

---

#### **CSS 的 5 种 Position 定位**  
- **`static`**：默认定位，元素按文档流排列。 
- **`relative`**：相对自身原始位置偏移（通过 `top`、`left` 调整），不脱离文档流。 
- **`absolute`**：相对于最近的非 `static` 父元素定位，脱离文档流。 
- **`fixed`**：相对于视口定位（如固定导航栏），脱离文档流 
- **`sticky`**：结合 `relative` 和 `fixed`，滚动到阈值后固定 CSS 常用布局方式 

---

#### CSS常用布局方式

- **浮动布局**：通过 `float` 实现元素横向排列（需清除浮动）  
- **Flexbox**：弹性盒子布局，适合一维排列（通过 `display: flex` 启用）  
- **Grid**：网格布局，适合复杂二维布局（通过 `display: grid` 启用）  
- **响应式布局**：使用媒体查询（`@media`）适配不同屏幕尺寸

---

#### CSS 伪类
伪类用于定义元素的特殊状态或位置：  
- **`:hover`**：鼠标悬停时的样式。  
- **`:active`**：元素被激活（如点击）时的样式。  
- **`:nth-child(n)`**：匹配第 n 个子元素（如隔行换色）。  
- **`:focus`**：元素获取焦点时的样式（如表单输入框）。

