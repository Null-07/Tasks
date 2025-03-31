# JavaScript学习笔记

***这是一种轻量级、解释型、面向对象的脚本语言，主要被设计用于在网页上实现动态效果***

---

### 作用

* 客户端脚本：用于在用户浏览器中执行，实现动态效果和用户交互。
* 网页开发：与HTML和CSS协同工作，使得网页有更强的交互性和动态性。
* 后端开发：使用Node.js, JavaScript 也可以在服务器端运行，实现服务器端应用的开发。

---

#### 基本语法

* **标识符**

  所谓标识符，就是指给变量、函数、属性或函数的参数起名字。

  标识符可以是按照下列格式规则组合起来的一或多个字符：

  * 第一个字符必须是一个字母、下划线（ _ ）或一个美元符号（ $ ）
  * 其它字符可以是字母、下划线、美元符号或数字。
  * 标识符不能是关键字和保留字符。

* **关键字**

  |  break   |   do    | instanceof | typeof |  case   |
  | :------: | :-----: | :--------: | :----: | :-----: |
  |   else   |   new   |    var     | catch  | finally |
  |  return  |  void   |  continue  |  for   | switch  |
  |  while   | default |     if     | throw  | delete  |
  |    in    |   try   |  function  |  this  |  with   |
  | debugger |  false  |    true    |  null  |         |

* **保留字符**

  |   class   |    enum    |  extends  |  super  | const  | export |
  | :-------: | :--------: | :-------: | :-----: | :----: | :----: |
  |  import   | implements |    let    | private | public | yield  |
  | interface |  package   | protected | static  |        |        |

* **常量**

##### 数字常量

729   8.07

**字符串常量**

可以使用单引号或双引号

"Cindy"

##### 表达式常量

8 + 7

##### 数组常量

[40, 100, 1, 5, 25, 10]

##### 函数常量



* **变量**

使用关键字 **var** 来定义变量， 使用等号来为变量赋值

var x, length

x = 5

length = 6

---

#### 数据类型

**值类型(基本类型)**：字符串（String）、数字(Number)、布尔(Boolean)、空（Null）、未定义（Undefined）、Symbol

**引用数据类型（对象类型）**：对象(Object)、数组(Array)、函数(Function)

JavaScript 拥有动态类型。这意味着相同的变量可用作不同的类型：

var x; // x 为 undefined

var x = 5; // 现在 x 为数字

var x = "John"; // 现在 x 为字符串

* **字符串**

  储存字符的变量

  var carname="Volvo XC60"; var carname='Volvo XC60';

* **数字**

  var x1=34.00; //使用小数点来写 var x2=34; //不使用小数点来写

* **布尔**

  布尔（逻辑）只能有两个值：true 或 false

  var x=true; var y=false;

* **数组**
  下面的代码创建名为 cars 的数组：
  var cars=new Array(); cars[0]="Saab"; cars[1]="Volvo"; cars[2]="BMW";

* **对象**
  var person={firstname:"John", lastname:"Doe", id:5566};

* **Undefined 和 Null**

  Undefined 这个值表示变量不含有值

  可以通过将变量的值设置为 null 来清空变量

---

### HTML / CSS / JavaScript 三者之间的关系

与HTML和CSS不同，JavaScript 使得网页不再是静态的，而是可以根据用户的操作动态变化的。

简单一点来所的话就是：

HTML：决定了网页有什么内容
CSS：决定了网页长什么样
JavaScript：决定了网页能做什么

---



