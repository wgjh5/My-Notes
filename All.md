# 基本概念：

1.HTML 指的是超文本标记语言 (Hyper Text Markup Language) 

标记：由一套标签组成的语言 

XHTML指可扩展[超文本](html基础语法.docx)标记语言（标识语言）（EXtensible HyperText Markup Language）。

HTML5指的是HTML的第五次重大修改（第5个版本）

2.HTML发展历史

## ![1531918143197](C:\Users\WANG\AppData\Local\Temp\1531918143197.png)

1. W3C制定的结构和表现的标准 

   W3C( World Wide Web Consortium )万维网联盟，创建于1994年是Web技术领域最具权威和影响力的国际中立性技术标准机构。(制定了结构html和表现css的标准，非赢利性的。)

   WHATWG 浏览器厂商临时组成的组织 

   ECMA：欧洲电脑场商联合会，制定的行为js的标准  

# Web标准 ：

#### 结构：XHTML   表现：css  行为：DOM[ECMAScript]

# 创建站点

#### 1.站点的作用

      用来归纳一个网站上所有的网页、素材以及他们之间的联系

#### 2.创建站点的步骤

site文件夹-html文件夹、css文件夹、js文件夹、images文件夹、index.html（首页入口文件） 

#### 3.文件的命名规则

   (英文开头，可以包含数字、下划线) 

  首页必须命名为index.html，其他页面写在html文件夹里。 

（工具-文件夹选项-查看-隐藏已知文件的扩展名的勾去掉）

# HTML的基本结构

`<!DOCTYPE html>`：声明文档类型

html>head+body

html：说明里面是html文件内容

head：存放页面信息

head>meta+title

meta：元信息节点[字符编码 ：charset   ][国际通用：utf—8 ][国内：gb2312 gbk]

title：页面标题

body：呈现在页面上（书写结构代码）

`<!DOCTYPE html>`

`<html>``

`<head><head>`

`<body><body>`

`</html>` 

![1531963155956](C:\Users\WANG\AppData\Local\Temp\1531963155956.png)	

# sublime的使用

1.菜单---打开文件夹---site文件夹 （site文件夹自行建好：![1531920548133](C:\Users\WANG\AppData\Local\Temp\1531920548133.png)）

2.鼠标移动到指定文件夹（html文件夹）------右键新建文件（后缀.html）

3.快捷键：

​	！+tab快捷生成结构			Ctrl+z返回上一步				标签名+tap快速生成标签

​        Ctrl+s保存					Ctrl+y返回下一步

​	Ctrl+c复制					Ctrl+？生成注释

​	Ctrl+x剪切					f1或f12打开谷歌浏览器

​	Ctrl+v粘贴					f3打开IE浏览器

1. 在浏览器打开控制台的使用：（1）找到指定的元素------右键检查

   ​						 （2）f12------通过左上角鼠标的图标找到指定元素所在的代码行

# html的基本语法

1.html标签：有尖括号包裹起来的整体

2.html元素：由一对双标签或一对单标签组成

3.html属性：

（1）常规标记： <标记 属性=“属性值” 属性=“属性值”></标记>，HTML的属性书写在标签名字的后面，用空格隔开属性或属性值。

（2）空标记 ：<标记 属性=“属性值” /> 

说明：

1.写在<>中的第一个单词叫做标记，标签，元素。

2.标记和属性用空格隔开，属性和属性值用等号连接，属性值必须放在“”号内。

3.一个标记可以没有属性也可以有多个属性，属性和属性之间不分先后顺序。

4.空标记没有结束标签，用“/”代替。

# 标签

#### 1.标题标签：h1----h6（直观上 越来越小，语义上越来越轻，）

<h1>一级标题</h1>-------（最好一个页面只用一次）

<h2>二级标题</h2>

……

<h6>六级标题</h6>

例如：

`<h1><h1>`

<h1><h2>

<h1><h2>

<h1><h2>

<h1><h2>

<h1><h2>

#### 2.段落标签：

<p>段落文本内容</p> 		备注：浏览器解析时会将多个空格及换行解析成一个空格及换行。

#### 3.换行标签：

#### <br /> 4.标识符：

&nbsp； （空格） 	&lt；（小于号）   		&gt；（大于号）

备注：空格的大小不等同于文字的大小，但是受文字大小的影响。

#### 5.加粗标签：

<b>加粗内容</b>    				 视觉标签

<strong>加粗内容</strong>   		 语义标签

#### 6.倾斜标签：

<i></i>   					 视觉标签

<em></em> 				 语义标签

#### 7.分隔线标签：

<hr/>

#### 8.删除线标签：

<s>内容</s>			<del>内容</del>

#### 9.列表标签

（1）无序列表

<ul>：只能嵌套<li>		

<li></li>

<li></li>			

．．．．．．

</ul>	

（2）有序列表

<ol>(ordered list)

<li></li>

<li></li>

．．．．．．

</ol>

（3）自定义列表 

dl>dt（自定义列表项）+dd（对自定义列表项的描述）

<dl>

<dt>文具</dt>

<dd>钢笔</dd>

<dd>橡皮</dd>

<dd>笔记本</dd>

</dl>

（4）图片标签

<img src="E:/H5%E6%AF%8F%E5%A4%A9/%E4%B8%80%E9%98%B6%E6%AE%B5/1/%E7%AC%AC%E4%B8%80%E5%A4%A9%E7%AC%94%E8%AE%B0/%E5%BC%95%E5%85%A5%E5%9B%BE%E7%89%87%E7%9A%84%E8%B7%AF%E5%BE%84" alt="图片无法加载出来显示的文字"/>

相对路径的写法：

1)当当前文件与目标文件在同一目录下，直接书写目标文件文件名+扩展名；

2)当当前文件与目标文件所处的文件夹在同一目录下，写法如下：

文件夹名/目标文件全称+扩展名；

3)当当前文件所处的文件夹和目标文件所处的文件夹在同一目录下，写法如下：

../目标文件所处文件夹名/目标文件文件名+扩展名

#### 10.锚链接标签，超链接标签  a

超链接的应用

语法：

<a href="跳转的路径或者域名">链接文本/图片</a>

例如：<a href="http：www.baidu.com">去百度</a>

属性：target:        		 页面打开方式

默认属性值：_self。	 当前窗口跳转）

属性值：_blank	         新窗口打开 

例如：<a href="http：www.baidu.com" target="_blank">去百度</a>

#### 11.表格标签

table>tr（行）>td（单元格）

作用：显示数据

组成：     <table>

​			<tr>

​				<td></td>

​				<td></td>

​			</tr>

​		</table>

##### 数据表格的相关属性

width="表格的宽度"

height="表格的高度"

border="表格的边框"

bgcolor="表格的背景色"

cellspacing="单元格与单元格之间的间距"

cellpadding="单元格与内容之间的空隙"

水平对齐方式：align="left/center/right";

##### 合并单元格属性：

colspan=“所要合并的单元格的列数"合并列;

rowspan=“所要合并单元格的行数”合并行;

备注：在td里面用。

#### 13.表单的应用

##### 表单的作用：用来收集、验证用户信息的;

input（表单控件）+select（下拉框）

name：（表单名字；同一组单选框或多选框要起一样的名字）

method：（提交方式）

action：（提交到的后台地址）

表单框 ：

<form name="" method="post/get" action="">

</form>

type：类型						radio：单选框

password：密码框				CheckBox：多选框

submit：提交按钮				checked：默认选中

value：给表单添加内容			button：普通按钮

text：文本框						reset：重置按钮





单选框/单选按钮

<input type="radio" name="ral"/>

<input type="radio" name="ral" />

单选按钮里的name属性必须写，同一组单选按钮的name属性值必须一样。

复选框

<input type="checkbox" name="like" />

<input type="checkbox" name="like" disabled="disabled" /> 

(disabled="disabled" :禁用)

(checked="checked" :默认选中)

文本框

<input type="text" value="默认值"/>

密码框

<input type="password" />

提交按钮

<input type="submit" value="按钮内容" />

重置按钮

<input type="reset" value="按钮内容" />





例如：

账号：<inpuut type="txet"/>

密码：<inpuut type="password"/>

性别：<inpuut type="radio"/>男

​	   <inpuut type="radio"/>女

 爱好 ：<inpuut type="radio" name="checkbox"/>吃

#### 14.form>select（下拉框）>option（选项）【value用它】（selected 默认选中）

例如：<select name="friuts">

​		<option value="苹果"  selected>苹果</option>

多行文本框（文本域）

<textarea name="textareal" cols="字符宽度" rows="行数">

</textarea>

#### 15.div

定义：没有语义的盒子，块级元素。

特点：（1）默认宽度占据一整行	（2）可以设置宽高

块级元素：div，h1---h6，p，hr，form，列表标签（ul>li  dl>dt>>dd  body）都是块级元素,大部分块级元素都会默认存在margin（外间距）除了div，li，dt。

#### 16.span

定义：没有语义的盒子，行内元素的代表

特点：（1）宽高由内容决定（不能设置宽高）

​	   （2）一行显示多个

行内元素：b，strong（加粗）  i,em（倾斜）  s,del（删除），img，  input, select, texttarea。

# 第二天

# 一.css简介

cascading style sheets 汉译**层叠样式表**,WEB标准中的表现标准语言,表现标准语言在网页中主要对网页信息的显示进行控制，简单说就是如何修饰网页信息的显示样式。

**层叠性：给同一个元素添加相同的css属性，属性值会存在覆盖问题.**（优先级及权重）

## （一）css语法

#### 1.样式的固定书写格式

选择器{声明}

#### 2.声明的组成  {css属性：属性值；}

例如：![1532001422209](C:\Users\WANG\AppData\Local\Temp\1532001422209.png)

#### 3.css注释

/*多行注释*/     //单行注释//

## （二）css属性

width 宽度

height 高度

background-color 背景颜色

color 字体颜色

## （三）三种样式表

#### 1.内部样式表

内部样式表语法：

<style type="text/css">

/*css语句*/

</style>

注：使用style标记创建样式时，最好将该标记写在<head></head>

作用域：当前页面

例如：

<style type="text/css">

​	div{

​		width:300px;

​		height:300px;

​		background-color:piank;

​	}

</style>

#### 2.外部样式表

a:外部样式表的创建 ：

在css的文件夹里新建css文件，书写样式，需要用到外部样式表的HTML文件。

a:外部样式表的创建 ：

<link rel="stylesheet" type="text/css" href="目标文件的路径及文件名全称" />

作用域：链接到该css文件的所有HTML页面。

#### 3.内联样式表（行内样式表）

将style作为html的属性（属性="属性值"），将声明（css属性：属性值；）作为html的属性值。

例如：<body>

​	<div style="width=300px; height=300px;">这是一个div</div>

  </body >

备注：内部：写在style里面

​	    外部：写在新建的css的文件夹里（link链接上）

​	    内联：写在body里面用style

样式表的优先级 ：

内联样式表的优先级别最高

内部样式表与外部样式表的优先级和书写的顺序有关，后书写的优先级别高。

![1532049273286](C:\Users\WANG\AppData\Local\Temp\1532049273286.png)

#### （四）选择器

#### 1.标签选择器（元素选择器）：

定义：通过标签名获取到元素。

#### 2.类选择器：

定义：通过类名（**.**class值）获取到元素，（class="绰号"）给元素添加类名（绰号），可重复。

命名规则：英文开头，包含数字，下划线。

#### 3.id选择器：

定义：通过#id获取到元素，（id="身份证号码"）给元素添加id名（身份证号码），不能重复。

id选择器 

语法：#id名{属性：属性值;}

说明： 

•  当我们使用id选择符时，应该为每个元素定义一个id属性；  如：<div id="top"></div>

•  id选择符的语法格式是“#”加上自定义的id名；  如：#box{width:300px; height:300px;}

•  起名时要取英文名，不能用关键字：(所有的标记和属性都是关键字)

•  一个id名称只能对应文档中一个具体的元素对象，因为id只能定义页面中某一个唯一的元素 对象。

•  最大的用处：创建网页的外围结构

#### 4.通配符选择器：

定义：获取到页面上的所有元素

语法：*{属性：属性值；}

说明：通配选择符的写法是“*”，其含义就是所有元素。

用法：常用来重置样式。

例如：*{margin:0;}  *{color:red;}

#### 5.群组选择器（并集选择器）：

定义：将多个基本选择器用逗号隔开，表示都获取到。

例如：p,h1,h3,f1,{margin:0;}

#### 6.后代（包含）选择器：

定义：将多个基本选择器用空格隔开，表示后一个选择器是前一个的后代。

例如：![1532008135978](C:\Users\WANG\AppData\Local\Temp\1532008135978.png)

![1532008162515](C:\Users\WANG\AppData\Local\Temp\1532008162515.png)

#### 7.伪类选择器：

定义：用冒号开头

语法 ：

a:link{属性：属性值;}超链接的初始状态（锚链接被访问前的样式）;

a:visited{属性：属性值;}超链接被访问后的状态（锚链接被访问后的样式）;

a:hover{属性：属性值;}鼠标划过超链接时的状态（鼠标悬停在原素上的样式）;

a:active{属性：属性值;}即鼠标按下时超链接的状态（鼠标点击链接时的样式）;

**当这4个超链接伪类选择符联合使用时，应注意他们的顺序**

例如：![1532009054430](C:\Users\WANG\AppData\Local\Temp\1532009054430.png)

![1532009072786](C:\Users\WANG\AppData\Local\Temp\1532009072786.png)

#### 8.选择器的优先级

!important>内联样式>id选择器>类选择器（伪类选择器）>标签选择器>通配符选择器

#### 9.只有作用在同一个元素上才能比较权重 0000

第一个0代表important或者行内

第二个0代表id选择器

第三个0代表类选择器

第四个0代表标签选择器

（继承的权重最低为0000）

![1532009861130](C:\Users\WANG\AppData\Local\Temp\1532009861130.png)

#### 10.交集选择器

定义：选择器之间没有空格，代表满足多个条件元素才被获取到。

# 第三天

# 一.CSS属性及属性值相关概念

属性：属性是指定选择符所具有的属性，它是css的核心，css共有150多个属性

属性值：属性值包括法定属性值及常见的数值加单位，如25px，或颜色值\#ccc等。

#### 1.字体的大小：

{font-size:12px/14px/16px;} 

说明：

1）属性值为数值型时，必须给属性值加单位，属性值为0时除外。

2）单位还可以是pt，9pt=12px;

3）为了减小系统间的字体显示差异，IE Netscape Mozilla的浏览器制作商于1999年召开会议，共同确定16px/ppi为标准字体大小默认值,即1em.默认情况下：1em=16px,0.75em=12px;1ppi=16px;

#### 2.字体加粗：

{font-weight:bolder/bold/normal (不想加粗)/100-900;}

说明：

1）在css规范中把字体的粗细分为9个等级，分别从100-900，其中100对应最轻的字体变形，而900对应最重的字体变形。

100-500常规字体 

600-900加粗字体

#### 3.字体倾斜：

###### {font-style:normal常规字体/italic/oblique倾斜;}

说明：

1）italic和oblique都表示倾斜，不过oblique的幅度要大一点。但一般浏览器对它们的区分不是很明显。

#### 4.字体家族

{font-family:"字体1","字体2";} 

中文字体或者多个单词组成的字体要加引号，多个字体家族用逗号隔开。

当字体是中文字体时需加引号；

当英文字体中有空格时需加引号如“Times New Roman”；

#### 5.字体颜色 color

属性值：英文单词；十六进制；

十六进制：#000000

前两个零：红		中间两个零：绿		后两个零：蓝

每一位的取值：0----9	abcdef

# 二.文本属性

#### 1.设置文本的大小写 text-transform

{text-transform:  none/capitalize/uppercase/lowercase} 

属性值：none：默认不转换	lowercase 全部小写

​		uppercase 全部大写	capitalize 首字母大写



#### 2.文本修饰

{text-decoration:   none/underline/overline/line-through/blink}

none:没有修饰		underline:添加下划线

overline:添加上划线	line-through:添加删除线

blink：闪烁 

#### 3.首行缩进

{text-indent:32px;}

text-indent可以取负值；

text-indent属性只对第一行起作用。

备注 ：单位：em 	以当前字体大小为基准，首行缩进可以取负值（隐藏字，隐藏几个字缩进几em）

#### 4.字间距

定义：控制英文字母或汉字的字距。 

例如：{letter-spacing:10px;}

#### 5.词间距

word-spacing

定义：以空格作为分隔符

例如：div{word-spcing:50px;}

#### 6.文本在容器中的水平对齐方式:text-algin

text-algin:left;（默认左边）	text-algin:center;(居中) 

text-algin:right;（右边）		text-algin:justify;（只对英文有效果，两端对齐）

#### 7.行内元素在垂直方向的对齐方式：vertical-algin

vertical-algin：base line；（默认基线对齐）	 

vertical-algin：middle；（中线对齐，一般用在图片与文字垂直居中对齐）

例如：img{vertical-algin:middle;}

vertical-algin：top；	（顶线对齐）	

vertical-algin：bottom；（底线对齐）

一般都用于图片与文字垂直方向的居中对齐

# 三.列表属性

#### 1.列表样式类型：list-style-type

list-style-type:disc(实心圆)/circle（空心圆）/square(实心方块 )none(去掉列表符号)； 

#### 2.使用图片作为列表符号：

###### list-style-image:url(所使用图片的路径及全称

#### 3.定义列表符号位置：

###### list-style-position:outside/inside;

（默认样式在li内容外边）

关于列表属性的简写：list-style:; 

# 四.边框的相关属性 border

#### ![1532774328116](C:\Users\WANG\AppData\Local\Temp\1532774328116.png)

#### 1.边框宽度：border-width

border-width

#### 2.边框的样式：border-style

border-style

边框线型：solid:实线，dashed:虚线，dotted:点状线，double:双线（最少3px），none:没有边框 

#### 3.边框的颜色：border-color

border-color

单独设置某个方向的边框属性：  

border-top：上边框 

border-bottom:下边框

border-left:左边框

border-right:右边框

#### 4.行高 line-height

定义：一行文本的高度

行高=字体大小+行高的上下间距（行高的上下间距相等）

单行文本若是想实现在容器中垂直居中，将line-height大小设置成height大小。

&：line-height测量：从上一行的最顶端到下一行文本的最顶端（一般都是偶数）

# 五.背景属性

#### 1.背景颜色

语法：选择符{background-color:颜色值;}

#### 2.背景图片的设置

语法：background-image:url(背景图片的路径及全称);

•容器尺寸等于图片尺寸，背景图片正好显示在容器中;

•容器尺寸大于图片尺寸，背景图片将默认平铺，直至铺满元素；

•容器尺寸小于图片尺寸，只显示容器/元素/范围以内的背景图。

#### 3.背景图片平铺属性

语法：选择符{background-repeat:no-repeat（不平铺）/repeat（默认平铺）/repeat-x（水平方向平铺）/repeat-y（垂直方向平铺） }

#### 4.图片在容器中的定位

语法：选择符{background-position：水平方向属性值  垂直方向属性性;} 水平方向值：left/center/right或数值        往右为正

垂直方向值： top/center/bottom或数值 往下为正

#### 5.背景图片的固定 background-attachment

属性值：scroll（默认滚动）	fixed（固定）

# 六.浮动 float

#### 1.语法：float:none（默认不浮动）/left（左浮动）/right（右浮动）;

&1.浮动的元素会脱离标准流，但文本不会脱离文本流

&2浮动的元素相当于行内块级元素（一行显示多个，可以设置宽高）

&3.当浮动的原素换行摆放，垂直的方向会考虑上一个元素的最低点

&4.浮动的起源：文字换套图片

# 第四天

# 一.盒模型

#### 1.盒模型=content（内容）+padding（内填充）+border（边框）+margin（外间距）

#### 2.width，height不是指盒子的大小，而是内容的大小

加：做页面的时候，一开始测量的是盒子的大小，但我们直接设置成width、height。若之后发现需添加padding、border盒子会被撑大，为了保证盒子的大小，width、height需减小值。

# 二.padding（内填充）

 1.padding取值:遵循上右下左原则，缺省的值找反义词的值

  2.padding-方位

  3.注意：(1)padding不可以为负值;

​                (2)背景会从padding的区域左上角开始摆放，说明background-position:0 0;在padding区域的左上角

# (三)margin

###### 1.margin取值:遵循上右下左原则，缺省的值找反义词的值

###### 2.margin-方位

###### 3.注意：margin可以为负值

# 第六天

# 一、元素类型

## (一) 块级元素

 **特点：** 

```
 (1)默认占一整行。即使设置了宽度，右边多余的部分也会用margin进行填充。
               (2) 可以设置宽高
               (3) 块级元素可以嵌套所有的行内元素以及部分的块级元素
                            错误： p>p  p>div  
               (4)大部分的块级元素都拥有默认的margin或padding，除了div、li...
                应用场景： 怎么实现块级元素在父容器里水平居中？
                        给该块级元素｛margin:0 auto;｝

​                总结：body、h1-h6、p、列表ul>li ol>li dl>dt+dd、form
```

## (二) 行内元素

**特点：**

```
（1）一行显示多个
（2）宽高由内容决定，不能设置宽高
（3）行内元素也遵循盒模型，但是设置上下的padding或margin无效
  应用：行内元素如何实现在容器中水平居中呢？
  	给其父容器添加text-align:center;
  总结：加粗、倾斜、a、span、img、input、textarea、label
```

# 二.元素类型的转换display

​             

```
   1. inline 转换成行内元素
   2. block 转换成块级元素
   3. list-item 转换成列表项 (li)
   4. inline-block 转换成行内块级元素 
      特点：（1）一行显示多个  （2）可以设置宽高
   5. none 隐藏元素，不占位置
```

# 三、行内块级元素与浮动的区别

​      

```
1.两个行内块级元素之间存在空格，会在页面中存在一条缝隙。
                解决办法：（1）将元素之间的空格删除
                          （2）给其父元素设置｛font-size:0;｝
2.行内元素都存在垂直方向基线对齐的问题
                解决办法: 设置vertical-align
      
```

# 四、如何实现元素在容器的垂直方向上居中

​    

```
1.设置一把尺子｛width:0;height:父容器的高度｝
2.该元素与尺子｛display:inline-block;vertical-align:middle;｝
```

# 第七天

## 一、定位 position

```
1. position:static; 静态定位(默认标准流定位)

	无法设置left、right、top、bottom值
2. position:relative 相对定位
  (1)相对于自己本身所在的位置进行移动定位
  (2)配合left、right、top、bottom进行移动定位。相对于自己的某条边往元素中心移动为正值。
  (3)相对定位的元素不脱离标准流。（灵魂出窍）
3. position:absolute; 绝对定位
  (1)绝对定位的元素是相对于html或者最近的有定位的父元素 进行定位
  (2)配合left、right、top、bottom进行移动定位。相对于包含块的某条边往包含块中心移动为正值
  (3)绝对定位的元素会脱离标准流 4. position:fixed ; 固定定位
  (1) 相对于浏览器的可视区域进行移动定位
  (2) 配合left、right、top、bottom进行移动定位。相对于浏览器可视区域的某条边往浏览器可视区域中心移动为正值
  (3) 脱离标准流
```

 **加：如何实现元素在容器中居中？**
            子绝父相（父元素可以是其他定位），子元素{top:50%;margin-top:-自己高度的一般;left:50%;margin-left:-自己宽度的一半。}

## 二、层级  z-index

​           

```
 1.定位>浮动>标准流
 2.z-index 只能用于有定位的元素上
 3.z-index 可以取负数
```

## 三、命名锚点

​       

```
 a[href="#id名"]跳转到id名所在的元素上
 a[href="页面路径#id名"]跳转到其他页面该id名所在的元素上
```

## 四、overflow 内容溢出容器时的处理方式

​         

```
属性值：visible 默认可见     hidden隐藏
       scroll 滚动条   auto判断需要出现滚动条时才出现
       设置某个方向： overflow-x 水平方向   overflow-y垂直方向
       规定：当某一个方向的值设置不为visible，另外一个方向会自动设置成auto
          
```

# 第八天

## 一、

```
/*a标签的padding对于span来说是margin,所以span的背景图片从右边开始摆放，不会影响到a标签padding内的背景图片*/
```

## 二、

```
滑动门：通过多张背景图片进行层叠，从而在视觉上达到同一张图片的效果
            a{padding-left存放左边的背景图片}>span{padding-right以实现文本居中}
```

# 第九天

## 一、宽高自适应

### （一）宽度自适应

```
 当块级元素的宽度设置成100%，或者不设置，宽度默认都是占父级元素的100%。
 
 经验：当父元素脱离了标准流，可以由子元素撑开它的宽度。
```

### （二）父元素的高度由子元素撑开

​          

```
  1. 高度塌陷:当子元素都浮动了，父元素会没有子元素撑开高度。
    解决办法：
          （1）给父元素加overflow:hidden;
          （2）给父元素添加最后一个子元素（块级){height:0;clear:both;overflow:hidden;} 缺点：会产生很多多余的标签
          （3）伪元素清除法，.clearfix::after{ content:"";display:block;height:0;clear:both;overflow:hidden;visibility: hidden;}
 一般我们用的时候,我们只需要将类名.clearfix添加到父元素上即可。
          
```

```
  2. 最小高度 min-height
	 * 当内容高度小于最小高度，按最小高度显示；
     * 当内容高度大于最小高度，按内容高度显示。
       应用场景：内容不确定，无法较好地控制父元素高度
```

```
 兼容ie6： ie6中，height代表的是最小高度。若想这个属性只让ie6识别，通过过滤器_height。
```

### （三）

```
1. 高度塌陷:当子元素都浮动了，父元素会没有子元素撑开高度。
      解决办法：
          （1）给父元素加overflow:hidden; 缺点:若存在内容溢出，会被裁剪掉。
          （2）给父元素添加最后一个子元素（块级){height:0;clear:both;overflow:hidden;} 缺点：会产生很多多余的标签
          （3）伪元素清除法，.clearfix::after{ content:"";display:block;height:0;clear:both;overflow:hidden;visibility: hidden;}
           一般我们用的时候,我们只需要将类名.clearfix添加到父元素上即可。
               
```

## 二.伪元素

```
1.E::before  给E元素添加第一个子元素,content:""不能省略

	  *元素类型默认为行内元素
 2.  E::after  给E元素添加最后一个子元素
 3.  E::first-letter 给E元素的第一个文本添加样式
 4.  E::first-line 给E元素的第行文本添加样式
```

# 第十天

## 一、隐藏元素的两种方式

​             

```
   1.display:none 隐藏元素，不占位置
   2. visibility:hidden; 隐藏元素，占位置
```

## 二、兼容问题

```
(1)图片有边框（ie8-） 解决办法： img{border:0 none;}
(2)div>img,img下方会存在间隙
     解决办法：
        * img{display:block;}
        * div{font-size:0;}
(3)ie6-，会错误地将浮动元素的浮向边margin加倍显示。
            解决：   ｛display:inline;｝
(4) ie7-，存在默认高度16px。
            解决办法:
                * {font-size:0;}
                * {overflow:hidden;}
(5)表单元素行高不一致问题（基线对齐的问题）
            解决办法：
                * {vertical-align: middle;}
                * {float:left;}
(6)表单元素样式在各浏览器渲染效果不一
            解决办法：给input清除默认样式{display:block;border: 0 none;padding:0;}，给input外层嵌套标签，设置input需要的样式
(7)浮动元素50%+50%>100% （ie6-）
            解决办法： 若两个元素都左浮动，给元素添加{clear:right;}
(8)ie8及以下浏览器才支持cursor:hand;
                解决办法： ｛cursor:pointer;｝
(9)透明度
                * opactity:val; val取值为0-1，越大越不透明。
                * filter:alpha(opacity=val)   val取值为0-100，整十数，越大越不透明。

```

## 三、margin塌陷：

​       

```
1.父元素与第一个子元素存在上间距，若给第一个子元素加margin-top，会错误地渲染成父元素的margin-top。
            解决办法： 
                    （1）子元素或者父元素浮动
                    （2）给父元素加overflow:hidden;
                    （3）给父元素加border-top
                    （4）将子元素的margin-top当作父元素的padding-top
```

```
2.当两个块级元素竖直排列时，上一个元素的margin-bottom与下一个元素的margin-top会发生合并，它们之间的margin取两者之间较大的值。
```

## 四、应用：自适应两栏布局

​        

```
​    * 方法一： 
                左边定宽加浮动，右边margin-left留出左边的宽（因为浮动的元素会脱离标准流，第二个元素会跑上来占据第一个元素的位置，而块级元素的宽度刚好是100%，当设置了margin-left为第一个元素的宽度，它的宽度会自动调整为页面剩余部分的宽度）
        */
        /*.dv1{width: 200px;height:600px;background-color: red;float: left;}
        .dv2{margin-left:200px;height: 600px;background: blue;}*/
```



```
    /*方法二：
            左边定宽加浮动，右边不定宽加overflow:hidden
            原理：bfc的区域不会与浮动块重叠
            加：属于同一个bfc的两个相邻块会发生margin重叠
```

# 第十一天

## 一、表单

```
1.	form[action提交的后台地址
2.	fieldset 表单字段集
3.	fieldset>legend字段集标题（必须作为表单字段集的第一个子元素）[align控制它在fieldset的某一个位置]
4.label提示信息标签
        [for] 关联到id名所在的表单元素
        若用于单选框或多选框，一般都是直接将文字及表单元素包含在label里面。
5.label提示信息标签
        [for] 关联到id名所在的表单元素
        若用于单选框或多选框，一般都是直接将文字及表单元素包含在label里面。
6.td[colspan合并列][rowspan合并行] 

```

## 二、

### （一）th\tfoot

```
1. th标题行单元格，加粗居中 
2. caption 表格标题(作为table的第一个子元素)
3. 行分组  thead表头   tbody表体      tfoot表尾
     thead>tr>th        tbody>tr>td   tfoot>tr>td
     书写顺序：thead、tfoot、tbody，这样子保证在数据加载完毕前，先呈现表头跟表尾。
如果要使用 thead、tfoot 以及 tbody 元素，就必须使用全部的元素。(如果没有表尾，就省略tfoot)
4. 列分组colgroup[span表示每个列分组占据的列数
5. table
        [rules 添加分隔线]:cols列分隔线   rows行分隔线   
        all 行与行、列与列都存在分隔线   none没有     groups组分隔线
        [align] 整个表格在其父元素的水平对齐方式  

```

### （二）table

```
1.(table)border-spacing 单元格与单元格之间的间距,不可取负值
2.(table)border-collapse 合并单元格边框
                    属性值：separate默认分离  collapse合并
3.(td)empty-cells 无内容时单元格边框的设置
                    属性值：show默认出现   hide隐藏
4.(caption)caption-side：top/right/bottom/left
                    * left,right位置只有火狐识别

           
            /*border-spacing : 0;*/  	 	边框距离为0
            /*border-collapse:collapse;*/	合并边框
```

## 三.  html5新表单

### (一) html表单标签

​          

```
  1.拥有输入功能的下拉列表 input[list]+datalist[id]
  2.输出output，配合着form[oninput]使用。
```

### (二)表单类型type

​        

```
​    1.color 拾色器
     2.email 邮箱（正则验证）
     3.number 数字
     4.tel 电话号码
     5.url 网址（正则验证）
     6.search 搜索
     7.range 特定范围内的数值选择器，min最小值、max最大值、step( 步数 )、value当前值
```

### (三)表单html属性

​           

```
 1.autofocus 自动聚焦
 2.placeholder 占位符
 3.required 必填项
 4.pattern  正则
```

# 第十二天

## 一、新标签

```
	    1.header 头部标签，一般都是包含标题标签或者导航条。header、footer不互相嵌套。
        2.hgroup 对标题进行组合
        3.footer 一般都是版权信息、作者简介。。。
        4.nav 导航条
        5.main  主要内容，一个页面就用一次，外层结构。
        6.article 文章、独立的内容块。article可以嵌套自己。
        7.section 章节、区块，专题性的内容
        8.aside 侧边栏，非正文的内容
        9.figure对图片跟文字进行组合>figcaption 对figure的内容进行说明
        10.time时间 [datetime 规定具体时间]
        11.details细节[open默认显示细节]>summary 对细节的总结
        12.定义进度条  progress[max最大值][value当前值]
        13.meter 度量尺[min最小值][max最大值][low较低的值][high较高的值][value当前值][optimum较佳的值，当取值小于较低的值说明越低越好，反之同理]
        14. ruby注释标签 > rt对内容的注释信息
        15.引入视频的方式：video[src] 或者 video>source[src]
        (1)[controls]控制条
        (2)[autoplay]自动播放
        (3)[loop]循环播放
        (4)[width][height]
        (5)[poster]等待加载时的图片

    支持格式：ogg、mp4、webM
```

# 第十三天

## 一、选择器

### （一）基本选择器

​             

```
   1.标签（元素）选择器：通过标签名获取元素
   2.类选择器：通过.类名获取元素
   3.id选择器：通过#id名获取元素
   4.通配符选择器：通过*获取到页面中所有元素
   5.群组选择器E1,E2：通过逗号同时获取到多个选择器，即获取E1和E2，以此类推。

```

### （二）层次选择器

​        

```
​    1.后代选择器E1 E2:表示获取到的E2元素是E1元素的后代
     2.子代选择器E1>E2:表示获取到的E2元素是E1元素的子代
     3.相邻兄弟选择器 E1+E2:表示获取的E2元素紧跟在E1元素的后面
     4.兄弟选择器E1~E2:表示获取E1后面的所有E2元素

```

### (三) 动态伪类选择器

​      

```
​      1. :link 锚链接被访问前添加的样式
       2. :visited 锚链接被访问后添加的样式
       3. :hover 鼠标悬停在任意元素上添加的样式
       4. :active 鼠标点击任意元素时添加的样式
       5. :focus 表单元素被聚焦时添加的样式

```

### (四)目标伪类选择器

​          

```
  E:target  获取到E元素里面被作为当前目标的元素

```

### (五)ui状态伪类选择器

​        

```
​    1. :enabled 可用的表单元素添加样式
     2. :disabled 可用的表单元素添加样式
     3. :checked 选中的表单选框添加样式

```

### (六)结构伪类选择器

​        

```
​    1. E:first-child  获取到其父元素的第一个子元素，且要满足为E元素
     2. E:last-child  获取到其父元素的最后一个子元素，且要满足为E元素
     3. E:nth-child(n) 获取到其父元素的第n个子元素，且要满足为E元素。从1开始计数。
     4. E:nth-last-child(n) 获取到其父元素的倒数第n个子元素，且要满足为E元素。从1开始计数。
                * n的取值： 具体数值    odd（2n-1）第奇数个孩子   even（2n）第偶数个孩子   
                            -n+a 获取到父元素第一个到第a个孩子
     5. E:first-of-type 获取到其父元素的第一个E类型的子元素
     6. E:last-of-type 获取到其父元素的最后一个E类型的子元素
     7. E:nth-of-type(n)  获取到其父元素的第n个E类型的子元素
     8. E:nth-last-of-type(n)  获取到其父元素的倒数第n个E类型的子元素
     9. E:empty  空文本的E元素（不能有空格）添加样式
     10. E:only-child   获取到其父元素唯一的一个子元素,且要满足为E元素
        /*.zhubaba div:only-child{background: red;}
     11. E:only-of-type  获取到父元素的唯一一个E类型的孩子

```

### (七)否定伪类选择器

​      

```
      F:not(E)  除了E条件以外的所有F元素

```

### (八)伪元素选择器

​        

```
​    1.E::before{content:""} 给E元素添加第一个子元素（行内元素）
     2.E::after{content:""} 给E元素添加最后一个子元素
     3.
     4.
     5.E::selection E元素的内容被选中时添加样式
              兼容火狐::-moz-selection

```

### (九) 属性选择器

​       

```
​     1. E[attr] 拥有该attr属性的E元素被获取到
      2. E[attr="val"] 拥有该attr属性，且属性值等于val值的E元素被获取到
      3. E[attr*="val"] 拥有该attr属性，且属性值包含val值的E元素被获取到
      4. E[attr^="val"] 拥有该attr属性，且属性值以val值开头的E元素被获取到
      5. E[attr$="val"] 拥有该attr属性，且属性值以val值结尾的E元素被获取到
      6.语言伪类选择器 q:lang(no){quotes:"""";}
            * q[lang="no"]在内容两侧会生成引号，若想改变符号，通过如上的语言伪类选择器

```

## 二、文本属性

​    

```
​    1.文本阴影 text-shadow:x-offset  y-offset blur color[,...];
            * x-offset 水平偏移，往右为正
            * y-offset 垂直偏移，往下为正
            * blur 模糊区域，不能取负值
     2.文本溢出 text-overflow
                * 属性值： clip默认不处理   ellipsis 以省略号的形式出现
                * 配合三个属性使用：width、white-space:nowrap、overflow:hidden
     3.单词换行 word-wrap:break-word;
     4.自定义字体 @font-face{font-family起名字;src:url("字体路径")}
     5. 字体图标：矢量图（理解成文字），放大缩小不会模糊。

```

## 三、背景属性

​            

```
​    1.背景图片的尺寸 background-size
        取值：
             * 数值: 水平 垂直; 绝大部分情况会出现扭曲变形。
             * cover 背景图片完全覆盖容器,绝大部分会出现背景图丢失一部分的情况
             * contain 容器完全包含背景图片,绝大部分会出现容器留白现象
             * 等比缩放：cover、contain
             * 应用：一般轮播图采用背景图片｛background-size:cover;background-position:center center;｝

```

```
2.背景图片的定位区域 background-origin
     属性值：
             * 默认从padding开始摆放 padding-box
             * 从content开始  content-box（说明此时background-position:0 0;在content内容的左上角。）
             * border-box 

```

```
3.背景图片的裁剪（最终显示区域）background-clip
             * border-box 从边框部分开始裁剪
             * padding-box 从padding部分开始裁剪
             * content-box 从content部分开始裁剪

```

# 第十四天

## 一、边框属性

#### 1.边框阴影box-shadow

```
 边框阴影box-shadow: x-offset y-offset blur spread color inset[,...];
                    * x-offset 水平偏移，往右为正值
                    * y-offset 垂直偏移，往下为正值
                    * blur 模糊区域
                    * spread 扩展区域
                    * color 颜色
                    * inset 往元素内部移动。若是不设置，则往元素外部添加边框阴影

```

#### 2.边框图片 border-image

```
边框图片 border-image
                * 边框图片引入border-image-source:url()
                * 边框图片的裁剪 border-image-slice 遵循上右下左原则(不带单位)
                * 边框图片的宽度 border-image-width 若省略该值，默认就是边框宽度
                * 边框图片的重复 border-image-repeat
                    *属性值：stretch默认拉伸    repeat重复  round压缩重复
                * 边框图片向外延伸 border-image-outset 不能取负数

```

#### 3.边框圆角 border-radius

​              

```
边框圆角 border-radius
某个角的边框圆角：border-垂直方位-水平方位-radius:水平半径 垂直半径;
                border-radius:水平半径/垂直半径;
                    水平或垂直半径遵循（从左上角开始）顺时针原则,缺省的值找对角

```

## 二.渐变

### （一）线性渐变  linear-gradient

​       

```
​         1.gradient(linear,起点坐标,终点坐标,from(color),to(color))
                    * 坐标写法：水平坐标 垂直坐标; (只能用百分比)
          2.gradient(linear,起点坐标,终点坐标,color-stop(渐变开始的位置,color)[,...])
                    * 渐变开始的位置取值为0-1
          3.linear-gradient(方向||角度,颜色 渐变开始的位置)
                    * 方向：top bottom left right
                    * 角度单位:deg
                    * 渐变开始的位置:0-100%
                    * 老版本（加前缀的写法）+新版本 = 90deg

```

### (二)径向渐变radial-gradient

​      

```
​          1. radial-gradient(圆心，颜色 开始渐变的位置[,....])
           2. radial-gradient(圆心,size||shape,颜色 开始渐变的位置[,....])
                    * size大小：
                        closest-side：最近边； 
                        farthest-side：最远边；
                        closest-corner：最近角；
                        farthest-corner：最远角（默认值）
                    * shape形状：
                        ellipse椭圆形(默认)，circle表示圆形。

```

#### (三) 重复渐变 repeating-linear（radial）-gradient 用法同上

#### 加

```
		 浏览器               内核                 私有前缀
        chrome、safari       Webkit               -webkit-
        opera                Presto               -o-
        ie                  Trident               -ms-
        firefox             Gecko                 -moz-
        chrome、opera        blink

```



## 三、过渡 transition  过渡：让变化在一段时间内进行

​          

```
 		   1. 需要过渡的属性  transition-property
            2. 过渡的时间 transition-duration
            3. 过渡的形式 transition-timing-function
                *linear 匀速    ease慢速进入慢速离开
                *ease-in 慢速进入   ease-out慢速离开
                *ease-in-out慢速进入慢速离开
            4. 过渡的延迟 transition-delay
            总属性 transition: 1 2 3 4;(1跟2不可以省略)
            多个属性同时过渡可以用all。

```

## 四.2d变换transform ==>这是一种状态

  

```
​           1. 移动变换 transform:translate(水平方向(右),垂直方向(下))
                改变某个方向 transform:translateX(水平方向) 
                transform:translateY(垂直方向)
                *取值取百分比的话，指的是参考自己的宽高
            2.利用移动变换实现小盒子在大盒子居中：子绝父相，left50%，top50%，transform:translate(-50%,-50%)
            3.盒模型的取值写百分比，指的是父元素宽高的百分比：content（width、height）、border、padding、margin
            4.缩放变换transform:scale(x,y)
                * 取值为缩放比（倍数），基准点为元素中心。
                * transform:scaleX(x)    transform:scaleY(y)
           5.旋转变换 transform:rotate(deg)
                *顺时针旋转为正值，基准点在元素中心
           6.transform:skew(x轴旋转的角度，y轴旋转的角度)
                *transform:skewX(x轴旋转的角度)
		  7.写变换时，先写移动，再写旋转。
		  8.改变元素变换的基准点 transform-origin
                取值：数值 百分比 方位

```

# 第十五天

## 一、颜色模式

​	

```
（属性值：可以控制某个属性）
            1.rgba(red0-255,green0-255,blue0-255,alpha不透明度0-1)
            2.hsla(色调0-360,饱和度0-100%,亮度0-100%,alpha0-1)
            3.transparent 完全透明 (三角形)

```

## 二、盒模型

​    

```
​    盒模型由content内容、padding内填充、border边框、margin外间距组成。
        1.标准盒模型：width、height指的是content的宽高
        2.怪异盒模型: width、height指的是content+padding+border的宽高
        box-sizing 规定盒模型
            *属性值：content-box（默认）     border-box设置成怪异盒模型
        

```

## 三、3d变换

```
1.transform:translate3d(x,y,z); 移动变换
            transform:translateZ(z),其他方向同理
2.transform-style:preserve-3d; 保持3d变换（父元素上）
                *flat平面（默认）
3.设置观察的距离，景深perspective(父元素上)
4.旋转变换   
        左手定律：大拇指指向轴的正方向，其他手指卷曲的方向为旋转的正方向
        transform:rotate3d(x,y,z,deg)  x、y、z取值为0（不旋转）或1（旋转）
                transform:rotateX(deg);

```

#### 加：

```
 1.导航的套路
 2.两个a一开始先放在li同一位置再进行移动旋转变换
 3.hover之后整个li翻转即可。过渡及延迟。

```

## 四、关键帧动画

### （一）自定义动画

​         

```
   （1）通过@keyframes指定动画序列；@keyframes name{}
            （2）通过百分比将动画序列分割成多个节点；
            （3）在各节点中分别定义各属性
            （4）通过animation将动画应用于相应元素；

```



```
        @keyframes name{
            百分比{
                声明
            }
        }

```

### (二) animation属性

​           

```
  1. animation-name 动画名字
  2. animation-duration 动画播放时间
  3. animation-timing-function 动画播放的形式
                    linear匀速   ease...
                    steps(n)
  4. animation-delay 动画播放的延迟
  5. animation-iteration-count 动画播放的次数  infinite无限次播放
  6. animation-direction 动画播放的方向
                    属性值：normal正向播放  reverse反向播放  alternate 交替播放 
                    alternate-reverse反向交替播放
  7. animation-fill-mode 动画完成后的状态  forwards保持最后的状态
                animation: 1 2 3 4 5 6 7;

```

# 第十六天

## 一、弹性盒布局

### （一）设置在父元素上

​         

```
 1.display:flex; 将父元素设置成弹性盒，那么里面的子元素会在主轴方向上默认不换行摆放；侧轴方向的大小不设置的话，就会在当前行默认被拉伸
 2.flex-direction 设置主轴方向
                    属性值：
                        row 从左往右
                        row-reverse 从右往左
                        column 从上到下
                        column-reverse 从下到上
3.flex-wrap 伸缩换行
                    *nowrap默认不换行
                    *wrap 换行
                    *wrap-reverse 换行反向    主轴是水平时，上下反向，主轴垂直时，左右反向；
4.flex-flow:flex-direction ||  flex-wrap;
5.justify-content 设置子项目在主轴方向的对齐方式
                * flex-start 默认在主轴的起点位置靠齐摆放
                * flex-end 在主轴的终点位置靠齐摆放
                * center 在主轴的中间位置靠齐摆放
                * space-between 将主轴方向空白区域平分在子项目之间
                * space-around 将主轴方向空白区域环绕在子项目两侧
 6.align-items 设置子项目在（当前行）侧轴方向的对齐方式
                * stretch 若不设置子项目在侧轴方向的大小，会被默认拉伸
                * flex-start 若设置子项目在侧轴方向的大小，会被默认摆放在侧轴的起点位置
                * flex-end 摆放在侧轴的终点位置
                * center 摆放在侧轴的中间位置
                * baseline 子项目以基线对齐
 7.align-content 控制子项目在侧轴方向的对齐方式（换行）
                属性值等同于 justify-content


```

### （二）设置在子元素上

​            

```
 1.flex 设置子项目在主轴方向的比份
 2.align-self 设置单个子项目在（当前行）侧轴方向的对齐方式
                    取值同align-items
 3.order 设置子项目的显示顺序
                * 设置了order会放在没设置order子项目后面
                * 都设置了order,数字越小越靠前

```

## 二、多列布局

​    

```
 1.column-width 每列的最小宽度
 2.column-count 最多的列数
 3.column-gap 列间距
 4.column-rule 列边框
 5.column-span 跨列
            *none不跨列 all跨所有列

```

w<768,pink。当页面宽度w大于768px时，div显示红色。w>992px,green。w>1200,blue。*/

## 三.媒体查询

​          

```
  1. 用法 @media screen and (条件){选择器{声明}}
  2.  min-width 当页面宽度大于最小宽度，生效。（从小写到大）
                max-width 当页面宽度大于最小宽度，生效。（从大写到小）
                min-device-width 【设备宽度】
  3.link[media="screen and (条件)"][href]

```

## 四、自适应布局

​      

```
1.  元素的宽高自适应窗口或者子元素的大小，从而实现同一套页面适应不同的窗口、分辨率及设备。（！！！）
2.  响应式布局（一般都是用于较为简单的页面）
        响应不同的屏幕大小或者设备大小，对同一套页面的部分布局进行修改，但大体保持一致。

```

# 8.8 第十七天

## 一、移动端页面布局

#### 1.弹性布局（100%布局）——拉勾网、天猫首页  px

```
好处：充分发挥大手机的优势——显示内容越多.
缺点：屏幕过大，间距过大，比例失调。

特点：

顶部与底部的bar不管分辨率怎么变，它的高度和位置都不变；

中间每条招聘信息不管分辨率怎么变，招聘公司的图标等信息都位于条目的左边，薪资都位于右边。

2、等比缩放布局（rem布局）——网易、淘宝首页
 尽量保证不同设备显示效果一致

```



#### 2.meta:vp 设置理想视口

```
   1. 观察设计稿640px-iphone5开发320px
      设计稿750px-iphone6开发375px
   2. js代码的后三句复制过来，记得给meta加id名！！！！
   3. #football{height:100%;display:flex;flex-direction:column;}
      除了main以外每一层都设置高度，main{flex:1;overflow-x:hidden;}
      !!!不要给main设置弹性盒
      5.若rem布局，添加两句代码（动态修改根部字体大小）。查看控制台，iphone5-64px。iphone6-75px



```

#### 加：字体图标网址：http://www.iconfont.cn/collections/detail?spm=a313x.7781069.1998910419.de12df413&cid=9402

# 二阶段

## 加：（一）js历史

### (1)JavaScript的诞生

JavaScript 诞生于 1995 年。由Netscape(网景公司)的程序员Brendan Eich(布兰登)与Sun公司联手开发一门脚本语言, 最初名字叫做Mocha，1995年9月改为**LiveScript**。12月，Netscape公司与Sun公司（Java语言的发明者）达成协议，后者允许将这种语言叫做JavaScript。这样一来，Netscape公司可以借助Java语言的声势。

1996年3月， Netscape公司的浏览器Navigator2.0浏览器正式内置了JavaScript脚本语言. 此后其他主流浏览器逐渐开始支持JavaScript.

### (2)js版本

JavaScript这种语言的基本语法结构是由ECMAScript来标准化的, 所以我们说的JavaScript版本一般指的是ECMAScript版本.

- 1997年7月，ECMAScript 1.0发布。

- 1998年6月，ECMAScript 2.0版发布。

- 1999年12月，ECMAScript 3.0版发布。

- 2007年10月，ECMAScript 4.0版草案想要提交ECMA组织, 但由于4.0版的目标过于激进, 改动太大, 并且微软,谷歌等大公司极力反对；一直到2008年7月ECMA开会决定，中止ECMAScript 4.0的开发（即废除了这个版本）

- 2009年12月，ECMAScript 5.0版正式发布

- 2011年6月，ECMAscript 5.1版发布

- 2015年6月，ECMAScript 6正式发布，并且更名为“ECMAScript 2015”。

  ### (3)js语言的组成

  javascript = ECMAScript + BOM + DOM

  核心(ECMAScript)

  浏览器对象模型(BOM)      brower

  文档对象模型(DOM)      document

  ECMA 欧洲电脑厂商联合会 制定js规范。

  W3c(万维网联盟)指定html及css规范



# 一、js语法

## （一）js的书写位置

#### 1.script[src引入外部js文件][type="text/javascript"]（可以省略）

备注：若是存在src属性，在当前script标签里写代码无效

```
`<script type="text/javascript" src="../js/01.js">`
```



#### 2.作为a标签的href属性值

```
[href="javascript:js代码"]
```

 `<a href="javascript:alert(100);" style="color:red">aaaa</a>`

## (二)js注释

​            //单行注释
            /*多行注释,不要嵌套多行注释*/

## （三）声明变量及赋值

#### 1.声明变量（容器）通过关键字 var

#### 2.给变量赋值，将10的值赋给a

例如：var a；

​	    a=10；

#### 3.同时声明变量及赋值

例如：`var uname="lemon"`

#### 4.同时声明多个变量，用逗号隔开

例如：

```
var  b,c,d;

b=100;

c=200;

d=300;

var b=100,c=200,d=300`
```



变量命名规范：

（1）变量名由数字,字母,下划线_和美元符$组成,不能由数字开头；

（2）不能使用关键字或保留字

（3）严格区分大小写，如：age和Age是不同的变量

变量命名建议：

（1）见名知义，例如苹果就写apple 

（2）驼峰命名，例如我的苹果就写myApple 

# 二、数据类型

## （一）基本数据类型

#### 1.数字类型 Number

```
var uage=17；
```

#### 2.字符串类型 String ：带引号的值都是字符串类型

例如：

```
var uname="lemon"
```



#### 3.布尔类型 Boolean

两个值：true，false

```
var result=true；	var result=false；
```



#### 4.字符串引号嵌套引号

备注：SyntaxError 语法错误

（1）将外层引号改成不一样的（单引号、双引号）

（2）通过反斜杠\转义字符

例如：

```
 		var sayHi = "Hello,my name's Lily.";
         var sayHi = 'Hello,my name\'s Lily.';
```



# 三、输出

#### 1.alert（变量不加引号||具体的值）弹窗输出

例如：

```
var="lemon"

	    alert(uname)（弹得是lemon）

	    alert("uname")（弹得是uname）

	     alert(10)（弹得是10）
```



#### 2.document.write()  在body里面输出内容，可配合标签使用

例如：

```
`document.write(啦啦啦);`

	    `document.write(不问天明);`

            `document.write(uname);`
```

备注：联在一起

#### 3.console.log (变量不加引号||具体的值) 往控制台console输出内容

```
*调试   `console.log(uname);`
        `console.log(true);`
```



# 四、运算

## （一）算数运算 +	 -	 * 	/ 	 %（求余数）

#### 1.字符串拼接：当字符串两侧有一侧为字符串，此时为字符串拼接。

例如：1+"2"="12"

备注：字符串内拼接变量口诀 "+变量+"（引号可以是任意引号，单双都可）

##### 案例做法步骤：

```
 <input type="text" id="num1" />
 <input type="button" value="+" onclick="jia()"/>
 <input type="button" value="-" onclick="jian()"/>

 <input type="text" id="num2" />
```



###### 1.获取到两个文本框 `document.getElementById("id名")`

例如：

```
 var num1 = document.getElementById("num1");
 var num2 = document.getElementById("num2");
```



###### 2..获取到两个文本框内容 value

例如： 

```
var _num1 = num1.value

var _num2 = num2.value
```



###### 3.文本框内容进行算数运算，将最终结果输出

例如：

```
var jieguo = Number (_num1)+Number(_num2)
var jieguo = _num1 - _num2
```



###### 4.点击按钮时才执行2,3代码

(1)给元素添加事件[onclick="函数名"]

例如：

```
 <input type="button" value="+" onclick="jia()"/>
 <input type="button" value="-" onclick="jian()"/>
```

（2）定义函数，函数里面定义2,3代码

​	function 函数名（）{js代码}

例如：

```
function jia(){
            var _num1 = num1.value;
            var _num2 = num2.value;
            var jieguo = Number(_num1) + Number(_num2);
            console.log(jieguo);
        }
```



```
      function jian(){
            var _num1 = num1.value;
            var _num2 = num2.value;
            var jieguo = _num1 - _num2;
            console.log(jieguo);`
       }
```

备注遇到的问题：
    	（1）代码执行顺序是从上往下的，必须在元素创建之后才能获取
   	   (2) 点击事件[onclick="函数名()"]触发函数,自定义函数通过function 函数名(){js代码}
	 （3）文本框的值肯定是字符串类型，会存在字符串拼接的问题

## （二）赋值运算

#### 1. = 将右边的值赋给左边（右边运算完再赋给左边）

例如：`var str = "我的名字叫";`

#### 2 += 在原来基础的内容上追加内容

例如：

```
var str = "我的名字叫";

	 var name = "lemon";
        str += name;（str = str + name;）

	console.log(str);`（输出的是我的名字叫lemon）
```

![1534163901266](C:\Users\WANG\AppData\Local\Temp\1534163901266.png)



#### 3.同理 -=		*=	/=	%=

## （三）关系运算，返回布尔值（存在隐式转换）

![1534168596540](C:\Users\WANG\AppData\Local\Temp\1534168596540.png)



#### 1. == 等于判断两边的内容发生隐式转换后一致，就返回true

```
var a = true == 1;
        console.log(a);

#### 2. != 不等于只有等式两边的值
```

#### 内容发生隐士转换后不一致，才返回true

#### 3.>		>=		<		<=

#### 4.=== 只有类型都一致的情况下（不发生隐式转换），才返回true

#### 5.！== 不全等于

#### 6.关系运算符的比较规则

（1）数字和数字直接比较

（2）数字和字符串比较：字符串转换成数字再进行比较

（3）字符串和字符串进行比较：进行字符串的ASCII码进行比较

## （四）逻辑运算

#### 1.与运算：&&运算符两侧的值都为true才返回true

 	

```
var b = 12;
        var c = "4"==4 && (b+=1) >12;//false
        console.log(b);
```

若与运算的左侧返回值为false，直接终止运算

#### 2.或运算 ||

运算符两侧的值都为false，才返回false

若或运算左侧的值返回true，直接终止运算

# 五、数据类型的转换

#### 1.主动转换（直接转换）

（1）Number（）将其他数据类型转换成数字类型

​	Number（字符串）==>数字、NaN）String

​	Number(布尔值) => 1、0

```
console.log(Number("123")); //123
        console.log(Number("abc")); //NaN(非数字),属于数字类型的一个特殊值。
        console.log(Number(true));  //1
        console.log(Number(false));  //0
```

（2）string（）转换成字符串类型，在值两侧加引号

```
console.log(string(123));//  转换成"123"
console.log(string(123));//  转换成"true"
```

（3）Boolean 转换成布尔类型 true	false

备注：数字0、NaN 、""、underfine、null 转换成布尔值为false，其余的都是true

###### 注意：NaN

(1)不代表任何值，也不等于任何值，甚至自己都不等于自己

(2)任何数据与NaN预算都返回NaN

(3)isNaN：用来判断a到底是不是非数字，返回布尔值

#### 2.隐式转换

定义：当运算无法进行下去时，内部就会尝试数据类型的转换

#### 3.数字常用的方法

###### （1）parseInt(a)将a取整

例如：

```
parseInt("123.33")==>123
```



###### （2）parseFloat(a)取浮点数

例如：

```
parseFloat("123.333abc")==>123.33
```



#### 4.Math.round(a)对a四舍五入取整数

```
console.log(Math.round(123.33));
```

#### 5.Math.random()取[0,1)里面的随机数，不包含1

#### 加：运算符优先级

###### 运算符优先级：括号>一元运算（！）>算术运算符>关系运算符（大于小于号>双等全等号）>逻辑与>逻辑或

# 8.14 第二天

## 一、特殊数据类型

#### 1.Null

```
Null 空对象：对象只有一个特殊的值为null，表示一个空对象引用（指针），
  typeof 操作符检测 null会返回object。
```

#### 2.Undefined

```
Undefined :只有一个值undefined，当声明一个变量但为赋值，返回undefined
备注：区分undefined和 not	defined （underfine与not defined的区别：underfine是没有对变量进行初始化赋值，而not defined是报错，意思是该变量未定义、不存在，不能使用。）
	 undefined：声明变量但未赋值
	 not  defined：报错变量未声明定义
```

### 加：（三）引用数据类型

```
Arrey 数组  object对象
```

## 二、typeof  判断数据类型

```
typeof(123);//Number
typeof(NaN);//number
typeof("123");//string
typeof(true);//boolean
typeof(null);//object 
typeof(undefined);//undefined
```

## 三、程序三大流程

```
顺序执行：从上到下
分支（选择）执行：通过条件判断语句，执行相应的代码
循环执行：通过循环语句执行相应的代码（重复做一件事情）
```

### （一）if 语句

#### 1.单分支

```
单分支：if(条件){满足条件执行代码}
例如：var a = 5;
		if(a == 5){
            alert("这个数是5")；
		}

```

#### 2.双分支

```
双分支：if(条件){满足条件执行代码}else{不满足条件执行这里的代码}
例如：   var a = 5;
		if(a == 5){
            alert("这个数是5");
        }else{
            alert("这个数不是5")
        }

```

#### 3.多分支

```
多分支：if(条件1){满足条件执行代码}else if(条件2){满足条件2执行的代码}else{不满足以上所有的条件执行}

```

#### 4.案例 判断奇数偶数步骤

```
1.获取到文本框跟#output
2.给按钮添加点击事件 [onclick = "函数名"]
3.定义函数 function 函数名(){
    获取文本框的值
    选择分支语句(奇数，偶数，其他)
    将结果输出
}

```

例如：

```
	 <input type="text" id="num" />
    <input type="button" value="判断奇偶数" onclick="jiou()"/>
    <div id="output"></div>		
        
 <script type="text/javascript">
		var num = document.getElementById("num");
        var output = document.getElementById("output");
        // var _output = output.innerHTML;
        function jiou(){
            var _num = num.value;
            if(_num % 2 == 0){
                output.innerHTML = '<span style="color:red">这个数是偶数</span>';
            }else if(_num % 2 == 1){
                output.innerHTML = '<span style="color:green">这个数是奇数</span>';
            }else{
                output.innerHTML = '<span>这个数不存在</span>';
            }
		 }
</script>		 

```

###### 三元运算符(双分支情况使用)

###### 条件？满足条件执行这里:不满足条件执行这里

```
 三元运算符写法：   output.innerHTML = _num%2==0 ? '<span style="color:red">这个数是偶数</span>':'<span style="color:green">这个数是奇数</span>';
       

```

##### 常犯错误：

```
1. = 代表的是赋值号，a = b; a = c; 相当于 b = c;这种说法不存在的，从始至终只改变了a的值，b没有任何变化

```

##### 补充：点击事件执行函数的三种方法

```
1.（1）给元素添加[onclick="函数名"]//加在btn那种
  （2）定义函数：function 函数名(){}
2.（1）ele.onclick = 函数名
  （2）定义函数 function 函数名 {}
3.ele.onclick = function (){} ==>匿名函数 例如：btn.onclick

```

### （二）switch 语句（语句在比较值得时候用的是全等符操作）

```
switch(变量||表达式){
	case 值1:
	case 值2:
	满足上面执行这里的代码;
	break;
	case 值3:
	满足上面执行这里的代码;
	break;
	........
	default:
	以上条件都不满足值行这里的代码;
	break;//跳出语句
}

```

例如：每个月 的天数

```
 	<input type="text" id="month" />
    <input type="button" id="btn" value="确定天数" />
    <div id="output"></div>
    <script type="text/javascript">
        var month = document.getElementById("month");
        var btn = document.getElementById("btn");
        var output = document.getElementById("output");
        btn.onclick = function(){
            var _month = Number(month.value);
            switch(_month){
                            case 1 :
                            case 3 :
                            case 5 :
                            case 7 :
                            case 8 :
                                output.innerHTML = _month + "月有31天";
                                break;
                            case 2 :
                                output.innerHTML = _month + "月有28天";
                                break;
                            case 4 :
                                output.innerHTML = _month + "月有30天";
                                break;
                            default :
                                output.innerHTML = "你是猪吗";
                        }
                    }
                </script>

```

## 四、一元运算

```
1. ++	自增1
 前置 ++a:先对a进行自加1，再将a的值返回出去
 后置 a++:先将a的值返回出去，在对a进行自增1
例如：	  var a = 10;
        var b = ++a; 
        console.log(a,b); //11 11


```

```
2. --	自减1
 前置 --a:先对a进行自减1，再将a的值返回出去
 后置 a--:先将a的值返回出去，在对a进行自减1
 例如：  var i = 1;
        var k = i++ + --i + i-- + ++i;
        //i=1
        //k = 1 + 1 + 1 + 1
        console.log(i,k);

```

### 五、进制(保留几位小数)

```
1.十进制 0~9	//10086
2.二进制 0b开头，取值为0或者1	//（0b1010）
3.八进制 0o开头，取值0~7	//0o77
4.十六进制 0x开头，取值0-9，a-f	//0x776
5.进制转换
       （1）十进制转多进制 toString(n)
        (2) 多进制转十进制 parseInt(num,n);
        (3) toFixed(n) 保留n位小数

```

例如：

```
	    var a = 10086; //十进制，取值0-9
        var b = "0b1010";
        var c = "0o776";
        var d = "0xef14";
        console.log(a.toString(2));
        console.log(parseInt("1010",2));
        console.log(a.toFixed(2));	

```

# 8.15第三天笔记

# 一、

##### （一）概念：当满足一定条件前提下，反复执行一段代码（死循环），直到条件不在满足时退出。（编写条件时，要避免出现死循环 ）

##### （二）三大要素：变量初始化、条件、变量更新。

##### （三）while语句

##### 1. while

```
变量初始化
	while(条件){
        执行的代码;//条件成立就会不断的执行这里的代码，直到条件不成立）
        变量更新;//一般都放在执行的代码 的后面
	}

```

例如：

```
var money = 100; //变量初始化
while(money>50){ //while（条件）
    console.log("666); //执行的代码
    meney = meney-10; //变量更新
}

```

##### 2. do

```
变量初始化
	do{
        执行的代码;//不管三七二之一先执行一次
        变量更新;//一般都放在执行的代码 的后面
	}while条件();

```

例如：

```
var num = 16; //变量初始化
do{
    console.log("未成年人禁止观看")(num<18) //执行的代码
    									//变量更新
}while(num>18)	//while(条件)
备注：先执行完再看条件

```

##### （四）for（变量初始化；条件；变量更新；）{执行的代码}

​	例如：

```
for(var i=10;i>0;i--){
    console.log(i); //循环条件成立，执行这里的代码
}

```

###### 注意：在变量更新后不加  ；（分号）

## 二、break （循环语句使用，继续下一次循环）

```
1.break 跳出当前整个循环 
备注：break一但运行，当前循环语句的里的代码都不再执行
	 在多个嵌套循环中，一个break语句只向外跳一层循环
	 break和continue如果带标识，则跳出标识所在的循环
	 
	 “++”拼接字符串

```

```
2.continue 跳出本次循环，继续下一次循环

```

# 8.16

## 一、函数的定义

###### （1）函数就是把特定功能的代码抽取出来并进行封装

###### （2）使用函数的好处：函数可以重复某一部分的代码通过函数名调用；

###### 使程序变得简短而清晰；

###### 有利于程序维护；

## 二、函数的声明

#### 1.声明式 ：通过关键字 function

###### 格式：function 函数名（形参）{js代码}

例如：

```
function zhengshu(a,b){
    for(var i=a;i<=b;i++){
        cosole.log(i);
    }
    zhengshu(99,111);
} //备注：a，b为形式参数，输入什么看下面

```

#### 2.赋值式：

###### 格式：var变量 （即函数名）=function（a,b）{js代码}

例如：

```
var zhengshu = function(a,b){
     for(var i=a;i<=b;i++){
        cosole.log(i);
    }
    zhengshu(99,111);
}//备注：a,b也为形式参数，输出什么看下面（好比btn.onclick=function(){}	）

```

#### 3.构造函数（不推荐使用）

```
 var sum = new Function(‘num1’,’num2’,’return num1+num2’);

```

## 三、函数的执行

#### 1.手动调用:

​    

```
  sum();

```

#### 2.事件驱动

###### 格式：元素.事件=function（）{} 或者   函数名

常见的事件：

- onclick：点击事件
- ondblclick：双击事件
- onmouseover：鼠标移入事件
- onmouseout:鼠标移开事件
- onchange：内容改变事件（一般用于表单元素）
- onkeyup：键盘按键弹起事件

例如：

```
btn.onclick=function(){}

```

## 四、函数的分类

#### 1.内置函数 alert（555）;

#### 2.自定义函数

#### 3.匿名函数  function(){}	btn.onclick = function(){}

###### 备注：没有名字的函数就叫做匿名函数

## 五、声明提前

###### 1.执行js代码前会将所有的声明提前到当前作用域的最前面

###### 2.当声明提前完成后，才从上往下执行js代码

![1534474298471](C:\Users\WANG\AppData\Local\Temp\1534474298471.png)

###### 备注：

###### （1）不能再赋值式函数前先使用函数（就是赋值式函数不能声明提前），这样会报错：zhengshu is not defined

例如：

```
正常的：var zhengshu = function(){console.log("666");}
var zhengshu;//声明变量
zhengshu();//声明提前：这一步就相当于加了上一步
zhengshu = function(){console.log("666");}
备注：代码在zhengshu（）;就终止了所以赋值式不能用提前声明

```

###### （2）关键字function声明的函数，可以在函数前后任意调用

```
正常的：function aaa(){console.log("8888");}
（1）声明提前
var aaa = new Function();//相当于新构建一个函数
        aaa();			//声明提前
（2）对变量赋值
        function aaa(){
            console.log("8888");
        } 

```

## 六、作用域

###### 定义：俗称“使用范围”，即能够使用某个变量的范围，分<全局作用域>和<局部作用域>

```
#### 1.全局作用域 ：放在函数最外层

#### 2.局部作用域：函数内

#### 3.全局变量：定义在全局作用域中的变量，在任意位置使用（放在函数的最外层）

#### 4.局部变量：声明在局部作用域的变量，只能在当前函数使用

```

例如：

```
 var a = 10; //全局变量
        // function sum(){
        //     var b = a + 10;
        //     console.log(b);//20
        // }
        // sum();
        
        function sum(){
            var b = 10;//局部变量
            function add(){
                var a = 20; //局部变量
                console.log(a);//20
            }
        }
        sum();
        var a = b + 10;
        console.log(a); //报错:b is not defined


```

备注：就近原则（如查找变量a）：

\* 使用变量a时先从当前函数查找，如果有则可以使用;

\* 如果当前函数无变量a,则往父级函数查找，如果找到则使用，并停止查找;

\* 如果在父级函数还是无法找到，则继续往上一层函数查找，以此类推;

\* 直到最顶层(全局作用域)，如果还是没找到，则报not defined错误;

#### 5.作用域链：当函数访问变量时，根据就近原则从内到外查询变量，这个路径称为作用域链。

## 七、函数的参数

#### 1.传参的作用：将值传入参数内

#### 2.形参：函数声明时的参数

#### 3.实参：实际参数，函数执行时的参数

备注：实参和形参的个数可以不一样

```
function sum(a,b,d){
        //     // 当执行这个函数时，其实进行了隐藏代码
        //     // （var a = 1;）//
        //     // （var b = 2;）//隐藏代码
        //     // 
        //     var c = a + b ;
        //     console.log(c);
        // }
        // sum(1,2,);

```

#### 4.arguments

函数内部隐藏的对象（是一个类数组），保存着实参的信息

arguments.length: 实参的数量

```
数组[]：一个变量存储多个值
       // 若想获取数组里面的某个值，通过索引（从0开始）获取： 数组名[索引]

```

## 八、返回值 return

#### 1.作用：将函数内部的值返回出去，需要一个变量接收

例如：

```
function sum(){
    var c = 10;
    return = c;
}
var d = sum();//接收变量,这里用函数名接收
console.log(d);

```

#### 2.如果函数没有return，执行的值返回undefined

#### 3.return；退出当前函数return往下的代码不会执行

###### 备注：return返回值返回的是它外面那一层，若是再外面一层想得到那个值，则需再return一次

#### 加：

#### 1.重复声明的变量无效

例如：

```
var a = 1;
var a ; //无效

```

#### 2.变量和作用域链

```
当前函数内没有定义该变量，继续往外找，直到找到该变量的声明。
若在函数内改变的是全局变量的值，则其他位置使用全局变量的值也会相应改变

```

### （一）this 当前对象，取决于谁调用了这个函数

```
1.执行函数的对象一般都是window
2.事件驱动执行函数，那么此时的this指向执行的函数

```

### （二）递归 ：函数自己执行自己

```
需要一个退出函数的条件return，若不存在退出条件会死循环
报错：Maximum call stack size exceeded  超出最大内存

```

### （三）回调函数

```
若想执行乙，但是需要甲的一个变量，选择在甲函数里面执行乙函数

```

例如：

```
function uname(fn){
            // var fn = show；
            fn("laoxie");
        }//甲
        function show(uname){
            // var uname = "laoxie";
            console.log(uname);
        }//乙
        
        //若想执行乙，但是我需要甲的一个变量。选择在甲函数里面执行乙函数
        uname(show);

```

# 第二周 第六天  8.20

## 数组

定义：一系类数据的集合，每一项可以保存任何类型的数据，称为数组的元素，每个元素用逗号隔开

数组格式：[1,2,3]

## 一、数组的定义 （声明）

```
1.字面量 var arr[];（推荐）
例如：var arr = ["laotian","laoxie","xiaoxie"];

```

```
2.使用构造函数创建数组
（1）var arr = new Array();//创建一个空数据
（2）var arr = new Array(n);//创建一个长度为n的数组(数组项都为undefined)
（3）var arr = new Array('王大锤',18 ,'普通青年','广州');//创建数组并同时写入数据

```

## 二、数组的操作（增删改查）

###### 1.数组的读取（查）与写入（改，增 。其实就是赋值）

 

```
*数组的索引	arr[index]
index 代表索引值，从0开始计数（代表的是数组中第几个元素，从0开始计算）
例如： 
	var arr["真香"，“躺赢”，“杨超越”]；
	arr[1];//==>躺赢  *读取
	arr[1] = "wsc";//==>写入，修改（把躺赢变成了wsc）
	arr[3] = "lemon";//增加，在后面又加了一个lemon
	arr.length = 1;//删除
	//打印数组
	  for(var i=0;i<arr.length;i++){
            console.log(i,arr[i]);
        }

```

###### 2.数组元素的删除

```
修改数组的长度 arr.length
例如：arr.length = 1;
解释：就是把数组的长度缩短了，后面的给删除了

```

###### 3.遍历数组

```
数组的长度 arr.length，索引的取值0到arr.length-1
解释：就是看一遍数组
例如：
var arr = ["真香","躺赢","杨超越"];
for(var i=0;i<arr.length;i++){
            console.log(i,arr[i]);
        }

```

![1534740069759](C:\Users\WANG\AppData\Local\Temp\1534740069759.png)

## 三、数组的方法

#### 1.增删改

```
push(元素，元素)	：往数组尾部添加一个或多个元素，用逗号隔开，返回数组新的长度
pop()			：删除数组最后一个元素，返回删除的元素
unshift（元素，元素）：往数组头部添加一个或者多个元素
shift（）			：删除数组第一个元素
splice(index,delNum,item)：
	index	代表的是索引（代表的是数组中的第几个元素）	
	delNum	要删除元素的数量		
	item 	添加的元素
	例如：
	arr.splice(2,1,"lemon");

```

#### *总结

| 方法                               | 返回值       |
| ---------------------------------- | ------------ |
| 增，例如push（）,unshift()         | 新数组的长度 |
| 删，改，例如pop(),shift(),splice() | 被删除的元素 |

#### 2.slice 切割

```
slice(start,end) 切割，将数组从start开始切割到end（不包括end所对应的元素），返回一个新数组
	*如果省略到end参数，则截取到数组的最后一项
	*支持负数，最后一个索引为-1，以次类推
	*原数组不受影响

```

###### 加：可用于复制一个数组为新数组，通过slice(0)

#### 3.join(分隔符)

```
*若分隔符参数省略，默认会将数组每一项用逗号拼接，返回字符串
*若分隔符参数存在，默认会将数组每一项用分隔符拼接，返回字符串

```

#### 4.concat 数组合并

```
返回一个新数组，这个新数组是由调用这个方法的数组和参数组成（原数组不变）

```

例如：

```
		var arr = ["莫赛", "何贵宇", "陈裕", "林宇鹏", "卢进球", "蔡景超"];
        var arr2 = ["荆轲","项羽","虞姬"];
        var arr3 = [1,2,3];
        console.log(arr.concat(arr2,arr3));
        console.log(arr);

```

![1534758855588](C:\Users\WANG\AppData\Local\Temp\1534758855588.png)

#### 5.sort 将数组中的元素排序，返回排序后的数组

```
默认以字符串以字符串的排列方式（转换成ASCII码进行对比）
sort(function(){return a-b;}) 数字从小到大排序
sort(function(){return b-a;}) 数字从大到小排序

```

例如：

```
		var arr = [10,666,444,2,545];
        var res = arr.sort(function(a,b){
            return b-a;
        });
        console.log(res);


```

### 四、数组的排序

#### 1.冒泡排序法

- 遍历：就是把数组中的元素一个一个取出来，想做什么看自己（遍历一般都用for循环）
- 遍历元素，跟其下一个元素对比
- 把最大的逐个往后排列
- 外层循环代表的是遍历的次数

```

```



```

```



#### 2.选择排序法

- 把当前元素分别跟后面所有元素对比
- 把最小的逐个往前排

例如：

```
 var arr = [10,2,444,245,1];
        for(var i=0;i<arr.length-1;i++){
            for(var j=i+1;j<arr.length;j++){
                if(arr[i]>arr[j]){
                    var current = arr[i];
                    arr[i] = arr[j];
                    arr[j] = current;
                }
                console.log(666);
            }
        }
        console.log(arr);

```

#### 快速排序法

```
利用递归函数实现排序
每次获取数组中间元素cItem
把大于和小于CItem的元素分别放置在arrGT和arrLt两个数组中
利用concat组合递归调用函数返回的值
直到数组的长度小于1时，直接返回元素调出递归

```

例如：

```
 function fastSort(arr){
            //5.避免死循环，满足数组长度小于1时，直接返回数组
            if(arr.length <= 1){
                return arr;
            }
            //1. 找出数组中间位置元素
            var cIdx = parseInt(arr.length/2);
            // 2. 通过splice(),改变原数组(去掉了中间那个数)。返回值为被删除的元素
            var cItem = arr.splice(cIdx,1);
            // 3.声明两个数组
            var arrGt = [];
            var arrLt = [];
            // 4.遍历arr,大于cItem的值，放在arrGt。小于的话放在arrLt
            for(var i=0;i<arr.length;i++){
                if(arr[i]>cItem[0]){
                    arrGt.push(arr[i]);
                }else if(arr[i] < cItem[0]){
                    arrLt.push(arr[i]);
                }
                console.log(666);
            }
            return fastSort(arrLt).concat(cItem,fastSort(arrGt));
        }
        console.log(fastSort(arr));


        // 数组的方法
        // 数组排序

```

## 五、数组的复制

#### 1.遍历，通过push

```
*先定义一个函数
*拟定一个为空的新数组
*通过for循环遍历
*再return出来
	例如
		var arr1 = [10,20,30];
		
		function copy(arr){
            var res = [];//拟定一个为空的新数组
            for(var i=0;i<arr.length;i++){
                res.push(arr[i]);//把每次循环得到的元素放进新数组中
            }
            return res;
        }
        var res1 = copy(arr1);
       console.log(res1);

```

#### 2.通过slice(0)

```
*直接切割原数组
*建立一个新数组接收
*var res1 = arr.slice(0)
	例如
		var arr1 = [10,20,30];
		
		var res1 = arr1.slice(0);
        res1.push("laoxie");

        console.log("arr1",arr1);
        console.log("res1",res1);


```

#### 3.map(arr)函数，把数组中的每一个数字都增加20%，并返回新的数组

```
var arr = [20,2,3];
function map(arr){
	var res[];
	for(var i=0;i<arr.length;i++){
       res.push(arr[i]*1.2);  
	}
    return res;
}
console.log(res);

```

#### 4.多维数组（数组里面包含数组）

###### 多维数组的获取与写入参考一维数组

# 第七天 8.21

## 一、对象Object

### （一）对象的定义

#### 1.创建对象

###### （1）字面量 var 变量名 = {键:值，键:值}

```
var laoxie = {name:xie,age:48,hobby:大保健,daughter:{}}

```

###### （2）构造函数 var变量名 = new Object();

```
var laoxie = new laoxie();

```

### （二）对对象的操作

#### 1.通过键值对操作对象

###### （1）对象.键		（2）对象["具体的键"]		对象[键的统称]

```
//方式1：点语法 obj.键
obj.sex;
//方式2：通过obj["具体的键"]
obj["sex"];
//obj[key] //key为所有键的统称变量，记住变量不加引号。

```

#### 2.添加、修改属性

```
解释：对对象的键值进行赋值
obj.sex = '男';
obj['weight'] = 60；

```

#### 3.删除键 delete

```
var obj = {name:'laoxie',age:18,gender:'man'}
//删除age属性
delete obj.age;

```

#### 4.读取键属性值

```
obj.name;//==>小明
//如果读取一个不存在的属性，返回undefined

```

#### 5.对象的遍历 for(var 键 in 对象){操作每个对象}

```
 for(var key in laoxie){
            console.log(key,laoxie[key]);
        }
   备注：这里的key是对所有的键的统称

```



## 二、es5新增数组方法

### （一）遍历（迭代）法法

#### 1.forEach(fn)

```
遍历方法，和for循环没有太大差别
*fn 指的是函数
	fn的三个形参
		item 第一个参数，代表数组的每一项元素
		index  第二个参数，代表数组的每一项索引
		arr  第三个参数，代表当前的数组

```

例如

```
 var arr = [1,2,3,666];
        arr.forEach(function(item，idx，arr){
            console.log(item,idx,arr);
        })

```

![1534851128448](C:\Users\WANG\AppData\Local\Temp\1534851128448.png)

#### 2.map(fn)

```
返回一个数量相等的数组，内容是什么，取决于fn中的返回值
	*fn 指的是函数
		fn的三个形参
            item 第一个参数，代表数组的每一项元素
            index  第二个参数，代表数组的每一项索引
            arr  第三个参数，代表当前的数组
     

```

```
       
	  var arr = [1,2,3,666];
        var res = arr.map(function(item,idx){
            return item*1.2;
        })
        console.log(res);


```



#### 3.filter(fn)

```
返回一个数组，存放执行fn后返回true的数组元素，利用这个方法可对数组元素进行过滤筛选
	*fn 指的是函数
		fn的三个形参
            item 第一个参数，代表数组的每一项元素
            index  第二个参数，代表数组的每一项索引
            arr  第三个参数，


```

```
 // 取出小于10的数组元素，并组成新数组
        var arr = [15, 16, 10, 15, 9, 0, 2, 17, 8, 18];
        var res = arr.filter(function(item){
            return item<10;
        });
        console.log(res);



```

#### 4.some(fn)

```
返回布尔值，如果该函数对任何一项都返回true，则返回true（只要有一个是true，则是true）


```

```
var arr = [15, 16, 10, 15, 9, 0, 2, 17, 8, 18];
        var res = arr.every(function(item,idx){
            return item>17;
        });
        console.log(res);
//只要有一个是大于17的就是返回true，所以这个是true


```

#### 5.every(fn)

```
如果该函数对每一项都返回true，才返回true(必须是所有的都是true，才是true)


```

```
var arr = [15, 16, 10, 15, 9, 0, 2, 17, 8, 18];
        var res = arr.every(function(item,idx){
            return item>17;
        });
        console.log(res);
//只有所有的都大于17，才返回true，所以这个是false


```

### （二）归并方法

```
reduce(fn,原始值)
	*fn的参数
		prev：上一次的返回值，第一次执行函数时，会将原始值当做prev的返回值，若原始值缺省，则拿当前数组的第一个元素作为prev的值
		cur：当前值（当前值为数组的每一项，第一次为第一项，第二次为第二项...）
		index：索引值
		arry：当前数组
			*原始值可以缺省


```

例如：

```
 var arr = [15, 16, 10];
 
 var res = arr.reduce(function(prev,cur){
            console.log(prev,cur);
            return prev+cur;
        },0)
        console.log(res);
        // prev     cur
        // 0         15
        // 0+15      16
        // 0+15+16   10



```

### （三）静态方法 Arry.is Arry

```
判断是否为数组，返回true/false


```

```
 var arr = {};
        console.log(Array.isArray(arr));
//返回false


```

### （四）索引方法

#### 1. `indexOf(keyword,startIdex)`

```
indexOf(keyword,startIdex)	//返回keyword所在数组中的索引值
	*keyword 要查找的项
		如果数组中不存在keyword，则返回-1
	*startIndex 开始查找的位置的索引，该参数默认为0


```

```
应用：判断数组是否存在某个参数
	if(arr.indexOf(keyword)) != -1{
        //说明该数组存在这个值
	}
	if(arr.indexOf(keyword) >= 0){
              //说明数组中存在这个值
              {


```

#### 2.lastIndexOf(keyword,[startIndex])

```
lastIndexOf(keyword,[startIndex])	//返回keyword所在数组中的索引值
	备注：这个也是从前往后的索引值，这个是为了找一样的值后（后面一点的）
	如果两个的值一样，就返回后面一点的索引。

```

# 第八天	8.22

# 字符串

```
定义：字符串就是一串字符，由双（单）引号括起来

```



## 一、创建字符串

#### 1.字面量

```
//方式一：字面量（推荐）
var str = '城市套路深，我想回农村';

//方式二：构造函数
//PS：用new产生的变量都是引用类型的变量，也叫对象
var str = new String('我不是黄蓉，我不会武功');

```

## 二、

#### 1. 属性：length获取字符串的长度

```
 var str1 = "good good study";
 console.log(str1.length);

```

#### 2.获取索引对应的值

```
（1）str(index);==>es5才出现	//index指的是索引，第几个就是几
（2）charAt(index)

```

例如：

```
console.log(str1[10]);//s
console.log(str1.charAt(10));//s	（字符串的名字和它用点连接）

```

#### 3.查找索引的方法

```
indexOf(keyword[,startindex])
	*从开头/尾部向后查找字符串keyword第一次出现的位置，如果没找到，则返回-1
			备注：返回一个数字
console.log(str1.indexOf("study"));		//返回s所在的索引

```

例如查找1~100里面包含7的和7的倍数的数字

```
for(var i=1;i<=100;i++){
    if(i %7 ==0 || String(i).indexOf("7") != -1){
        console.log(i);
    }
}

```

#### 4.split 字符串转换成数组

```
split(分割符) 根据分割字符，把字符串拆分成数组

```

例如：

```
	var str = "good good study";
        var arr = str.split(" ");
        console.log(arr);

```

![1534935030231](C:\Users\WANG\AppData\Local\Temp\1534935030231.png)

#### 5.replace 字符串替换方法

```
原字符串.replace(str||regExp,替换的值)返回被替换后的字符串，原字符串的值不受影响
	*备注：字符串的替换只能进行一次。不能够进行全局匹配，如果需要全局匹配，则应使用正则表达式
	备注：regExp为你上面自己定义的变量
		例如： var reg = /fuck/gi
	如果你的是个变量，则只能用构造函数的方式定义，(变量不加引号)括号里面的东西要加引号
		var reg = new regExp("fuck","gi");
		str.replace(reg,"**");

```

#### 6.slice 截取方法

```
（1）slice(start[,end])		截取start到end（不包括end）的字符串，支持负数
（2）substring(start[,end])	截取start到end（不包括end）的字符串
（3）substr(start,length)		索引支持负数，length为截取的数量
	
	备注：第1,2里面的start到end指的是从0开始截取到第几个
		第3个里面的length指的是从start开始往后截取的长度

```

例如：

```
		var str = "good goodaaaa GOODgooD Good study";
        console.log(str.slice(5,10));

```

![1534940434970](C:\Users\WANG\AppData\Local\Temp\1534940434970.png)

```
 var str = "good goodaaaa GOODgooD Good study";
 console.log(str.substr(5,5));

```

![1534940619208](C:\Users\WANG\AppData\Local\Temp\1534940619208.png)

## 三、正则表达式

#### 1.正则表达式的创建方式

```
（1）var reg = /值/gi;	//值指的是要替换的东西
（2）var reg = new RegExp("值"，"gi");
	*var reg = new RegExp(变量，"gi");

```

#### 2.正则表达式的参数

```
	*g	全局匹配
	*i	不区分大小写		//全局匹配的意思是，全局里面所有的要被替换的东西

```

## 四、ASCII码和字符集

#### 1.字符串charCodeAt(3)

```
 //获取下标为3的字符的编码	（3位索引）
 例如：var res = "老谢".charCodeAt(0);//32769
        console.log(res);
        备注：把“老“字 转换成数字编码32769

```

#### 2.String.fromCharCode(94)

```
//编码转成字符 
解释：就是通过数字得到相应的汉字
例如：String.fromCharCode(97) //"a"

```

## 五、Math

定义：一个保存数学公式和信息的对象，一般用于执行数学任务

#### 1.属性  Math.PI	//3.1415926

#### 2.方法：

```
        round(3.6) //四舍五入取整
        ceil(11.3) //12 向上取整
        floor(11.8) //11 向下取整
        random() //返回0-1之间的随机数（不包括1）
        max(num1, num2) //返回较大的数
        min(num1, num2) //返回较小的数
        abs(num) //绝对值
        pow(x,y) //x的y次方
        sqrt(num) //开平方根	

```

例如：

```
Math.ceil(-11.3) //-11 向上取整
Math.floor(11.8) //11  向下取整

```

```
三角函数复习
    sin(radian)
    cos(radian)
    tan(radian)
    
    角度与弧度的转换
    弧度=角度*Math.PI/180
    
    勾股定理复习
    在直角三角形中，斜边的平方等于直角边的平方和
    曲线方程复习(一元二次方程)

```

# 8.23 第九天

# 日期Date

### 了解时间

- GMT：格林尼治标准时(Greenwich Mean Time)，俗称“天文学时间”
- UTC：协调世界时(Universal Time Coordinated)，“原子物理时间”，它更加精确,50亿年才误差1秒
- 时区：为了克服时间上的混乱，1884年在华盛顿召开的一次国际经度会议（又称国际子午线会议[1]）上，规定将全球划分为24个时区（东、西各12个时区）。规定英国（格林尼治天文台旧址）为中时区（零时区）、东1-12区，西1-12区。每个时区横跨经度15度，时间正好是1小时
- 闰年：四年一闰，百年不闰，四百年再闰
- 纪元时间(UNIX TIME)：1970-1-1零时

## 一、时间 Date

#### 1.创建日期时间对象

```
（1）创建当前的时间和日期
	var d = new Date();
（2）创建的指定的时间和日期
	var d = new Date("2020/08/22");
	var d = new Date(666666);//解释：返回的时间就是1970/01/01 0:00加上你写的这个毫秒数 

构造函数
	无参数：得到的是代码执行的时间（本地时间）
	有参数：（1）字符串：指定日期，返回指定日期对应的时间
		   （2）数字 ：距离1970年1月1日0时0分的毫秒数
	

```

#### 2.日期时间对象的方法

##### *获取年月日

```
getFullYear()	/	setFullYear(2018)	
括号里面写你要获取的年份

getMonth()		/	setMonth(8)
括号里写你要获取的月份（获取月份是从0开始的，里面的8指的是7月，最好在后面加上1）

getDate（）			/	setDate(25)
返回日期，返回的是本地时间上的日期，不可修改！！！

```

##### *获取星期

```
getDay();	//返回 0~6代表的是星期日到星期六,获取的也是本地的星期几，也是不可修改

```

##### *获取时分秒

```
getHours()		/setHours()	//返回本地的 时
getMinutes()	/setMinutes()//返回本地的 分
getSeconds()	/setSconds()//返回本地的 秒

```

#### 3.设置方法

```
setFullYear(2018)	//设置年份，括号里为数字  表示自1970年到括号里面数字的毫秒数
setMonth(8)			//设置月份
setDate				//设置日期

- getTime()/setTime()：获取/修改某个日期自1970年1月1日0时以来的毫秒数
- toLocaleDateString(); 以特定地区格式显示年、月、日
- toUTCString(); 转换成UTC时间


```

#### 4.ES5方法

```
Date.parse("2015-08-24");	//返回指定日期距1970-1-1零时的毫秒数
	*转换格式默认支持2015-08-24或者2015/08/24
Date.now();	//返回 执行这行代码时距1970-1-1零时的毫秒数

```

例如：

```
 	var nowDate = new Date();
        var lastDate = new Date("2018-08-25"); 
        var offset = lastDate.getTime()-nowDate.getTime();
        var offset = Date.parse("2018-08-25")-Date.now();
        var tianshu = Math.ceil(offset/1000/60/60/24);
        console.log(tianshu);        

```

## 二、延迟与定时器

```
setTimeout(fn,200);	 两百毫秒后执行这个fn函数（只执行一次），返回一个id标识
clearTimeout(timer); 清除指定id标识的延迟操作
setInterval(fn,30)	 每隔30毫秒执行一次fn这个函数，返回一个id标识
clearInterval(timer) 清除指定id标识符的定时器操作

```

# 第十天	8.24

# BOM

## BOM的概念

BOM 是Browser Object Model（浏览器对象模型）的缩写，提供与浏览器窗口进行交互的对象。JavaScript语法的标准化组织是ECMA，DOM的标准化组织是W3C, 而BOM缺乏标准。这也是各种浏览器不兼容的根源所在

## window对象

window对象是BOM的核心, 是最顶层的对象，所有对象都是通过它延伸出来的。

### 全局作用域

- 定义在全局环境下的变量都会成为window对象的属性
- 把变量定义在函数体里，可以有效减少全局环境下的变量冲突，避免污染全局环境
- 在函数内部不用var声明的变量会成为全局变量，即window对象的属性
- window对象可以在代码中省略，如window alert()可以写成alert()
- 通过var在全局作用域下声明的变量用delete无法删除

```
var obj = {name:'xxx'}

//删除对象的属性用delete：
delete obj.name;

```

#### *备注

```
1.window的属性：name,top,避免使用
2.window的属性或者事件，一般都不省略window
3.记住尽量不要给window的属性赋值

```

## 一、window对象下的属性

#### 1.常用的属性

##### （1）浏览器的窗口尺寸

```
innerWidth	浏览器可视区域的宽度
innerHeight	浏览器可视区域高度
innerWidth/innerHeight, //表示浏览器窗口”可视区域”尺寸（能看见的地方）

outerWidth/outerHeight,	//表示整个浏览器的尺寸（屏幕的大小）

```

##### （2）滚动相关（方法）

```
scrollX/scorllY		//获取浏览器窗口滚动条滚动过的距离
scrollTo(x,y)		//设置浏览器滚动条与顶端距离
scrollToBy(xnum,ynum)//设置基于当前位置滚动的距离

```

#### 2.常用方法

##### （1）系统对话框

```
alert("666")		//弹出对话框（弹窗）

confirm("666")	//确认/取消框，返回布尔值

prompt(question,default)	//弹出输入框，返回值为输入的消息或者null
	prompt("请问你的大名","lemon")
	备注：以上是三个方法都会暂停代码运行

```

```
open("域名"，"名字","属性")
open(url,name,[options])	
//打开一个新窗口并返回新window对象（括号里面就是网址）
 *	name ：不命名会每次打开新窗口，命名的第一次打开新窗口，之后在这个窗口中加载
 	options：为字符串：'width=400,height=400,top=200,left=200'
 	opener父窗口对象，通过open方法打开的窗口才有opener
例如：
for(var i=0;i<3;i++){
            open("http://www.qq.com","qq"+i,'width=400,height=400,top=200,left=200');
        }
        
 close() 关闭窗口
 print() 调出打印框
 例如：
  setTimeout(function(){
            close();

        },3000)

```

#### 3.属性对象

```
document(核心)	文档对象，让我们可以在js脚本中直接访问页面元素(DOM)(获取元素)

```

###### （1）history(重要)

定义：历史对象，包含窗口浏览历史，可以实现后退

```
属性：
	length	返回浏览器历史列表中的URL数量

方法：back() 	加载history列表中的前一个URL
	 forward()加载history列表中的下一个URL
	 go()	  加载history列表中的某个具体位置，支持负数

```

```
history.back();//往前倒一个页面
history.forword();//往下一个页面
history.go(2);//向前两个页面
history.go(-2);//后退两个页面

```

###### （2）location（重要）

定义：location是BOM最有用的对象之一，保存着当前窗口中加载文档的相关信息，还提供一些导航功能，它是个很特别的对象，既是window的属性，也是document的属性 

```
hash	设置或返回从（#）开始的URL（锚）===>哈希值
href	设置或返回完整的 URL。
  * 修改href值 ：location.href = "html2/aa.html?id=1&name=iphone7&price=4000"
search	设置或返回从问号（？）开始的URL（查询部分）
  * 参数的作用：传递到另一个页面告知具体的显示信息


```

```
 encodeURI();//转码,将中文、特殊字符转成一定码
 decodeURI();//解码,将码转回中文、特殊字符

```

```
PS：修改以上属性(hash除外)都会刷新当前页面，并生成历史纪录

方法：

reload() 重新加载当前文档，带参数true表示不使用缓存刷新页面。

```

- navigator（了解）: 
  导航对象, 包含所有有关访问者浏览器的信息，通常用于检测浏览器类型
  - appName 浏览器名称
  - appVersion 浏览器版本
  - platform 操作系统
  - userAgent 用户代理信息，通过该属性可以获取浏览器及操作系统信息
  - geolocation 获取地理位置信息

### 二、window对象常用事件

#### 1.window对象常用事件

```
onload		//页面资源全部加载完成后触发这个事件
	例如：window.onload = function(){}

```

```
onscorll	//窗口滚动条滚动时触发
	例如：window.onscroll = function(){}

```

```
onresize	//窗口大小改变时触发

```

#### 加：offsetWidth	offsetHeight

```
获取元素的宽高	offsetWidth offsetHeight
	*获取的是content+padding+border的总宽高

```

# 第三周 8.27

# DOM

![1535980887699](C:\Users\WANG\AppData\Local\Temp\1535980887699.png)

## 什么是DOM

```
DOM是Document Object Model（文档对象模型）的缩写，它是W3C国际组织的一套Web标准。是针对HTML和XML文档的一个API，它定义了访问HTML文档对象的一套属性、方法和事件

```

## 一、节点类型

- 每个节点都有一个nodeType属性，用于表明节点的类型。
- 常用节点类型与nodeType值，用于判断元素属于什么类型节点

```
元素节点 <==> 1
文本节点 <==> 3
属性节点 <==> 2

/找出所有节点
<div class="content" title="属性节点">测试Div</div>

```

## 二、节点属性

#### 1.nodeType返回节点的类型

```
元素：1
文本：3
属性：2
解释：如若节点类型是元素，则返回1，是文本返回3，是属性返回2

```

#### 2.nodeName返回节点的名称，根据其类型

```
元素：标签名
文本：#text
属性：属性名

```

#### 3.nodeValue返回节点的值(元素节点的nodeValue为null)

```
元素：null
文本：文本内容
属性：属性值

```

## 三、获取元素节点

#### 1.document.getElementById()

```
document.getElementById("id")
	*通过id获取元素的节点（速度最快）
	*必须通过document调用
	*返回DOM节点对象，如果id不存在返回null

```

##### 如何获取body及html：

document.body获取body

document.documentElement获取html

#### 2.getElementsByTagName()

```
getElementsByTagName()
通过标签名获取元素节点列表
返回类数组，如果类名不存在返回空数组[]
	*元素节点均可用
备注：括号里面写标签名

```

例如：

```
var maolianjie = box.getElementsByTagName("a");

```

#### 3.getElementsByClassName()

```
getElementsByClassName()
通过class类名获取节点列表
返回类数组，如果类名不存在返回空数组[]

```

#### 4.document.getElementsByName()

```
document.getElementsByName()
通过那，name属性获取元素节点列表
必须通过document调用
返回类数组，如果name属性不存在返回空数组

```

## 三、利用节点关系获取到其他节点

#### 1.获取父级节点

```
ele.parentNode	/ parentElement		得到ele元素的父节点	
例如： <h1>获取节点</h1>
    <div id="box">
        <a href="#" >bilibili</a>
        <a href="#" class="bb">cilicili</a>
        <a href="#">ailiaili</a>
    </div>
	var baba = bb.parentNode;//得到#box

```

#### 2.获取子节点

```
ele.childNodes	/ ele.children			得到ele元素的全部子节点列表（类数组）
ele.firsiChild	/ele.firstElementChild	获得ele元素的第一个子节点
ele.lasiChild	/ele.lastElementChild	获得ele元素的最后一个子节点

```

例如：

```
<h1>获取节点</h1>
    <div id="box">
        <a href="#" >bilibili</a>
        <a href="#" class="bb">cilicili</a>
        <a href="#">ailiaili</a>
    </div>
var son = baba.childNodes;//此时son包含文本节点以及元素节点
var son = baba.children;

```

#### 3.获取兄弟元素节点

```
ele.nextSibling	/previousElementSibling 	获取ele元素的下一个兄弟节点
ele.previousSibling	 /previousElementSibling 得到ele元素的上一个兄弟节点

```

例如：

```
<h1>获取节点</h1>
    <div id="box">
        <a href="#" >bilibili</a>
        <a href="#" class="bb">cilicili</a>
        <a href="#">ailiaili</a>
    </div>
var first_mao = bb.previousSibling; //<a href="#" >bilibili</a>
var aili = bb.nextElementSibling;

```

## 四、节点的创建与插入

### （一）创建

#### 1.创建元素节点

```
document.createElement()	创建一个元素节点

```

#### 2.创建一个文本节点

```
document.creatTextNode()	创建一个文本节点

```

#### 3.创建一个属性节点

```
document.creatAttribute		创建一个属性节点

```

### （二）插入

```
parent.appendChild()		向节点的子节点列表的结尾追加新的子节点

```

```
parent.insertBefore(new,node) 在指定的子节点node前插入新的子节点new

```

```
ele.setAttributeNode(attrNode) 在指定元素中插入一个属性节点（了解）
//以上parent表示父级元素，ele表示元素
删除属性：removeAttribute(新建的属性)

```

##### 演示：利用创建节点方法，生成三种节点，并往元素节点插入内容及属性

```
//1.创建元素节点
var h3 = document.createElement("h3");
//2.创建文本节点，并往h3元素节点插入文本节点
var txt = document.createTextNode("啦啦啦");
h3.appendChild(txt);
//常用方法 =====> h3.innerHTML = "啦啦啦"；
//3.创建属性节点，并往h3元素节点插入属性节点
var title = document.createAttribute("title");
title.nodeValue = 'xxx';
h3.setAttributeNode(title)；
//常用方法 =====> h3.title = "xxx"
//4.将元素节点插入body里面
document.body.appendChild(h1);

```

##### 演示：insertBefore(),往子节点前面插入一个新节点

```
var h2 = document.createElement('h2');
h2.innerHTML = '哈哈哈';
document.body.insertBefore(h2,h3);

```

##### 案例:生成表格

```
//1.获取文本框、按钮、及输出元素
//2.封装表格函数（保证单一原则,即一个函数只做一件事）
	function createTable(r,c){
        //2.1 创建table>tbody>tr>td,记得插入对应的父元素内
        //2.2 将table返回出去
	}
//3.点击按钮时
	//2.1 获取行列值
	//2.2 执行生成表格函数
	//2.3 将表格插入输出元素
	//2.4 注意事项：每次插入前，记得清空上一次插入的内容
		output.innerHTML = '';
		output.appendChild(table);

```

##### 案例：自动应答机器人

```
// 1.获取输出元素ul、输入框及按钮
// 3.设置应答消息，用数组方式存放
	var q = '你好,在吗,约吗,十年了还约吗'.split(',');
	var a = '他好我也好,不是本人,叔叔在哪约,滚'.split(',');
// 2.点击按钮，发送信息（.active）
btn.onclick = function(){
	//2.1 发送信息（即在ul内插入li，并设置类名）：
	//2.2 发送自动应答信息（设置延迟n秒，setTimeout）
    // 注意：利用发送信息在q数组的索引，获取a数组中自动回复的内容
    var idx = q.indexOf(_msg);
    if(idx >= 0){
    	aLi.innerHTML = a[idx];
    }else{	
    	aLi.innerHTML = '你说什么？风太大我听不到';
    }	
    //2.3 清空内容，自动聚焦
    msg.value = '';
    msg.focus();
}   

```

## 五、节点的复制、删除、判断方法

#### 1.复制

```
当前节点.cloneNode(boolean)		复制节点，为true是深复制。返回值为复制后的新节点

```

#### 2.删除

```
父节点.removeChild(ele)		删除（并返回）当前节点parent的指定子节点ele

```

#### 3.判断

```
父节点.hasChildNodes()			判断当前节点是否拥有子节点，返回布尔值

```

##### 案例：表格删除、复制表格行

```
*添加行号
*添加删除按钮
*删除当前行（一定要书写在生成表格后）
	*获取所有按钮
	*分别给所有按钮绑定事件处理函数
for(var i=0;i<btnDels.length;i++){
	btnDels[i].onclick = function(){
		//console.log(i)//演示：不管点击哪个按钮，最终都会得到10（变量查找规则）
		//利用当前对象this，删除当前行tr、
	}
	//*添加复制功能，复制行
	btnCopies[i].onclick = function(){
        // 获取当前行
        var currentTr = this.parentNode.parentNode;
        // 复制tr
        var copyTr = currentTr.cloneNode(true);
        // ！！！问题：复制的tr没有事件，为什么，怎么解决？
        table.getElementsByTagName('tbody')[0].appendChild(copyTr);
    }
}

```

##### 演示：

```
1.判断父节点是否存在子节点
2.对已存在的元素进行插入操作的后果

```

### 六、元素节点的操作

### （一）操作的是DOM节点属性

> 可以通过点语法或方括号访问

- tagName 获取元素元素的标签名
- id 设置/获取元素id属性
- name 设置/获取元素name属性
- style 设置/获取元素的内联样式
- className 设置/获取元素的class属性
- innerHTML 设置/获取元素的内容（包含html代码）
- outerHTML 设置或获取元素及其内容（包含html代码）
- innerText 设置或获取位于元素标签内的文本
- outerText 设置(包括标签)或获取(不包括标签)元素的文本

### （二）操作html结构属性:

- ele.getAttribute(attr) //获取元素的属性值（自定义属性获取）
- ele.setAttribute(attr,val); //设置元素的属性
- ele.removeAttribute(attr) //删除属性attr
- ele.hasAttribute(attr) //判断是否存在属性attr

#### 演示：DOM节点及html元素的属性的关联及区别

```
<div id="box"></div>
<script>
	var box = document.getElementById('box');
	//(一)操作标准属性
	//1.操作dom节点属性，会影响到html元素。可通过控制台查看元素，多了[class]。
	box.className = 'mybox'; 
	//2.操作html元素属性，会影响到dom节点。可以通过ele.id查看对应的值。
	box.setAttribute("title","divBox");
	//（二）操作非标准属性
	box.man = 'lemon'; //不互相影响，可通过控制台查看元素，并没有任何改变
	box.setAttribute("love","you");//不互相影响，通过ele.love会发现值为undefined
</script>


```

## 七、盒模型相关

### 1.offsetLeft、offsetTop

```
offsetTop		当前元素离<定位父级>元素顶部的距离	（有定位的父级元素）
offsetLeft		当前元素离<定位父级>元素左边的距离
		*以上两个属性如果没定位的父级，则相对与根元素html的距离
offsetWidth		当前元素的宽度（border+padding+content）
offsetHeight	当前元素的高度（border+padding+content）

```

## 八、获取css样式(非内联样式)

```
window.getComputedStyle(ele,pseudo)	(标准)
	ele：要获取样式的元素	pseudo：伪元素样式字符（可选），可获取伪元素样式
ele.currentStyle	(IE8-)
	//注意事项：ie浏览器都不能直接获取css属性的值

```

###### 封装获取css样式的方法

```
function getCss(ele,key){
	// 思路：判断浏览器是否支持这个方法
	if(window.getComputedStyle){
		// 标准浏览器
		return getComputedStyle(ele)[key]
	}else if(ele.currentStyle){
		// IE8-
		return ele.currentStyle[key]
	}else{
		// 
		return ele.style[key]
	}
}


```

案例：tab切换

```
1）初始化
* 高亮第一个tab
* 隐藏除第一张以外的图片
* 给每个tab添加idx保存索引
2）切换：鼠标点击tab（关键：获取点击的index值，利用this.idx）
* 高亮显示当前tab,去除其他高亮
* 切换相应的图片，隐藏其他图片


```

# 8.28

# 一、Event事件

```
	事件是可以被JavaScript侦测到的行为。网页中的每个元素都可以产生某些可以触发JavaScript函数的事件.

	事件是一瞬间触发。

```

### （一）事件绑定方式

​	格式：节点 .on+事件名 = 事件处理函数;

```
div.onclick = function(){}
//<div onclick="sum()"></div> 不常用，不实用。
//结构、样式、行为相分离
//拿不到数据

```

## （二）常用事件

#### 1.鼠标事件

```
鼠标事件

onclick 当用户点击某个对象时调用的事件。

ondblclick 当用户双击某个对象时调用的事件。

onmousedown 鼠标按钮被按下。

onmouseup 鼠标按键被松开。

onmouseover 鼠标移到某元素之上。

onmouseout 鼠标从某元素移开。

onmousemove 鼠标被移动时触发。

onmouseenter 在鼠标光标从元素外部移动到元素范围之内时触发。 		 //这个事件不冒泡

onmouseleave 在位于元素上方的鼠标光标移动到元素范围之外时触发。 		//这个事件不冒泡，

oncontextmenu 鼠标右键菜单展开时触发。

PS：onclick = onmousedown + onmouseup, ondblclick = onclick*2(短时间内两次单击);

执行顺序：mouseover=>mouseenter; mouseout => mouseleave


```

#### 2.键盘事件

```
onkeydown	某个键盘按键被放下
onkeyup		某个键盘按键被松开
onkeypress	键盘<字符键>被按下触发，而且如果按住不放的话，会重复触发次事件

```

#### 3.UI事件

```
onload		页面元素（包括图片多媒体等）加载完成后
onscroll	滚动时触发
onresize	窗口或框架被重新调整大小

```

#### 4.表单事件

```
表单事件

onselect 输入框文本被选中。

onblur 元素失去焦点时触发。

onfocus 元素获得焦点时触发。

onchange 元素内容被改变，且失去焦点时触发。

onreset 重置按钮被点击。

onsubmit 确认按钮被点击。

oninput 输入字符时触发

```

##### 演示：常用事件

```
鼠标事件
* onclick
* onmousedown		
* onmouseup
* onmouover
* onmouseout
* onmousemove
结论：click = mousedown + mouseup
dblclick = click*2

```

## 二、Event对象

### （一）什么是event对象

​	

```
事件执行过程中的状态，用来保存当前事件的信息对象

```

### （二）如何获取event对象

```
ele.事件 = function(e){
	e = e || window.event;//获取event对象的兼容写法。IE8-：window.event
}

```

### （三）鼠标event对象的属性

#### 1.鼠标按键

#### button 返回当事件被触发时，哪个鼠标按钮被点击

```
W3C标准
	0：代表鼠标按下了左键
	1：代表按下了滚轮
	2：代表按下了右键

```

```
IE8-（IE8以下的浏览器）

1鼠标左键， 2鼠标右键， 3左右同时按， 4滚轮， 5左键加滚轮， 6右键加滚轮， 7三个同时

```

###### 演示：检测鼠标按键

```
box.onmousedown = function(event){
    switch(event.button){
        case 0:
            box.innerText = '射击';
            break;
        case 1:
            box.innerText = '换枪';
            break;
        case 2:
            box.innerText = '开镜';
            break;
    }
}

```

#### 2.光标位置信息

```
clientX /clientY		光标相对于浏览器可视区域的位置，也就是浏览器坐标
screenX	/screenY		光标指针相对于电脑屏幕的水平/垂直坐标
pageX	/pageY			鼠标相对于文档的位置
	
	*IE-8不支持
	  包括滚动条滚动的距离，即：	e.clientX+window.scrollX
offsetX，offsetY：光标相对于事件源对象的相对偏移量
	*事件源对象：触发事件的对象

```

###### 演示:检测光标位置

###### 案例：新闻提示信息

```
//1.给所有新闻绑定鼠标移入移出移动事件
for(var i=0;i<links.length;i++){
    links[i].onmouseover = function(){
    	//2.移入事件：
    		//2.1将title属性值作为details元素的内容
       		//2.2显示details元素
       		//2.3为了不让title默认行为影响，去除title属性
            this.bak = this.title;  // 2.3.1移除前备份title内容,下一次移入才不会没有没有内容
            this.removeAttribute('title'); // 2.3.2去除title属性
    }
    links[i].onmouseout = function(){
        //3.移出事件：隐藏details。重置title属性值
    }
    links[i].onmousemove = function(e){
    	//4.移动事件，设置定位
    }
}

```

### （四）键盘event对象的属性

```
which	/keyCode
	对于keypress事件，该属性声明了被敲击的键生成的Unicode字符码（ascii码）
	对于keydown和keyup事件，它指定了被敲击的键的虚拟键盘码。虚拟键盘码可能和使用的键盘布局有关

```

```
altKey	当事件被触发时，ALT键是否被按下。返回布尔值

```

```
ctrlKey	当事件被触发时，CTRL键是否被按下。返回布尔值

```

```
shiftKey 当事件被触发时，Shift键是否被按下。 返回布尔值

```

###### 案例：愤怒的小鸟

```
//键盘按下，根据上下左右移动小鸟
document.onkeydown = function(e){
	// 1.获取小鸟当前位置
    var top = bird.offsetTop;
    var left = bird.offsetLeft;
	//2.初始化速度及类名变量
    var speed = 10;
    var className = '';
    // 3.判断按下上下左右方向键,设置left值及类名变量值
    switch(e.keyCode){
        case 37:
            left -= speed;
            className = '';
            break;
        //同理其他方向
    }
    // 4.通过变量值，设置bird的位置，及类名
    bird.style.left = left + 'px';
    bird.style.top = top + 'px';
	bird.className = className;
}

```

## 三、事件冒泡

### （一）什么是事件冒泡：

```
在一个对象上触发某类事件，（如onclick），那么click事件就会沿着DOM树向这个对象的父级传播，从里到外，直至它被处理程序处理，或者到达了最顶层（document/window）

```

###### 演示：从里到外的元素添加相同的事件，查看事件冒泡

1）不是所有的事件都能冒泡。

​	以下事件不冒泡：blur、focus、load、unload…。

​	【onmouseover与onmouseenter的区别】

 2）冒泡到最顶层的目标不同。大部分浏览器到window对象，IE8-到document对象 

### （二）停止事件的传播

```
 标准：event.stopPropagation(); 
 IE8-：event.cancelBubble = true; 
 // 阻止事件冒泡兼容写法：
 if(e.stopPropagation){
 	e.stopPropagation();
 }else{
	e.cancelBubble = true;
 }

```

### （三）事件委托

​	利用事件冒泡原理，把本来绑定给某个元素的事件委托给它的父级（已经存在页面元素）处理。

###### 事件源对象：触发事件的元素

标准：event.target
IE8-：event.srcElement

###### 案例：表格删除当前行

```
//影响页面性能的三大操作：
	//* 事件数量
	//* dom节点操作次数
	//* 请求次数
output.onclick = function(e){	
	//兼容性问题
    e = e || window.event;
    var target = e.target || e.srcElement;
    if(target.className === 'btnDel'){
    	//this指的是谁?
        var currentTr = target.parentNode.parentNode;
        currentTr.parentNode.removeChild(currentTr);
    }else if(target.className === 'btnCopy'){
        var currentTr = target.parentNode.parentNode;
        currentTr.parentNode.appendChild(currentTr.cloneNode(true));
    }
}



```

# 8.29

## 一、阻止浏览器默认行为

> - 链接跳转
> - 表单提交
> - 右键菜单…
> - 文本的选择

- 标准：event.preventDefault();
- IE-8 :   event.returnValue = false;

###### 例：自定义右键菜单

```
document.oncontextmenu = function(e){
    e = e || window.event;
    //获取鼠标在文档中的位置
    e.pageX = e.pageX || e.clientX + window.scrollX;
    e.pageY = e.pageY || e.clientY + window.scrollY;
    //给菜单框添加位置样式
    contextMenu.style.left = e.pageX + 'px';
    contextMenu.style.top = e.pageY + 'px';
    contextMenu.style.display = 'block';
    //阻止浏览器的默认行为
    e.preventDefault ? e.preventDefault() : returnValue = false;
}
// 点击空白地方关闭右键菜单
document.onclick = function(){
	contextMenu.style.display = 'none';
}
contextMenu.onclick = function(e){
	e = e || window.event;
	//禁止事件冒泡
	e.stopPropagation ? e.stopPropagation() : e.cancelBubble=true;
}

```

### 加：影响js代码运行的事件

```
 1.添加事件

 2.请求次数
 
 3.频繁操作dom节点

```

## 二、事件捕获（反冒泡）

```
事件的传播
	（1）事件冒泡：从里到外
	（2）事件捕获：从上到下
			*监听器

```

## 三、事件监听器

```
标准浏览器：元素.addEventlistener(事件名，事件处理函数，是否捕获（默认false，为冒泡）)
	例如： btn.addEventListener("click",function(e){
            console.log("btn2");
        });
        	target.addEventListener("click",fn,false);
        备注：如果为冒泡，则可以省略false
     		

```

```
IE8- ：元素.attachEvent(on+事件名，事件处理函数)
target.attachEvent("onclick",fn)

```

- 可以绑定多个处理函数在一个对象上, 执行顺序按照绑定的顺序来(标准)

  - 不同元素事件执行顺序跟html结构有关
  - 相同元素事件执行顺序跟绑定先后有关

- 可以绑定多个函数在一个对象上, 执行顺序按照绑定的反序（ie8-

- ##### 演示:绑定事件的两种方式的区别

###### 封装：绑定事件，兼容浏览器

```
function bind(ele,type,handler,isCapture){
	// 优先使用事件监听器
	if(ele.addEventListerner){
		// 标准浏览器
		ele.addEventListerner(type,handler,isCapture);
	}else if(ele.attachEvent){
		// IE8-
		ele.attachEvent('on' + type,handler);
	}else{
		// DOM节点绑定方式
		ele['on' + type] = handler
	}
}

```

## 四、事件的移除

#### 1.DOM绑定事件的移除

```
ele.on+事件 = null；

```

#### 2.事件监听器移除

###### 标准：

```
removeEventListener("click",fn,true)//传入的参数fn要跟添加时一样(同一个函数)，否则不能移除事件

```

​	IE8-:

```
detachEvent("onclick",fn)，传入的参数fn要跟添加时一样，否则不能移除事件

```

###### 注意：

页面事件绑定数量越多，越影响性能（速度越慢）

#### 3.案例：拖拽效果

###### 拖拽的原理：

​	鼠标按下且移动鼠标时，改变当前元素的top,left值

##### 拖拽思路及案例演示

```
//给目标元素添加onmousedown事件
//- 拖拽的前提是目标元素设置css定位
//- 记录按下鼠标位置与元素左上角的偏移量offsetX，offsetY
box.onmousedown = function(e){
	var ox = e.offsetX;
	var oy = e.offsetY;
    //当onmousedown发生以后，此刻给document添加onmousemove事件
    // - 意味着此刻鼠标在网页的移动都将改变目标元素的位置
    // - 目标元素的left = 鼠标的pageX – ox
    // - 目标元素的top = 鼠标的pageY– oy
    document.onmousemove = function(e){
        box.style.left = e.pageX - ox + 'px';
        box.style.top =  e.pageY - oy + 'px';
    }
}
//给目标元素或者document（效果有差异）添加onmouseup事件，清空document的onmousemove事件
document.onmouseup = function(){
	document.onmousemove = null;
}		

```

###### 案例：给图片实现拖拽

###### 案例：实现复杂的拖拽效果

```
1.按拖拽原套路实现拖拽效果，唯一不同的在于初始鼠标位置与大盒子左上角初始偏移量获取
2.用数组记录mousedown、mouseover时的大盒子的定位坐标
3.mousedown，状态值改成true；mouseup，状态值改成false
4.mouseover过程，改变坐标元素的值：dragTop.innerText
h2.onmousedown = function(e){
	dragStatus.innerText = 'true';
    pos.push({x:box.offsetLeft,y:box.offsetTop})
   	//注意点1：
    var ox = e.clientX - box.offsetLeft;
    var oy = e.clientY - box.offsetTop;
    document.onmousemove = function(evt){
        var left = evt.clientX - ox;
        var top = evt.clientY - oy;
        box.style.left = left + 'px';
        box.style.top =  top + 'px';
		// 注意点2：取消文字选择
		evt.preventDefault();
		 pos.push({x:left,y:top});
        dragTop.innerText = top;
        dragLeft.innerText = left;
	}
}
document.onmouseup = function(){
    document.onmousemove = null;
    dragStatus.innerText = 'false';
}
//5.点击轨迹回放，定时器拿到数组的每个索引的值，赋值给box的样式。
//索引到达最后一个值的时候，清空定时器及数组
box.onclick = function(e){
    e = e || window.event;
    var target = e.target || e.srcElement;
    if(target.tagName.toLowerCase() === 'a'){
        var i=pos.length;
        var timer = setInterval(function(){
            i--;
            box.style.left = pos[i].x + 'px';
            box.style.top =  pos[i].y + 'px';
            dragTop.innerText = pos[i].y;
            dragLeft.innerText = pos[i].x;
            if(i<=0){
                clearInterval(timer);
                pos = [];
            }
	},50);
}

```



# 8.30

## 网络知识（了解）

### 通信协议

通信规则，设备与设备之间通信时共同遵守的规则

### TCP/UDP/IP

IP： Internet Protocol（网络之间互连的协议），规定了计算机在因特网上进行通信时应当遵守的规则

- IP地址：4个字节, 一共32位 ，用来标识设备在网络中的位置

TCP：Transmission Control Protocol（传输控制协议）

- TCP面向连接的协议（通信之前必须先建立连接）
- TCP相对可靠，它建立连接的过程称为3次握手
- 经历3次握手，才能建立连接
- 所有的消息传送，需要对方确认送达

> //正常通信
> A："土豆，土豆，我是茄子，收到请回答" 
> B："茄子，茄子，我是土豆，收到消息，有什么指示？"
> A："没事，没事，我以为你挂了呢" 
> A："开始传送消息..."   

> //如果对方没回应，则不断重复发送当前消息，直至对方收到回应为止。 
> A："茄子，茄子，我是土豆，我被人油炸了，现在改名叫薯片，收到请回答"
> ............ 
> A："茄子，茄子，我是土豆，我被人油炸了，现在改名叫薯片，收到请回答，第2遍"
> ............ 
> A："茄子，茄子，我是土豆，我被人油炸了，现在改名叫薯片，收到请回答，第3遍" 
> ............ 
> B："薯片，薯片，我收到消息"
> 因此可以确保数据的准确送达

UDP:面向数据报的协议 (不可靠的协议)，如果TCP比作是打电话，那么UDP就是在发短信

- 无需建立连接，发送消息也无需对方确认
- 无法保证数据的发送顺序，以及准确率
- UDP通常用于视频、语音等通信（丢掉了一帧画面是无所谓的）

### http/https

超文本传输协议HyperText Transfer Protocol，基于TCP协议的一种高级协议, 用于客户端和服务器直接的通信.

http的特点是，请求完成后就立即断开与服务器的连接

> 缺点:
> 通信使用明文（不加密），内容可能会被窃听
> 不适用特定的Web服务器，如：聊天室，消息广播

### socket

是一种通信模式，客户端与服务端一直保持着连接，用于随时传输数据

## 一、cookie

#### 1.cookie的概念

cookie 是客户端与服务器端进行通讯使用的一个能够在浏览器本地化存储的技术

> PS：chrome不支持本地文件的cookie读写

###### 演示：利用sublimeserver开启服务器，演示cookie的设置与获取（了解协议域名端口）

#### 2.cookie的基本设置及获取

```
设置:document.cookie = 'name=value'
	name：你要存的东西的名字
	value：要存的东西（字符串格式）
    * 一次只能写入一个cookie
读取:document.cookie
	* 一次性读取所有cookie（当前页面往上找，一直到根目录下的所有cookie）

```

###### 案例：保存图片拖拽位置

```
// 1.鼠标松开，保存图片位置。即设置cookie：保存left,top
document.cookie = 'left=' + girl.style.left;//100px
document.cookie = 'top=' + girl.style.top;//100px
// 2.页面加载，获取cookie：获取top,left
var cookies = document.cookie;//得到所有cookie
cookies = cookies.split('; ');
//3. 遍历数组，找出top,left,给图片设置位置
cookies.forEach(function(cookie){
    var arr = cookie.split('=');
    if(arr[0] === 'left' || arr[0] === 'top'){
    	girl.style[arr[0]] = arr[1];
    }
});

```

###### 案例:七天免登陆

```
btnSubmit.onclick = function(){
	// 5.表单submit按下即提交，不管满不满足条件。所以阻止默认行为
	e.preventDefault();
    // 1.获取用户名密码
    var _username = username.value.trim();
    var _password = password.value;
    //2.若用户名长度为0，退出函数。
    if(_username.length===0){
        alert('用户名不能为空');
        return;
    }
    //3.判断是否勾选"7天内免登陆"选项。若勾选保存cookie
    if(checkbox.checked){
        var d = new Date();
        d.setDate(d.getDate()+7);//d此时是一个UTC时间对象，转成字符串格式
    	document.cookie = 'username=' + _username + ';expires='+d.toUTCString();
    }
    //4.不管有没有勾选，点击提交，显示跳转页面
	location.href = 'http://www.baidu.com';
}
// 6.下一次访问：判断页面是否存在cookie，是否存在username的cookie，若存在自动登录，即自动跳转到百度
var cookies = document.cookie;
//（1）判断页面是否存在cookie，即cookie长度不为0
if(cookies.length>0){
    cookies = cookies.split('; ');
    cookies.forEach(function(item){
        var arr = item.split('=');
        //（2）是否存在username的cookie
        if(arr[0] === 'username'){
        	location.href = 'http://www.baidu.com';
        }
    });
}

```

### 二、cookie的组成部分

```
格式：'name=value[;expires=xx][;path=/][;domain=xxx]'
参数：
	expires：有效期
		默认Session：临时cookie（关闭浏览器会被清除）
		格式：'expires=' + d.toUTCString
	path：保存cookie的位置
		默认当前html所在目录
		格式：'path=/'	根目录（不设置默认在当前文件夹）
    domain：域名
    	默认：当前域名
读取：document.cookie（读取当前能访问的所有cookie）
	当前目录->根目录

```

### 三、封装cookie的操作

```
var Cookie = {
	get:function(key){
		// 1.先获取所有cookie，若cookie没有值，返回空字符串
		var cookies = document.cookie;
		if(cookies.length === 0){
			return '';
		}
        // 2.拆分每一个cookie
        cookies = cookies.split('; ');
        for(var i=0;i<cookies.length;i++){
            var arr = cookies[i].split('=');
            if(arr[0] === key){
                return arr[1];
            }
        }
    },
    set:function(key,value,date,path){
    	//拼接字符串
        var str = key + '=' + value;
        if(date){
            str += ';expires=' + date.toUTCString();
        }
        if(path){
            str += ';path='+path;
        }
        document.cookie = str;
    },
    remove:function(key,path){
    	//获取过期的日期，重新设置cookie
        var d = new Date();
        d.setDate(d.getDate()-1);
        this.set(key,'x',d,path);
    },

    // 清空cookie
    clear:function(){
    }
}

```

### 四、cookie的限制

> 数量50个（不同浏览器值不同）
>
> 大小2m（不同浏览器值不同）
>
> 只能写入字符串

### 五、JSON

```
* 转换
    * 对象/数组 -> json字符串：JSON.stringify()
    * json字符串 -> 对象/数组：JSON.parse()
* 格式：
    * 属性名和字符串必须使用双引号
    * 不能有注释
    * 不能存在多余逗号
* 属性值必须为以下类型
    * String
    * Number
    * Boolean
    * Object
    * Array
    * Null
    
    注意：JSON.parse("") ==>如果传入的是空字符串，会报错

```

案例：将商品添加到购物车列表

```
// 3.每次刷新，拿到上一次的存放值。第一次是为空数组
// * 若已经存在值，默认为JSON字符串，要转回数组
var goodslist = Cookie.get('goodslist') || [];
if(typeof goodslist === 'string'){
    goodslist = JSON.parse(goodslist);
}
// 1.利用事件委托实现添加到购物车的效果
goods.onclick = function(e){
    e = e || window.event;
    var target = e.target || e.srcElement;
    if(target.parentNode.className === 'add2cart'){
        // 2.若当前为按钮被点击
        // （1）生成一个商品信息对象{guid，name，imgurl，price，qty（商品数量）}
        // （2）推入数组，将数组添加到cookie里面
        // （3）考虑如果商品信息已经添加过，则应该增加数组里面的该商品数量
        // 	* 第一步:判断当前的guid是否在数组存在。
        //  * 第二步:若存在，拿到该商品信息在数组中的索引，利用索引将qty++
        var currentLi = target.parentNode.parentNode;
        var guid = currentLi.getAttribute('data-guid');
        var idx;
        var has = goodslist.some(function(g,i){
            idx = i;
            return g.guid === guid;
        });
        if(has){
            goodslist[idx].qty++;
        }else{
            var goods = {
                guid:guid,
                name:currentLi.children[1].innerText,
                imgurl:currentLi.children[0].src,
                price:currentLi.children[2].innerText,
                // 商品数量
                qty:1
            }
            goodslist.push(goods);
        }
        document.cookie = 'goodslist='+ JSON.stringify(goodslist);
    }

```

##### 加：trim();

```
移除两侧的空白字符（解释：就是不让空白的东西也提交）

```

# 9.3

# 正则表达式

## 了解正则表达式

- 什么是正则表达式
  正则表达式(regular expression)是一个描述字符模式的对象。
- 为什么要使用正则表达式
  正则表达式能够进行强大的“模式匹配”和“文本检索与替换”功能。前端往往有大量的表单数据校验的工作，采用正则表达式会使得数据校验的工作量大大减轻

## 一、创建正则表达式

### （一）使用RegExp构造函数

第一个参数就是我们的模式“字符串”

```
var reg= new RegExp('study');

//使用特殊字符
var reg= new RegExp('\\d\\w+');\d\w+

```

第二个参数可选，模式修饰符

- i: case-insensitive，表示忽略大小写
- g: global，表示全局匹配
- m: multiline，表示多行匹配

```
var reg = new RegExp('study', 'ig');

```

### 还可以用字面量方式直接声明

```
var reg = /study/gi;

```

- 直接量是字符匹配，不支持变量

## 使用正则表达式

### 支持正则表达式的字符串方法

#### 1.search

```
search
返回第一次匹配时所在的索引值,如果匹配不到则返回-1

```

#### 2.match

```
match 
默认匹配字符串，返回一个数组
0:所匹配的字符
    - index:匹配第一个字符所在的索引
    - input:对字符串的引用
  	- 全局匹配(g)，返回一个匹配所有字符串数组
  	- 如果匹配不到则返回null

```

#### 3.replace

```
- replace
  替换字符串
- split
  `'a,b ,c , d, e'.split(/\s*,\s* /);`

```

#### 4.split

```
a,b ,c , d, e'.split(/\s*,\s* /)`

```

### 二、正则表达式的属性和方法

测试正则表达式用test方法,返回布尔值

- 格式：正则表达式.test(字符串)

- 用<正则表达式>测试<字符串>是否匹配,返回true/false

- 测试正则表达式exec方法

  ```
   /xx/.exec(字符串)
  
  ```

  ```
  PS: 1）数量词*,+,{5,}，会尽可能多的去匹配结果（贪婪）
  	2）在后面加一个?表示尽可能少的去匹配结果（非贪婪） google,goooogle ==> /go+/ 
  
  ```

  ```
  格式：正则表达式.test(字符串)
  
  - 用<正则表达式>测试<字符串>是否匹配,返回true/false
  判断如果不满足正则表达式时，阻止默认提交表单的默认行为
  	表单验证： if(!/^正则表达式$/).test(字符串){return false;}
  		例如：if(!/^[a-z][\w\-]{5,19}$/i.test(username)){
              		alert("你的用户名不满足条件");
              		return false;
  
  ```

#### 1.匹配规则

```
所有字母和数字都是按照字面量进行匹配,和字符串匹配等效
/good/gi

字符类（只记小写字母即可）

. : 除换行以外的字符
\w : 代表数字或字母或下划线
\W : 非数字字母和下划线字符
\d : 数字
\D : 非数字
\s : 代表一个空格
\S : 空格以外的字符
\b : 匹配一个单词边界，也就是指单词和空格间的位置
\B : 匹配非单词边界。

```



###### PS:以上所有字符类都只是匹配“一个”字符

#### 2.特殊符号

```
^ $ . * + ? = ! : | \ / () [] {}
[]: 代表任意“单个字符” ,里面的内容表示“或”的关系

-: 代表范围
^: 代表非
(): 表示分组（n是以最左边括号出现的顺序排列）

$1: 表示第一个分组
$n: 表示第n个分组（不能写在正则表达式里）
\n: 在正则分组后面使用，表示对第n个分组的引用(一定要写在正则表达式里)
PS: 编写的正则分组数量越少越好
|: 表示或者

```

#### 3.锚点定位

```
^: 表示以什么开头	（写在前面）
$: 表示以什么结尾 （写在后面）
表示数量，对前一个字符计数，

*: 代表0个或0个以上 <===>{0,}
+: 代表1个或1个以上 <===>{1,}
?: 代表0个或1个 <===>{0,1}
{}:
\d{5}: 匹配5个数字
\d{5,10}: 匹配5个到10个数字
\d{5,}: 匹配5个或5个以上的数字
PS:
1）数量词*,+,{5,}，会尽可能多的去匹配结果（贪婪）
2）在后面加一个?表示尽可能少的去匹配结果（非贪婪）
google,goooogle ==> /go+/



```

```
[案例]

快速替换html标签
去除首尾空格
提取手机号码
表单验证
验证账号
不能为空，
不能使用特殊字符（数字、字母、下划线、横杠），
必须以字母开头，
长度6-20
昵称只能输入中文
Unicode编码中的汉字范围 /^[\u2E80-\u9FFF]+$/
电子邮件
jinrong.xie@qq.com
x@qq.com
x@163.com
x@a-r.com.cn
密码
长度小于20
不能包含空格
身份证
18/15位
445655 19900707 2165
445655 19900707 211x
手机号码
生日 
1999/05/08
1999-5-8
19990508
[练习]

邮政编码检测
文件格式检测
邮箱格式检测
[作业]

Alt text

表单验证
登录名
必填
数字或字母组合
不能少于3位
昵称
中英文皆可
电子邮件
必填
密码
必填
至少6位
显示密码强度
弱：只有数字
一般：数字字母组合
强：数字字母特殊字符组合

```

# 9.3

# ES5

## 支持ES5的浏览器

> Opera 11.60+
>
> Internet Explorer 9+  (IE9不支持严格模式)
>
> Firefox 4+
>
> Safari 5.1+
>
> Chrome 13+

## 页面加载事件

#### DOM文档加载的步骤为

1. 解析HTML结构。
2. 加载外部脚本和样式表文件。
3. 解析并执行脚本代码。
4. DOM树构建完成。//DOMContentLoaded
5. 加载图片等外部文件。
6. 页面加载完毕。//window.onload

## 一、页面加载事件

#### 1.redaystatechange

```
readystatechange事件（准备阶段状态改变，两个状态）
	*interactive	:DOM树完成执行
	*complete		:页面加载完毕后执行，类似window.onload，但比它先执行

```

#### 2.DOMContentLoaded

```
 DOMContentLoaded事件
	*DOM树完成执行
	*必须使用事件监听器绑定
备注：以上事件用以取代window.onload事件（实际开发不常用window.onload）
	*例如：
	document.addEventListener("DOMContentLoaded",function(){
    console.log("DOMContentLoaded");
})	//跟window.onload用法一样

```

###### 演示：通过控制台打印查看执行顺序

```
document.onreadystatechange = function(){
    if(document.readyState === 'interactive'){
    	console.log(iteration);
	}
	if(document.readyState === 'complete'){
        console.log('complete');
	}
}
document.addEventListener("DOMContentLoaded",function(){
    console.log("DOMContentLoaded");
})
document.onload = function(){
    console.log("onload);
}

```

## 二、ES5的严格模式

```
定义：除了正常模式，ES5添加了第二种运行模式：“严格模式(strict mode)”。顾名思义，这种模式使得javascript在更严格的条件下运行(更可靠，更安全)。目前，除了IE6-9，其它浏览器均已支持ES5严格模式。

```

#### （一）为什么要用严格模式

- 消除javascript语法的一些不合理，不严谨的地方，减少一些怪异行为；
- 消除代码运行的一些不安全之处，保证代码运行的安全；
- 提高编译器效率，增加运行速度；
- 为未来新版本的javascript做好铺垫

###### 举例子：

```
function sum(){
    a = 10;
  	//在普通模式下，若在函数内不使用var声明变量，会默认变成全局变量
  	//为了改变现状，出现ES4版本，然而变动太大，未被使用
  	//出现ES5作为过渡阶段，存在两种模式
}

```

#### （二）如何使用ES5

###### 在头部写入"use strict"

```
全局：针对整个js文件
	*将"use strict"放在js文件的第一行（就上放在script标签的下面）
局部：针对单个函数
	*将"use strict"放在函数体的第一行（就是放在function下面）

```

例如：

```
<script type="text/javascript">
        "use strict";		//全局严格模式
        function sum(){		//局部严格模式
            "use strict";
            arguments[3] = "lemon";
            console.log(arguments);
            // num = 10;//在函数内不通过var声明的变量，浏览器会把它当做全局变量
        }
        sum(10,20,30);
        // console.log(num);

        // 全局污染、变量名相同就覆盖了。
        // 
        // delete obj.uname;
    </script>	

```

### （三）ES5执行限制

- 不使用var声明变量严格模式中将不通过

- 删除系统内置的属性会报错

- 不能删除var声明的全局变量（会自动成为window的属性）

- 对象有重名的属性将报错

  - var obj={name:"小王",name:'王大锤'}

- 函数有重名的形参将报错

  - function sum(a,a,b){}

- arguments严格定义为参数

  - 不允许对arguments赋值
  - 禁止使用arguments.callee

- 函数必须声明在顶层，不能写在条件判断语句或for循环语句中

  var arr = [10,2,3,50];
  if(arr.length>3){
      function sum(){//报错}
  }

## 三、获取元素节点

#### 1.querySelector(css选择器)

```
querySelector("css选择器")
	获取匹配选择器的第一个节点，返回DOM节点 （就是你获取的即使是一个 类名，它给你返回的也是第一个类名所在的元素）
	备注：括号里面要加双引号

```

例如：

```
      var h3 = document.querySelector(".erzi");
        console.log(h3);

```

![1535982410029](C:\Users\WANG\AppData\Local\Temp\1535982410029.png)

```
querySelectorAll("css选择器")
	获取匹配选择器的所有元素，返回数组
		备注：对比用getElementsByClassName()等方法获取到的类数组，querySelectorAll()可以使用forEach()方法。

（学会查看控制台！！！）

```

例如：

```
   var h3 = document.querySelectorAll("#box .erzi");
        console.log(h3);

```

![1535982714697](C:\Users\WANG\AppData\Local\Temp\1535982714697.png)

## 四、Function方法

#### 1.bind()

​	定义：用于将当前函数和指定对象绑定（改变this指向），返回一个新的函数

​	解释：就是你把bind（this）绑定在哪个函数上，它的this就变成了你绑定的那个this

例如：

```
<input type="button" value="按钮1" />
    <input type="button" value="按钮2" />
    <input type="button" value="按钮3" />
    <input type="button" value="按钮4" />
    <input type="button" value="按钮5" />
    <script type="text/javascript">
        var btn = document.querySelectorAll("input");
        //1.点击按钮，控制台输出当前被点击按钮的索引
        for(var i=0;i<btn.length;i++){
            btn[i].idx = i;//给每个btn对象都添加一个属性idx，值就是当前索引
            btn[i].onclick = function(){
                // console.log(i);//因为i是全局变量，for循环执行效率很快，已经递增到5.此时再点击执行函数，拿到的都是i最终的值为数组长度。
                console.log(this.idx); 
                // this当前执行函数的对象。
                //  * 若是事件触发的函数，都指向事件源对象。
                //  * 若是普通函数，大部分的this都指向window。
            }
        }
        //2.点击按钮，一秒后，控制台输出当前被点击按钮的索引
        for(var i=0;i<btn.length;i++){
            btn[i].idx = i;
            btn[i].onclick = function(){
                var self = this;
                setTimeout(function(){
                    console.log(self.idx); 
                },1000)
            }
        }

        for(var i=0;i<btn.length;i++){
            btn[i].idx = i;
            btn[i].onclick = function(){
                // 四、函数的方法
                // bind() 用于将当前函数和指定对象绑定(改变this指向)，返回一个新的函数
                setTimeout(function(){
                    console.log(this.idx); 
                }.bind(this),1000) //将触发点击事件函数的事件源对象this传入当前函数。
            }
        }


        // var yinliao = "water";
        // function sum(){
        //     console.log(this);
        // }
        // sum.bind({name:"laoxie",yinliao:"shenbao"})();


    </script>

```

## 五、获取class的属性

#### 1.classList 类数组，包含了所有类名

```
length：class类名的个数
add（）：添加class方法					//在括号里面写你要添加的类名，加双引号
remove() : 删除class方法
toggle() : 切换class方法
contains():是否含有某个类,返回布尔值

```

## 六、data自定义对象

#### 1.dataset对象

```
//1.符合W3C标准自定义属性：data-*
<div id="box" data-name="laoxie" data-age="18" data-first-name="xiexie"></div>

//2.dataset：存放所有data自定义属性的对象。
//(1)获取
dataset.age;//获取data-age的属性值
dataset.firstName;//获取data-first-name的属性值
//(2)设置
dataset.gender="girl"；//设置data自定义属性，在html结构会多出[data-gender="girl"]
	例如： box.dataset.gender = "zhong";
//回顾：操作任意自定义属性（可以是非标准的）
//setAttibutte（）
//getAttibute（）

 // 任意自定义属性
        box.setAttribute("love","yiyi");
        box.getAttribute("data-first-name");


```

# 9.4	ES6

## 一、变量声明

#### 1.（一）let：变量声明

```
（1）变量声明不会提前		//就是你在哪声明的边量就作用到哪
（2）let不允许相同作用域内多次声明同一变量
（3）块级作用域{}		//大括号里面称为块级作用域，你在块级作用域声明的let别的地方拿不到

```

例如：

```
  var a;
        let a = 10;			相当于：let a = 10;
        var a = 20;					let a = 20;
        console.log(a);
        //  报错：Identifier 'a' has already been declared 变量a已经被声明

```

![1536033505825](C:\Users\WANG\AppData\Local\Temp\1536033505825.png)

#### 2.const:声明常量

```
（1）变量声明不会提前
（2）块级作用域
（3）const不允许相同作用域内多次声明同一变量
（4）声明后的值无法修改

```

###### 演示：

```
const MY_NAME = 'laoxie';
// 报错：无法修改常量的值
MY_NAME = 'LEMONE';
//演示：PI、Number()内置的一些常量属性

```

> const常用于引用第三方库的声明

## 二、解构

```
声明变量时，从数组和对象中提取值，对变量进行赋值，这被叫做“解构”

```

### （一）数组解构

```
var [a,b] = [1,2];
console.log(a,b);//var a=1，b=2；

var [a,...b] = [1,2,3,4]; //...表示获取剩余参数
console.log(a,b); //var a=1，b=[2,3,4]；

//(1)解构失败，得到undefined
var[a,b,c,d] = [10,20,30]；
console.log(a,b,c,d);//d解构失败：数组arr中无对应索引值
var [a] = 1；//a解构失败，对应的右边不是数组，无法解构

//（2）指定默认值：
var [a=true]= 1; //当a解构失败的话，拿到默认值

```

### （二）对象解构

```
var obj = {name:"lemon",age:18};
var {name,age} = obj; // var name="lemon",age=18；
//(1)解构失败，得到undefined
var {username,age} = obj;//username解构失败，变量必须与对象属性名相同，否则为undefined

//(2)如果变量名与属性名不相同，则必须写成以下格式才能取到值
var {name:username,age} = obj; //声明的变量为username，解构obj中的name属性 
							//相当于：var username="lemon",age=18;
//(3)指定默认值：
var {a=10} = {};//当a解构失败的话，拿到默认值

```

### （三）应用

#### 1.交换变量值

```
var x = 10;
var y = 20;
var[x,y] = [y,x];	//相当于var x=20; var y = 10;

```

#### 2.函数返回多个值

```
//数组：
function example(){
    return [1,2,3]
}
var [x,y,z]	= example();
//对象：
function example(){
     return {name:"lemon",age:18};
}
var {name,age} = example();

```

#### 3.定义函数形参

```
//数组：
function test([x,y,z]){
    //相当于 var [x,y,z] = [1,2,3];
}
test([1,2,3]);
//对象：
function test({name,age}){
    //相当于 var {name,age} = {name:"lemon",age:18};
}
test({name:"lemon",age:18});

//常规操作：参数可以设置默认值
fuction test({x=0,y=0,z=0}){
    //相当于var {x=0,y=0,z=0} = {x:10}
    //为避免没有实参值传入，给形参默认值
}
test({x:10});

//扩展：若形参是基本数据类型，函数也可以对形参进行设置默认值的操作。
var func1 = function(x=1,y=2){return x+y}；
func1(); // 得到 3
//同样，也可以用...表示获取剩余参数
var func2 = (x, ...args) => { console.log(args) };
func2(1,2,3); // 输出 [2,3]

```

## 三、字符串扩展

### （一）字符串方法

#### 1. includes

```
判断是否包含某个字符，返回布尔值
	*'html5'.includes('html');	//true

```

#### 2. startsWidth/endsWidth

```
是否以某一字符或某一字符串开头/结尾
    let str = 'google';
    str.startsWidth('goo');	//true
    str.endWidth('e');		//true

```

#### 3. repeats(n)

```
得到的字符串重复n次后的结果，n可以为小数，但不能为负数
	'laoxie'.repeats(2);	//laoxielaoxie

```

### 4.字符串模板template string（重点）

```
使用反引号``表示，你可以通过一种更加美观、更加方便的方式向字符串中插入变量
格式： $(变量|函数)

```

```
`你好，我的名字叫${username},接下来是我的自我介绍：${introduce()}`

```

备注：模板字符串中所有的空格、新行、缩进，都会原样输出在生成的字符串中。

## 四、箭头函数arrow function（重点）

### （一）基本操作

- 格式：标识符=>表达式
- 省略了function、return关键字、圆括号、花括号

#### 1.函数内只有一句return代码，可以省略{}及return

```
1.零个参数用()表示

var sum = function(){return 10+10;}	//箭头函数： var sum = () =>10+10;
	*省略了function和return

```

```
2.函数只有一个参数（可以省略括号）

var test = function(x){return x+2;} //箭头函数 var test = x =>x+2;

```

```
3.函数有多个参数，用（参数）表示
var test = function(x,y){return x+y} //箭头函数 var test = (x,y) =>x+y;

```

#### 2.函数内包含多行代码时用代码扩起来

###### *备注：ES6中的规则是，紧随箭头的{}被解析为块的开始，而不是对象的开始

```
//ES5
	btn.onclick = function(e){
        e= e || wiodow,event;
        var keCode = e.which ||e.keyCode
        console.log(keyCode);
	};

//ES6
	btn.onclick = e =>{
        e= e || wiodow,event;
        var keCode = e.which ||e.keyCode
        console.log(keyCode);
	}
备注：只要有花括号，就不能省略return

```

#### 3.当使用箭头函数返回一个普通对象时，需要将对象包裹在小括号里

```
//传统写法
var createPerson = function(){
    return {name:'laoxie',age:18};
}

//ES6
var createPerson = ()=>{name:"laoxie",age:"18"};	//这样写会报错
var createPerson = ()=>({name:'laoxie',age:18}); 
备注：因为它不知道你的对象还是块的开始，所以要用小括号包裹起来

```

###### 总结：

```
（1）function均可省略
（2）函数内有一个参数可以省略小括号
（3）函数内有两个或两个以上的的参数不能省略小括号
（4）函数内有多句执行代码，则不能省略花括号，有花括号则不能省略return
（5）若你要返回的是一个对象，需要将花括号括在小括号里面（此处可以省略花括号）

```

### （二）箭头函数this的值

```
箭头函数没有它自己的this值，箭头函数的this值会继承自外围作用域

```

例如：

```
    <input type="button" value="按钮1" />
    <input type="button" value="按钮2" />
    <input type="button" value="按钮3" />
    <input type="button" value="按钮4" />
    <input type="button" value="按钮5" />
    <script type="text/javascript">
        var btn = document.querySelectorAll("input");
        for(var i=0;i<btn.length;i++){
            btn[i].onclick = function(){
                // 这里this指的是事件源对象
                setTimeout(()=>{
                    console.log(this);
                    // 箭头函数没有自己的this，this继承自其外围作用域。
                },1000)
            }
        }
    </script>

```



## 五、生成器函数 Generators

```
function和函数之间有一个*号
yield：暂停代码执行
return：终止函数
next():执行后的到一个对象，有两个属性如下：
	value ：暂停时返回的值（yield）	//yield的值就是就是value的值
	done  ：表示函数是否执行完毕

```

例如：

```
  function* sum(){
            console.log(1);
            yield 50;
            console.log(2);
            yield 100;
            console.log(3);
            yield 150;
        }
        var obj = sum(); 
var obj = sum();//得到一个状态为suspended的对象{next()}
// obj.next();//得到一个对象：{value:xx,done:false}
console.log(obj);

```

![1536059587544](C:\Users\WANG\AppData\Local\Temp\1536059587544.png)

## 六、Set

#### 1. Set集合

```
概念：（1）Set集合，类似于数组，但是成员的值也是唯一的，可自动去重。
	 （2）去重的前提是两个值恒等于
引用数据类型创建多个，即使值一样也不恒等于，因为它们地址不同

```

#### 2. Set方法

- add(value)：添加某个值，返回Set结构本身。
- delete(value)：删除某个值，返回一个布尔值，表示删除是否成功。
- has(value)：返回一个布尔值，表示Set集合中是否存在该值。
- clear()：清除所有成员，没有返回值。

```
let imgs = new Set(); //创建一个set集合
imgs.add(1); 
imgs.add(1);
imgs.add(5);
imgs.add("5"); 
imgs.add({name:"lemon"}); 
imgs.add({name:"lemon"});
//打印的结果： 1  5  '5'  {name:"lemon"} {name:"lemon"}

```

#### 3. 利用set去重数组

```
var arr = [1, 2, 3, 4, 5, 5, 5, 5]；
let items = new Set(arr);
//去重后将set集合重新转成数组
arr = Array.from(items)；

```

###### 备注：Array.from()方法就是将一个类数组对象或者可遍历对象转换成一个真正的数组。

###### 那么什么是类数组对象呢？所谓类数组对象，最基本的要求就是具有length属性的对象。

#### 4.遍历set集合

- forEach()
- for…of

```
set.forEach((item,idx)=>{
    console.log(item,idx);
})

var imgs = new Set(['a','b','c']); //根据KEY遍历 
for(let item of imgs){
     console.log(item); 
} 

```

#### 5.for...of

- 这是最简洁、最直接的遍历数组元素的语法
- 这个方法避开了for-in循环的所有缺陷
- for…of跟for-in的区别很明显，就是直接取值，而不再取下标了
- 与forEach()不同的是，它可以正确响应break、continue和return语句

```
var arr = [10,12,18,30];
for (var value of arr) {
  console.log(value);
}

```

> 只要有[迭代器Symbol(Symbol.iterator)  ]就可以用for...of遍历
>
> - Array			
> - DOM
> - Set/Map集合
> - String
> - 不支持普通对象

## 七、对象扩展（重点）

### （一）对象的合并方法

```
Object.assign(obj1,obj2,…objN); 合并对象到obj1，返回obj1

```



```
var obj1 = {a:1}；
var newObj1 = Object.assign(obj1,{b:2});
//1.合并对象到obj1,所以obj1 = {a:1,b:2}
//2.返回obj1，传递给newObj1，所以newObj1 = {a:1,b:2}

var newObj2 = Object.assign(obj1,{b:2},{b:4,c:3});
//若存在相同属性，后面的覆盖前面的。//newObj=obj1={a:1,b:4,c:3}


```

扩展：对象的传递与复制 

```
var obj = {
    name:"laoxie",
    hobby:['大保健','money']
}
//1.对象的传递：
var newObj = obj; //此时修改obj的任意属性，也会同时影响newObj
//2.对象的复制
//（1）for...in遍历复制
for(var key in obj){
	newObj2[key] = obj[key];
}
//（2）利用assign（）
var newObj3 = Object.assign({},obj);
//注意：以上两种复制方式，都只支持浅拷贝（对于引用类型，只拷贝引用）
obj.hobby.push('羽毛球');//此时也会影响newObj2与newObj3

//（3）深拷贝
var newObj3 = JSON.parse(JSON.stringify(person))；

```

```
   var obj = {name:"lemon",age:17,hobby:["睡觉","讲故事"]};
        var newObj = Object.assign({},obj);
        newObj.age = 16;
        newObj.hobby.push("唱儿歌");
        console.log(obj,newObj);
   备注：*浅拷贝
   			拷贝的只有地址，你改变newObj的hobby，其他的也会改变

```

### （二）对象简写

> ES6允许在对象之中直接写变量，如

```
//1. 属性简写
var myName = 'laoxie';
var obj = {myName};//等效于var obj = {myName:'laoxie'}。变量名作为属性名，变量值作为属性值。

//2.使用变量值作为属性名
var obj = {
    [myName]:18 //等效于 laoxie:18
}

//3.方法简写
var obj = {
    coding(){} //等效于 coding:function(){}
}


```

## 八、Map集合

js对象（Object）只能用字符串当作键(属性名)。这让它的使用有了很大的限制。所以ES6推出了一种类似于对象的数据集合：Map集合，它能让所有类型的数据作为键

### 常用方法

- 设置set(key, value)
- 获取get(key)
- has(key)
- delete(key)
- clear()

```
//创建：
let map = new Map(); 

//设置：
map.set('name','laoxie');
map.set(6,666);
// 把数组作为键
var arr = [10,20,30];
map.set(arr,'数组');

//获取：
map.get(arr); //[10,20,30]


```

### 遍历方法

- keys() 获取所有键，可以用Array.from()转成数组
- values() 获取所有值，可以用Array.from()转成数组
- entries() 获取所有键值对，可以用Array.from()转成数组
- 循环遍历，配合解构赋值 for...of

```
for(var item of map){
    console.log(item); //每个item得到的都是一个数组，索引0为键，索引1为值
} 
//解构写法：
for(var [key,value] of map){
    console.log(key,value);
}


```

## 九、Symbol数据类型

ES6引入了一种新的原始数据类型Symbol，表示独一无二的值，一旦创建后就不可更改，是一种类似于字符串的数据类型，但Symbol 值不能与其他类型的值进行运算，否则报错。

#### 1. symbol的创建

```
// 没有参数的情况
var s1 = Symbol();
var s2 = Symbol();
s1 === s2 // false

//Symbol函数可以接受一个字符串作为参数，表示对Symbol实例的描述，主要是为了标识和区分，对调式非常有用
// 有参数的情况
var s1 = Symbol("foo");
var s2 = Symbol("foo");
s1 === s2 // false

//Symbol值不能与其他类型的值进行运算


```

#### 2.symbol的用途

- 给对象创建私有属性
- 给现有的对象添加属性，可能会产生命名冲突，Symbol的出现解决这个问题

```
var attr = Symbol();

// 第一种写法,不用加引号
var a = {};
a[attr] = 'Nani';

// 第二种写法（注意加方括号，否则回被当作普通属性）
var a = {
	[attr]: 'Nani';
};

// 以上写法都得到同样结果
a[attr] // "Nani"


```

Symbol.for() 登记symbol,会先查找当前Symbol是否存在

```
// 存在：则引用，不存在：则创建登记
var s11 = Symbol.for('laoxie');//创建一个Symbol
var s12 = Symbol.for('laoxie');//引用一个Symbol
//注意：直接使用Symbol()创建的Symbol值的键不会被登记，所以也就获取不到


```

# 9.5 Animation

## （一）运动原理

不断改变对象的属性产生动画的效果

## （二）动画分类

#### 匀速运动

速度保持不变的运动

##### 案例：飞翔的小鸟

```
//1.获取元素及初始化速度变量
let bird = document.querySelector('img');
let speed = 7;
//2.设置定时器
let timer = setInterval(()=>{
	//2.1 获取元素当前位置
	let left = bird.offsetLeft;
    //2.3 边界处理
    if(left >= window.innerWidth - bird.offsetWidth){
        left = window.innerWidth - bird.offsetWidth -speed;
        clearInterval(timer);
    }
    //2.2 将当前位置+速度变量值，更新赋值给当前元素的位置样式
    bird.style.left = left + speed + 'px';
},20);	

```

##### 案例：圆周运动

```
//1.获取太阳、地球半径
var sun_r = 155;
var earth_r = 15;
//2.设置太阳居中,太阳左上角的定位
sun.style.left = (window.innerWidth-sun.offsetWidth)/2 +'px';
sun.style.top = (window.innerHeight-sun.offsetHeight)/2 +'px';
//3.设置地球初始角度
var deg = 0;
getPos(deg);
//4.设置定时器，实现角度改变
setInterval(function(){
    deg +=5;
    getPos(deg);
},30)
//设置地球左上角的位置
function getPos(deg){
    var rad = toRad(deg);
    var a = sun_r*Math.sin(rad);
    var b = sun_r*Math.cos(rad);
    var x = window.innerWidth/2+a-earth_r;
    var y = window.innerHeight/2-b-earth_r;
    earth.style.left = x +'px';
    earth.style.top = y +'px';
}
//角度转弧度
function toRad(deg){
    return deg*Math.PI/180;
}

```

#### 加速运动

速度不断增加的运动

##### 案例：自由落体

```
//其实就是比匀速运动多了速度变量更新而已！！！
//1.获取元素及初始化速度变量	
let ball = document.querySelector(".ball");
let speed = 1; 
//2.设置定时器
let timer = setInterval(()=>{
	//2.1 获取元素当前位置
    let top  = ball.offsetTop;
    //2.2 更新速度变量
    speed++;
    //2.4 边界处理
    if(top >= window.innerHeight-ball.offsetHeight){
        top = window.innerHeight - ball.offsetHeight-speed;
        clearInterval(timer);
    }
    //2.3 将当前位置+速度变量值，更新赋值给当前元素的位置样式
	ball.style.top = top + speed + 'px';
}, 20)

```

#### 减速运动

速度不断减小的运动

##### 案例：刹车运动

```
//减速运动边界处理时，更多判断的是速度！！！
//1.获取元素及初始化速度变量
var car = document.querySelector('.car');
var speed = 60;
//2. 设置定时器
var timer = setInterval(()=>{
	//2.1 获取元素当前位置
    var left = car.offsetLeft;
    //2.2 更新速度变量
    speed -= 3;
   //2.3 速度边界处理
    if(speed<=0){
        speed = 0;
        clearInterval(timer);
    }
	//2.4 将位置更新赋值给当前元素的样式
	car.style.left = left + speed + 'px';
},50);

```

#### 抛物线运动

水平方向速度不断减小，垂直方向速度不断增加

##### 案例: 抛球不反弹

```
//垂直方向加速与水平方向减速的结合
//1.获取元素及初始化速度变量
var basketball = document.querySelector('.basketball');
var xspeed = 20;
var yspeed = 0;
//2. 设置定时器
var timer = setInterval(()=>{
	//2.1 获取元素当前位置
    var left = basketball.offsetLeft;
    var top = basketball.offsetTop;
	//2.2 更新速度变量
    yspeed++;
	xspeed -= 0.01;
	//2.3 边界判断
    if(top >= window.innerHeight - basketball.offsetHeight){
    	top = window.innerHeight - basketball.offsetHeight - yspeed;
        clearInterval(timer);
    }
	if(xspeed <= 0){
    	xspeed = 0;
    }
	//2.4 将位置更新赋值给当前元素的样式
    basketball.style.left = left + xspeed + 'px';
    basketball.style.top = top + yspeed + 'px';
},30);

```

##### 案例:抛物线的重力回弹

#### 缓冲运动

一开始速度很快，然后慢下来，直到停止

 缓冲运动的关键：动态计算速度（一般都跟目标值-当前值相关）

##### 案例：点击返回顶部

```
//1.window.onscroll事件，实现当window.scrollY的值大于一定的值时，出现点击返回顶部按钮
window.onscroll = ()=>{}
//2.给按钮绑定点击事件（事件触发定时器，一般都要先清除上一次的定时器）
totop.onclick = ()=>{
	clearInterval(timer);
    //2.2 开启定时器
    var timer = setInterval(()=>{
    	//2.2.1 获取元素当前位置
		var scrollTop = window.scrollY;
        //2.2.2 根据当前位置，更新速度变量值
        var speed = parseInt(scrollTop/10);
        // 2.2.3 边界判断
        if(speed<=10){
            speed = 10;
            clearInterval(timer);
        }
        //2.2.4 滚动到位置更新的位置
		window.scrollBy(0,-speed);
	},30);
}

```

##### 案例：图片展示上移效果

```
for(let i=0;i<cols.length;i++){
	cols[i].onmouseenter = function(){
        clearInterval(this.timer);
        // 1.获取当前a标签及设置目标值
        let link = this.children[1];
        let target = 0;
        //2.鼠标移入（不想冒泡就用enter）,设置定时器拿到当前top及设置缓冲速度。
        this.timer = setInterval(()=>{
            let current = link.offsetTop;
            let speed = Math.ceil((current-target)/10);
            current -= speed;
            if(current <= target){
                clearInterval(this.timer);
                current = target;
            }
            link.style.top = current + 'px';
        },30);
    }
}
//鼠标移出，回复原来的位置。

```

#### 透明度变换

##### 案例：图片的淡入淡出

```
box.onmouseover = function(){
	//4.多次进入事件，清楚上一次的定时器
    clearInterval(timer);
    timer = setInterval(function(){
    	//1.鼠标移入，设置定时器，获取当前透明度*100.
        var cur = getComputedStyle(img).opacity*100;
        //2.具体的change看你想做什么运动。缓冲运动
        var change = Math.ceil((100-cur)/10);
        cur += change;
		//3.当获取到的当前透明度+change值>=100时，设置当前透明度的值。清除定时器
        if(cur >= 100){
            cur = 100;
            clearInterval(timer);
        }
        //3.透明度改变的值除于100，给元素赋值样式
        img.style.opacity = cur/100;
    },100)
}
//鼠标移出，回复半透明效果。

```

## （三）动画的封装

```
// 缓冲运动原理，利用(target-current)/10得到速度
function animate(ele,attr,target){
    clearInterval(ele.timer);
    if(attr == "opacity"){target *= 100;}
    //1.定时器:
    //(1)获取ele的attr属性值，可能存在px、deg、target获取单位及数值
    //(2)设置缓冲速度
    //(3)设置当前属性值，判断达到目标值，清除定时器
    //(4)设置给元素作为样式
    //2.考虑透明度
    //3.函数一进来，先清除定时器，避免事件触发重复添加
    ele.timer = setInterval(function(){
        var current = getComputedStyle(ele)[attr];
        var unit = current.match(/[a-z]+$/i);
        unit = unit ? unit[0]: "";
        current = parseFloat(current);
        if(attr == "opacity"){current *= 100;}
        var speed = (target-current)/10;
        speed = speed>0? Math.ceil(speed) : Math.floor(speed);
        current += speed;
        if(current == target){
           clearInterval(ele.timer);
        }
        if(attr == "opacity"){current /= 100;}
     	ele.style[attr] = current + unit;
	},100)
}

```

​        Animation(下)

##### 案例：利用封装的代码，书写轮播图

```
//（一） 定时切换图片
//1.初始化索引
var index  = 0；
let timer = setInterval(function(){
	//2.设置定时器让索引递增，改变图片的top值为，为-图片大小*索引
    index++;
    //3.当索引大于等于图片数量时，将索引重置为0
    if(index >= ul.children.length){
        index = 0;
    }
    ul.style.top = -320 * index +'px';
}, 1000)

```

```
//（二） 利用封装animate实现动画
//1.初始化索引
var index  = 0；
let timer = setInterval(autoPlay, 1000)
lbt.onmouseenter = ()=>{
	clearInterval(timer);
}
lbt.onmouseleave = ()=>{
	timer = setInterval(autoPlay,1000);
}
function autoPlay(){
    //2.设置定时器让索引递增，将-图片大小*索引作为每次动画的目标值
    index++;
    //3.当索引大于等于图片数量时，将索引重置为0
    if(index >= ul.children.length){
        index = 0;
    }
    var target = -320 * index;
    animate(ul,"top",target);
}

```

## 完善animate封装

```
function animate(ele,opt,callback){
	// 2.记录动画的数量，遍历时加1。执行后减1。动画结束后执行回调函数
	let timerLen = 0;
    // 1.遍历opt，获取所有attr和target
    for(var attr in opt){
        timerLen++;
        createTimer(attr);
    }
    function createTimer(attr){
        let target = opt[attr];
        // 3.1设置定时器的名字与attr关联
        let timerName = attr + 'timer';
        // 3.2清除定时器，避免多个定时器用作于一个效果
		clearInterval(ele[timerName]);
		ele[timerName] = setInterval(()=>{
            let current = getCss(ele,attr);//100px,45deg,0.5(string)
            let unit = current.match(/[a-z]+$/i);//[0:px,index:6,input:current],null
            unit = unit ? unit[0] : '';
            current = parseFloat(current);
            let speed = (target-current)/10;
		   speed = speed>0 ? Math.ceil(speed) : Math.floor(speed);//1,-1
		   current += speed;
		   if(current === target ){
				clearInterval(ele[timerName]);
				// 每一个动画完成数量减一
				timerLen--;
				// 动画结束后执行回掉函数
                if(timerLen === 0){
                    typeof callback==='function' && callback();
                }
             }
             ele.style[attr] = current + unit;
		},30);
	}
}			

```

##### 案例：实现一个动画结束后再改变字体颜色之类的效果

##### 案例：链式动画

##### 案例：水平无缝滚动

```
2）无缝滚动
    * 把第一张复制到最后
ul.appendChild(ul.children[0].cloneNode(true));
1）获取ul子元素的长度设置ul宽度，达到水平排列的效果
let len = ul.children.length;
let imgWidth;
ul.querySelector('img').onload = function(){
	imgWidth = this.offsetWidth;
	ul.style.width = imgWidth*len + 'px';
}
3）水平轮播效果
let timer = setInterval(autoPlay,3000);
function autoPlay(){
    index++;
    show();
}
function show(){
	//当show()执行到最后一张图片len-1时，代表索引为0的图片。
	//再次进入autofocus，index++后，其实要执行的下一次索引应该为1。所以要把当前位置改成0.
    if(index >= len){//0,1,2,3,4
        ul.style.left = 0;
        index = 1;
    }
    animate(ul,{left:-imgWidth*index});
    // 遍历所有页码，取消高亮，给点点被点击的页码添加高亮
    for(let i=0;i<len-1;i++){//0,1,2,3
        page.children[i].className = '';
    }
    if(index === len - 1){
        page.children[0].className = 'active';
    }else{
        page.children[index].className = 'active'
    }
}
4）移入移出，清除轮播效果
focus.onmouseenter = ()=>{clearInterval(timer);}
focus.onmouseleave = ()=>{timer = setInterval(autoPlay,3000);}
5）添加分页效果，点击分页切换
let page = setPage();
function setPage(){
    let page = document.createElement('div');
    page.className = 'page';
    for(let i=1;i<len;i++){
        let span = document.createElement('span');
        span.innerText = i;
        if(i===1){
            span.classList.add('active');
        }
        page.appendChild(span);
    }
    focus.appendChild(page);
    return page;
}
focus.onclick = e=>{
    if(e.target.parentNode.className === 'page'){
        index = e.target.innerText-1;
        show();
    }
}
6）添加前后按钮，实现上一张、下一张的效果（待完成...）

```

案例：瀑布流

```
(1)获取图片宽,计算当前容器能容纳多少列
//	* 列数 = parseInt(容器宽度/图片宽度)
let imgWidth = items[0].offsetWidth;
let col = Math.floor((window.innerWidth-17)/imgWidth);//10.6
//2）计算水平间隔
//    * 间隔 = （容器宽度-17）%图片宽度/(列数+1)，17为滚动条宽度
let gap = ((window.innerWidth-17)%imgWidth)/(col+1);
// 3）创建一个数组pos
//	  * 用来保存第一行每列图片左上角坐标(left,top)
let pos = [];
for(let i=0;i<col;i++){
    pos.push({
        left:(i+1)*gap + i*imgWidth,
        top:gap
    })
}
// 4）遍历所有图片，往容器里添加图片
    //  当前图片加载时，遍历数组pos，查找最小top值及对应的索引，给当前元素设置样式
    //  然后更新当前索引，即minIdx的top值,top = 容器高度（由图片高度跟上一次gap撑开） + gap 
for(let i=0;i<items.length;i++){
    let currentImg = items[i].querySelector('img');
    // 等图片加载完成获取div高度
    currentImg.onload = function(){
        let minIdx = 0;
        let minTop = pos[minIdx].top;
        for(let j=1;j<pos.length;j++){
            if(pos[j].top < minTop){
                minTop = pos[j].top;
                // 更新最小索引值
                minIdx = j;
            }
        }
        animate(items[i],{left:parseInt(pos[minIdx].left),top:parseInt(pos[minIdx].top)})
        // 然后更新当前top值
        pos[minIdx].top += gap + items[i].offsetHeight;
    }
}             

```

# 第一天 9.10

# 一、wampserver安装及使用

### 1. wampserver安装

- a:安装 Web 服务器Apache
- p:安装 PHP解析器
- m:安装MySQL数据库

> 对于初学者建议使用集成的服务器组件（如：WampServer），它已经包含了 PHP、Apache、Mysql 等服务,免去了开发人员将时间花费在繁琐的配置环境过程。

WampServer下载地址：<http://www.wampserver.com/>

若是缺乏某个dll，直接安装[vc_redist.x64_2015.exe](./anzhuangbao/vc_redist.x64_2015.exe)

【计算机-管理-服务和应用程序-服务-wampapache-wampmysql（开启服务前，先停止svn、mysql、iis）】

> 测试：
>
> 当wampserver图片变成绿色：
>
> 1. 网址中输入localhost或127.0.0.1（本机ip），默认打开C:\wamp64\www路径下的index.php
> 2. 同样可以localhost/*** 访问默认路径下（C:\wamp64\www）的任意文件

### 2.创建虚拟目录

- 左键小图标---->apache---->alias directories--->add an alias 
- 创建虚拟目录名字，例如aaa。enter后
- 创建虚拟目录对应的url，即需要开启web服务的文件夹路径(路径不可有中文、空格)
- 以上步骤完毕，访问虚拟目录只需在浏览器输入http://localhost/aaa，可访问目录下任意文件。

### 3.创建端口

- 左键小图标---->apache---->httpd-vhost.conf

- 复制如下代码，往下写。（//只是注释，记得删掉）

- ```
  listen 1704    //端口号
  <VirtualHost *:1704>      //端口号
  	ServerName localhost
  	DocumentRoot D:\laoxie\01Basic      //端口对应url(不可有中文路径、空格)
  	<Directory  "D:\laoxie\01Basic">    //端口对应url
  		Options +Indexes +Includes +FollowSymLinks +MultiViews
  		AllowOverride All
  		Require all granted     
  	</Directory>
  </VirtualHost>
  
  ```

  以上步骤完毕，访问端口下目录只需在浏览器输入http://localhost:1704，可访问目录下任意文件。

### 4.开启局域网服务器

​	1.查看本机ip地址：common+r进入cmd，输入ipconfig，查看ipv4。

​	2.在vhost.conf给端口对应的url添加一句代码

```
#Require local //#代表注释
Require all granted    //允许其他主机访问

```

# 二、PHP

#### 1.概念

```
PHP是一种通用开源服务端脚本语言，将程序嵌入到HTML文档中去执行，结果以纯 HTML 形式返回给浏览器。

PHP: Hypertext Preprocessor “超文本预处理器”，1994年由Rasmus Lerdorf创建，刚刚开始仅仅是为了要维护他本人个人网页而制作的一个简单程序（Perl语言编写），原名Personal Home Page（PHP由此得名），后用C语言重新编写，改名Hypertext Preprocessor


```

##### PHP能做什么：

- 生成动态页面内容
- 创建、打开、读取、写入文件
- 收集ajax数据
- 发送和接收cookie
- 添加、删除、修改您的数据库中的数据
- 限制用户访问您的网站上的一些页面
- 加密数据

#### 2.基本语法

```
默认文件扩展名是“.php”
通常包含HTML标签和一些PHP脚本代码

```

##### 2.1 分界标

```
	<?php	//开始
	
	//在这里写php代码
	
	>		//结束

```

##### 2.2 注释

```
与js一样，分单行注释和多行注释
	*单行注释	//
	*多行注释	/**/

```

##### 2.3 输出语句

##### *echo

可以输出一个或多个字符（字符串可以包含HTML标签），速度较快，一般用于向前端返回数据

###### *备注：echo 返回的必须是字符串形式，它可以直接输出到页面上

例如：

```
<?php
    //输出一个字符
    echo "Hello world!<br>";
    //输出多个字符
    echo "This", " string", " was", " made", " with multiple parameters.";
?>

```

```
json_encode(array,JSON_UNESCAPED_UNICODE);  把数组转成字符串
	php5.4+ 使用JSON_UNESCAPED_UNICODE防止中文转义
json_decode(json,assoc);把字符串转成数组/对象
	json：待解码的 json string 格式的字符串
	assoc：默认false,返回object, 当该参数为 true 时，将返回array

```

- print_r
  打印关于变量的信息，适用于数组、对象的打印，一般用于测试
- var_dump
  判断一个变量的类型与长度,并输出变量的数据类型和数值，一般用于测试

#### 3. 变量

##### 3.1 命名规则

- 以$符号开始，后面跟着变量的名称（$称为标识符，不属于变量的组成部分）
  - 就像var，let一样的作用，声明变量
- 只能包含字母、数字字符以及下划线，不能以数字开头（不能包含空格）
- 区分大小写

```
//PHP 没有声明变量的命令，也没有声明提前的概念
//变量在第一次赋值时被创建
	<?php
		$txt ="Hello world";
	?>

```

#### 4. 拼接字符串及变量

```
<?php
	 $myname = "lemon";  
    echo 'My name is' . $myname;  //1.通过并置运算符.拼接字符串及变量
    //或者
    echo "My name is $myname"； //2.双引号内可以直接输出变量，无需拼接
?>

	备注：这里的 . 就想当于js中的 + 号

```

#### 5. 函数中访问全局变量

- 全局变量：在函数外部定义的变量，可以任意位置访问（需要手动定义为全局变量）
- 局部变量：函数内部声明的变量，仅能在函数内部访问

##### （1）$GLOBALS

```
<?php
    $x='global x';
    function myTest(){
        //echo $x;//报错 Undefined variable:未声明定义的变量
        echo $GLOBALS['x']; //1.获取全部变量正确写法：$GLOBALS[变量名]，其中变量名不带$。

        //2.同时，可以在函数中创建全局变量
        $GLOBALS['y'] = $GLOBALS['x'] + $GLOBALS['y'];
    } 
    myTest();
    echo $y;
?>

```

（2）global 关键字

```
    <?php
        $x=5;
        function myTest(){
            global $x;
            $y=$x;
        }
        myTest();
        echo $y; 
    ?>

```

##### （2）超级全局变量

- `$GLOBALS`
  是PHP的一个包含所有全局变量的数组，可以在任意位置使用
- `$_SERVER`
  是一个包含了头信息(header)、路径(path)等信息的数组
- `$_POST / $_GET`
  被广泛应用于收集表单数据，常用于ajax请求等操作
- `$_COOKIE`
  用于收集前端发送过来的cookie数据
- `$_REQUEST`
  变量包含了 `$_GET、$_POST 和 $_COOKIE` 的内容
- `$_SESSION`
  服务器版cookie
- `$_FILES`

##### （3）常量

- 规范
  - 命名规则与变量一致，但常量名不需要加$修饰符。
  - 常量值被定义后，在脚本的其他任何地方都不能被改变。
  - 默认是全局作用域，可以在整个运行的脚本的任何地方使用。
  - 常量名建议全部大写
- 格式：

```
define("常量名"，"常量值")
	例如：define("EN_NAME", "laoxie");     就相当于：// const MY_NAME = "lemon";

```

#### 6.运算符及语句（等同于js）

​	算术运算符、赋值运算符、递增/递减运算符、比较运算符(等于大于...)、逻辑运算符(与或非)、三元运算符
	条件语句、循环语句

#### 7.数据类型

$$
String（字符串）
Integer（整型）
Float（浮点型）
Boolean（布尔型）
Array（数组）
Object（对象）
NULL（空值）
$$

##### 7.1 String

```
strlen() 	获取字符串长度，得到的是字符串的字节数
mb_strlen() 获取字符串的长度
strpos()	查找某个字符在字符串中的索引，如果未找到，则返回false

```

例如：

```
?php
    $str = "哈嘿嘻";
    $length = mb_strlen($str);
    $idx = strpos($str,"呵"); 
    var_dump($idx);//测试
?>

================================================
	strpos("Hello world!","world");//=>6

```

##### 7.2 Array

> 数组是一个能在单个变量中存储多个值的特殊变量。

###### （1）创建数组：array()

```
//1.数值数组，等同于js的数组
$cars=array("Volvo","BMW","Toyota");
//2.关联数组，等同于js的对象
$age=array("Peter"=>"35","Ben"=>"37","Joe"=>"43");
//3.多维数组，包含一个或多个数组的数组

```

###### （2）数组常用方法

- count() 获取数组长度
- in_array() 判断某个值是否存在数组中
- array_slice() 从数组中取出一段
- array_rand() 随机获取索引值

###### 练习案例：在php文件里生成动态商品页面

###### （3）遍历数组

- for	一般用于遍历数值数组

- foreach() 一般用于遍历关联数组,或者对象

  ```
  <?php
      //遍历数值数组：for循环
      $cars=array("Volvo","BMW","Toyota");
      $arrlength=count($cars);
      for($x=0;$x<$arrlength;$x++){
          echo $cars[$x] . "<br>";
      }
      //关联数组：
      $age=array("Peter"=>"35","Ben"=>"37","Joe"=>"43");
      //获取单个值
      echo $age['peter'];
      //遍历关联数组：foreach..as
      foreach($age as $x=>$x_value){
          echo $x .":". $x_value;
          echo "<br>";
      }
      //多维数组：
      foreach($age as $item){
          //item代表数组里面的关联数组
      }
  ?>
  
  ```

###### 数组排序

- sort() 对数组进行升序排列
- rsort() 对数组进行降序排列
- asort() 根据关联数组的值，对数组进行升序排列
- ksort() 根据关联数组的键，对数组进行升序排列
- arsort() 根据关联数组的值，对数组进行降序排列
- krsort() 根据关联数组的键，对数组进行降序排列





# 第二天 9.11

# Ajax

## 了解AJAX

- AJAX: Asynchronous Javascript And Xml，Ajax 技术的核心是XMLHttpRequest对象（简称XHR），这是由微软首先引入的一个特性，其他浏览器提供商后来都提供了相同的实现

*Ajax起源：
最早出现在2005年的google搜索建议

- ajax优点
  - 增加速度：减轻服务器的负担,按需加载数据,最大程度的减少冗余请求
  - 改善的用户体验：局部刷新页面,减少用户等待时间,带来更好的用户体验
  - 页面和数据分离：前后端分离，操作更灵活，后期维护更方便
- 后端语言和服务器配置
  - php + Apache + mySQL
  - NodeJS + MongoDB
  - Java + tomcat + Oracle
  - .NET + IIS + SQL Server

## 一、json

#### 1. json数据（json字符串）

```
{"id" : 21465461461461, "name": "张三"},[{"id" : 21465461461461, "name": "张三"}]

```

#### 2. json字符串与对象的转换

```
//（一）json字符串转成对象的转换
//1. eval("("+json字符串+")"); 
它的作用是，将一个普通的json格式的字符串，转换成Json格式的对象
//var list = eval("("+request.responseText+")");
//2. JSON.parse(); //把JSON字符串转成JSON对象(js对象/数组)【es5】

//（二）把JSON对象转成JSON字符串
JSON.stringify(); 

```

#### 3. 了解json文件存在的意义

```
//模拟数据(与后端先商量)
[
	{
		"id":"G001",
		"name":"Thermos 膳魔师 Funtainer系列水杯 12盎司（340g） 粉红色",
		"imgurl":"images/g1.jpg",
		"price":899,
	}
]	

```

## 二、Ajax请求步骤

#### 1. 创建请求对象，返回一个异步请求对象

`var xhr = new XMLHttpRequest();`

#### 2.处理服务器返回数据

```
xhr.onreadystatechange = function(){
    if(xhr.readyState == 4) {
        //responseText：保存服务器返回的数据（从服务器返回的数据是“字符串”）。
        alert(xhr.responseText);
    }
}

```

#### 3.设置请求参数，建立与服务器连接

```
xhr.open("get", "http://localhost/api/ajaxtest", true);

```

#### 向服务器发送请求

`xhr.send(null);`

###### 案例：演示向goodslist.json请求数据

## 三、XMLHttpRequest对象属性方法

#### 1. open(type,url（同源策略）,async（同步、异步）)

```
1.open(type,url,async): 建立与服务器的连接
    type：请求的类型，get、post
    	* 区别? 
    		get请求数据接在url后面，post请求数据通过send方法传递
    		get传递的数据会比较少
    		get传递的数据会暴露出来
    url：数据请求的地址（API地址），一般由后端开发人员提供
        * 当前页面访问地址，API地址两者一定要同域
        * 同域（同源策略）：协议，域名，端口三者一致
        * 报错： No 'Access-Control-Allow-Origin' header is present on the requested resource. Origin 'null' is therefore not allowed access.
	async：是否异步发送请求（true,false），默认为true
        * 同步：按步骤顺序执行，前面的代码执行完后，后面的代码才会执行
        	做完前一件事情, 才能下一件事情（排队）
        * 异步：与其他操作同时执行，也叫并发（图片加载，ajax请求，定时器）

```

#### 2. send(data)

```
2.send(data): 向服务器发送请求
	data：可选参数，post请求时才生效，表示发请求时传送的数据字符串。
    	 xhr.send('size=20&type=music');
		在某些浏览器中，如果不需要通过post请求主体发送数据，则必须传入null
//备注：get请求的数据写在url地址后
	request.open("get", "http://localhost/api/getdata.php?type=get&qty=10", true);
	setRequestHeader(key,val)：设置请求头
//备注：利用请求头设置POST提交数据格式：
	xhr.setRequestHeader(‘content-type’,”application/x-www-form-urlencoded”)；//open方法后设置

```

> **在请求收到服务器的响应后，响应的数据会自动填充xhr 对象的属性，相关的属性简介如下：

#### 3. readyState

```
0 － （未初始化）尚未调用open()方法。
1 － （启动）已经调用open()方法，但尚未调用send()方法。
2 － （发送）send()方法执行完成，但尚未接收到响应。
3 － （接收）已经接收到部分响应数据。
4 － （完成）响应内容解析完成，可以在客户端调用了
只要readyState 属性的值由一个值变成另一个值，都会触发一次readystatechange 事件。必须在调用open()之前指定onreadystatechange事件处理程序才能确保跨浏览器兼容性。

```

#### 4. responseText

​	保存服务器返回的数据（从服务器返回的数据是“字符串”）。

#### 5. status

```
* 响应的HTTP 状态。
200（OK）：服务器成功返回了页面
304（Not Modified）：数据与服务器相同，不需要重服务器请求（直接使用缓存的数据）
400（Bad Request）：语法错误导致服务器不识别
401（Unauthorized）：请求需要用户认证
404（Not found）：请求地址不存在
500（Internal Server Error）：服务器出错或无响应
503（ServiceUnavailable）：由于服务器过载或维护导致无法完

```

## 四、php本地数据操作

#### 1. 获取前端数据

```
$_GET 获取前端用get方式传递过来的数据（url地址后面数据也能被获取）
$_POST	获取前端用get方式传递过来的数据
isset() 判断某个值是否被设置，若不存在返回boolean

```

#### 2. 文件的读取与写入

##### fopen(path,mode)：打开文件

> 使用fopen函数打开文件时，你首先需要明确打开文件的模式：
> 1.将数据写入文件，亦或者读写文件
> 2.考虑如果文件中已经存在相关数据，你是覆盖原有文件中的数据呢，还是仅仅将新数据添加至文件末尾

> 文件模式:
>
> - r 以只读方式打开文件，从文件头开始读
> - r+ 以读写方式打开文件，写入时以追加的方式写入文件
> - w 以写入方式打开文件，从文件头开始写。文件不存在则尝试创建，若存在，则先删除文件中的内容
> - w+ 以读写方式打开文件，从文件头开始读写。文件不存在则尝试创建，若存在，则先删除文件中的内容
> - a 以写入方式打开，从文件末尾开始追加写。如果文件不存在则尝试创建
> - a+ 以读写方式打开，从文件末尾开始追加写入或者读。如果文件不存在则尝试创建。

##### fread(file,length)：读取内容

##### fwrite(file,json字符串)：写入内容

##### fclose(file)：关闭文件,避免资源占用

##### filesize(path)：读取文件字符长度

```
//1.以读取模式打开文件
$path = './data/weibo.json'
$myfile = fopen($path, 'r');

//2.读取文件内容
$content = fread($myfile, filesize($path));

//3.关闭文件，减少资源占用
fclose($myfile);

```

```
echo返回数据
json_encode(); 把数组转成字符串
	php5.4+ 使用JSON_UNESCAPED_UNICODE防止中文转义
json_decode(json,assoc); 把字符串转成数组/对象
	json：待解码的 json string 格式的字符串
	assoc：默认false,返回嵌套对象的多维数组，通过arr->key获取对象键对应的值。当该参数为 true 时，将返回嵌套关联数组的多维数组，通过arr[key]获取关联数组键对应的值。

```

###### 案例：微博点赞

```
//（html页面）1.发起ajax请求，将weibo.json的内容返回到页面
var xhr = new XMLHttpRequest();
xhr.onreadystatechange = function(){
    if(xhr.readyState === 4 && xhr.status === 200){
        var res = JSON.parse(xhr.responseText);
        ul.innerHTML = res.map(item=>{
            return `<li data-id="${item.id}">
            <h4>${item.username}</h4>
            <p>${item.content}</p>
            <span>${item.comtcnt}</span>
            <span class="like">${item.likecnt}</span>
            </li>`;
    	}).join('');
    	datalist.appendChild(ul);
    }
}
xhr.open('get','../data/weibo.json',true);
xhr.send();
//(html页面)2.点赞，获取到当前按钮对用的id，发送ajax请求，get方法通过url拼接参数传送id到后台。
//随后php页面对json数据进行修改，再将当前被改变的对象返回。xhr对象通过responseText进行接收为字符串，转成对象，获取到linkcnt键对应的值，给当前事件源修改innerHTML。
//考虑多次请求，可能存在缓存状态，所以补充若是status为304也为请求成功。
datalist.onclick = function(e){
    if(e.target.className === 'like'){
        // e.target.innerText = e.target.innerText*1+1;
        // 获取当前微博id
        let currentLi = e.target.parentNode;
        let id = currentLi.dataset.id;
        let xhr = new XMLHttpRequest();
        let status = [200,304];
        xhr.onreadystatechange = function(){
            if(xhr.readyState === 4 && status.indexOf(xhr.status)>=0){
                let res = JSON.parse(xhr.responseText);
                e.target.innerHTML = res.likecnt;
            }
        }
        xhr.open('get','../api/weibo.php?id='+id,true);
        xhr.send();
    }
}
//（php）
//1.接收前端传过来的id，返回值为字符串
$id = isset($_GET['id']) ? $_GET['id'] : Null;
//2.打开json文件fopen()，读取json文件数据fread()。
$path = '';//相对路径
$file = fopen($path,"r");
$content = fread($file,filesize($path));
fclose($file);
//2.对得到的content内容转成json数组后，遍历里面每个item对象，若id键对应的值等于传入的$id,将该对象的linkcnt++。
$contentArr = json.decode($content);//此处contentArr为对象数组
$res;
foreach($contentArr as $item){
    //此处item为一个对象
    if($item->id == $id){
        $item->linkcnt++;
        $res = $item;
    } 
}
//4.将contentArr转成字符串，重新写入json文件
$file = fopen($path, 'w');
fwrite($file, json_encode($arr,JSON_UNESCAPED_UNICODE));
fclose($file);
//5.将步骤2声明变量res，将改变的item对象用res接收，转成字符串，echo给前端
echo json_encode($res,JSON_UNESCAPED_UNICODE);

```

###### 补充：eval的使用

```
var json = '{"name":"lemon","age":18}'; //标准json字符串
var json = '{"name":"lemon",\'age\':18}';//不标准
eval('()'+json+')');//也可以转成对象
eval('1+2');//3
eval('定义函数；执行函数') //函数可以在字符串中执行

```

###### 讲解：ajax的来历及同源策略、同步异步

###### 案例：用户名验证

```
username.onblur = function(){
    let _username = username.value;
    let status = [200,304];
    let xhr = new XMLHttpRequest();
    //xhr.onload意思为数据请求完成后，等同于xhr.readystate==4的状态
    xhr.onload = function(){
        if(status.includes(xhr.status)){
            let res = xhr.responseText;//fail,success
            if(res === 'fail'){
                username.nextElementSibling.innerHTML = `${_username}太受欢迎，你走吧`；
            }else{
                username.nextElementSibling.innerHTML = `恭喜你绿了`；
            }
        }
    }
    xhr.open('get','../api/checkname.php?username='+_username,true);
    xhr.send();
}
//php
//1.数组存放已经存在的用户名
$userlist = array('张三','李四','王尼玛','奥巴马','laoxie','lemon');
//2. 获取前端传来的用户名
$username = isset($_GET['username']) ? $_GET['username'] : null;
//3. 判断前端传来的用户名是否已存在数组内
$res = in_array($username, $userlist);
if($res){
    // 用户名已存在，注册失败
    echo "fail";
}else{
    echo "success";
}

```

###### 案例：分页数据加载

```
//html页面：
var qty = 5;
// 1.发起ajax请求数据，拿到返回的数据，转成对象。
let status = [200,304]
let xhr = new XMLHttpRequest();
xhr.onload = function(){
    if(status.includes(xhr.status)){
        let res = JSON.parse(xhr.responseText);
        // 2.拿到对象的data键对应的值(为json字符串)，渲染页面
        datalist.innerHTML= res.data.map(function(item){
            return `<li>
            <h4>${item.name}</h4>
            <div>${item.content}</div>
            </li>`;
        }).join("");
        //3.得到总页码数pageNum，parseInt(数据总数res.total/每页数据qty).遍历生成页码
        var pageNum = parseInt(res.total/res.qty);
        page.innerHTML = "";
        for(var i=0;i<pageNum;i++){
            var span = document.createElement("span");
            span.innerHTML = i+1;
            //5.拿到返回的当前页码-1，把当前索引设置高亮
            var curidx = res.curpage -1;
            if(i == curidx){span.className = "active";}
            page.appendChild(span);
        }

    }
}
xhr.open('get','../api/lemon.php?qty='+qty+'&curpage=1',true);
xhr.send();
// 4.点击分页切换
page.onclick = function(e){
    if(e.target.tagName.toLowerCase() === 'span'){
        let curpage = e.target.innerText;
        xhr.open('get','../api/lemon.php?qty='+qty+'&curpage='+curpage,true);
        xhr.send();
    }
}
//php：
<?php
    $qty = isset($_GET["qty"])? $_GET["qty"] : 5;
    $curpage = isset($_GET["curpage"])? $_GET["curpage"] : 1;
    //1.拿到json数据,根据每页数量与当前页，裁切对应的数据
    $path = '../data/football.json';
    $file = fopen($path,'r');
    $content = fread($file,filesize($path));
    $data = json_decode($content);
    $curdate = array_slice($data,$qty*($curpage-1),$qty);
    //2.格式化数据，再返回给前端
    $res = array(
        "total" => count($data),
        "data" => $curdate,
        "qty" => $qty*1,
        "curpage" => $curpage*1,
    );
    echo json_encode($res,JSON_UNESCAPED_UNICODE);
?>

```



## 五、ajax跨域解决方案

#### 1.JSONP

- JSONP 是JSON with padding（填充式JSON 或参数式JSON）的简写。

- JSONP是一种可以绕过浏览器的安全限制，从不同的域请求数据的方法。

- JSONP请求不是ajax请求，是利用script标签能加载其他域名的js文件的原理，来实现跨域数据的请求 

- 局限性：

  - 只能为get请求
  - 接口必须有回调函数的执行

- JSONP是一种可以绕过浏览器的安全限制，从不同的域请求数据的方法。使用JSONP需要服务器端提供必要的支持。

- JSONP 由两部分组成：回调函数和数据。回调函数是当响应到来时应该在页面中调用的函数 

- #### jsonp请求原理

  - JSONP的原理是通过script标签发起一个GET请求来取代XHR请求。
    - JSONP生成一个script标签并插到DOM中，
    - 然后浏览器会接管并向src属性所指向的地址发送请求。
    - 从服务器端返回一段js代码，这段代码就是一个函数的执行（执行时把数据作为参数传入，函数为本地预定义的函数）,这个我们就间接地得到了服务器传出的数据。

步骤如下：

1. 预定义全局函数getData

   ```
   function getData(data){
       console.log(data);
   }
   
   ```

   PS:预定义函数必须为全局函数

   2.生成script标签，请求服务器地址,并附带函数名 

   ```
   <script src="http://localhost:3000/getJSONP?callback=getData">< /script>
   
   ```

   3.服务器返回js文件（js文件里面包含我们预先定义的函数执行） 请求成功后，得到的js代码为 

   ```
   getData({name: '王大锤',age: 30,sex: '男',married:false})
   
   ```

   - 当这个函数成功调用时，就可以执行预定义函数里的代码（处理返回的数据）

   > jsonp请求不是ajax请求，是利用script标签能加载其他域名的js文件的原理，来实现跨域数据的请求

   - 缺点
     这种方法只支持GET方式，不如POST方式安全

###### 演示：使用script标签其他js文件调用本地js的某个函数

```
//html页面：
<script type="text/javascript">
    function sum(n){
        console.log(n);
    }
</script>
<script type="text/javascript" src="../js/common.js"></script>

//common.js代码
sum(6666);

//此时html页面的控制台打印 6666。

```

###### 演示：使用script标签其他php文件调用本地js的未知名方法，返回数据

```
//html页面：
<script type="text/javascript">
    function sum(data){
        console.log(data);
    }
    function sum2(data){
        alert(data);
    }
</script>
<script src="../api/lemon.php?callback=函数名"></script>

//php文件：
<?php
    $fn = $_GET["callback"];
    echo "$fn(数据)";
?>

```

###### 案例：利用JSONP原理调用百度建议

```
msg.oninput = function(){
    let _msg = msg.value;
    clearTimeout(timer);
    timer = setTimeout(()=>{
    let script = document.createElement('script');
    script.src='https://sp0.baidu.com/5a1Fazu8AA54nxGko9WTAnF6hhy/sujson=1&cb=getData&wd='+_msg;
    document.body.appendChild(script);
    },500);
}
window.getData = function(data){
    suggest.innerHTML = data.s.map(item=>{
        return `<li>${item}</li>`
        }).join("");
    }
})
//原理性代码：
//1.script的src中回调函数的传递
script.src='https://sp0.baidu.com/5a1Fazu8AA54nxGko9WTAnF6hhy/sujson=1&cb=getData&wd='+_msg;
//2.声明全局函数
window.getData = function(data){处理数据}

```

### 六、CORS

CORS是一个W3C标准，全称是”跨域资源共享”（Cross-origin resource sharing），它允许浏览器向跨源服务器发出XMLHttpRequest请求，从而克服了AJAX只能同源使用的限制。

CORS需要浏览器和服务器同时支持。目前，所有浏览器都支持该功能，IE浏览器不能低于IE10。

```
1.Access-Control-Allow-Origin
	header('Access-Control-Allow-Origin: * ');  
该字段是必须的。需要在后端响应头添加词字段，值要么是一个*，表示接受任意域名的请求，要么指定一个域名http://localhost。
2.Access-Control-Allow-Methods
3.Access-Control-Allow-Headers
    header('Access-Control-Allow-Methods:POST');  
    header('Access-Control-Allow-Headers:x-requested-with,content-type'); 

```

###### 案例：天气预报

```
//1.直接利用ajax请求得到数据
let xhr = new XMLHttpRequest();
let status = [200,304]
xhr.onload = function(){
    if(status.includes(xhr.status)){
        let res = JSON.parse(xhr.responseText)
        console.log(res.data);
        //拿到数据，可以渲染部分到页面上
        let title = document.createElement('h2');
        title.innerHTML = res.data.city + '天气预报';
        let tips = document.createElement('p');
        tips.innerHTML = res.data.ganmao;
        let ul = document.createElement('ul');
        ul.innerHTML = res.data.forecast.map(item=>{
            return `<li>
                <h4>${item.date}</h4>
                <p>${item.low} / ${item.high}</p>
                <p class="type">${item.type}</p>
            </li>`
        }).join('\n');
        // 清空内容
        weather.innerHTML = '';
        weather.appendChild(title);
        weather.appendChild(tips);
        weather.appendChild(ul);
    }
}
xhr.open('get','http://wthrcdn.etouch.cn/weather_mini?city=广州',true);
xhr.send();
//2.配合文本框实现，得到不同城市的天气预报
city.onblur = function(){
    let _city = city.value.trim();
    if(_city.length === 0){
        return;
    }
    xhr.open('get','http://wthrcdn.etouch.cn/weather_mini?city='+_city,true);
    xhr.send();
}

```

###### 演示：百度地图

### 七、服务器代理

后端不存在跨域问题，所以可以利用后端间接获取其他网站的数据

```
ajax跨域请求之服务端代理（爬虫）
原理：获取页面所有内容，并利用正则匹配所需内容
file_get_contents($url) //获取网站内容
preg_match_all($reg,$str,$res) 
preg_match($reg,$str,$res)   //$str代表被匹配的内容，$res为结果
$content = iconv(原字符编码,新字符编码,$content);//修改$content字符编码

```

###### 案例：利用服务器代理获取外网IP

```
api地址：http://2018.ip138.com/ic.asp
//本地api代理
<?php
    $content = file_get_contents("http://2018.ip138.com/ic.asp");//拿到远程网站内容
    $content = iconv('gb2312','utf-8',$content);//修改网站内容字符编码与相应头一致
    preg_match_all('/\[([\d\.]+)\]/',$content,$res);//正则匹配
    echo $res[1][0];
?>
//前端访问本地api

```

###### 案例：根据IP获取所在城市（ajax嵌套）

```
api地址：http://ip.taobao.com/service/getIpInfo.php?ip=$ip
//利用上一个案例请求拿到的ip，传入本地api。
let xhr_city = new XMLHttpRequest();
xhr_city.onload = function(){
    if(status.includes(xhr_city.status)){
        let city = xhr_city.responseText;
        //返回的是一串html结构加城市名，通过正则拿到城市名
        city = city.match(/[\u2E80-\u9FFF]+/)[0];
        console.log(city);
    }
}
xhr_city.open('get','../api/lemon.php?ip='+ip,true);
xhr_city.send(null);
//本地api
$ip = isset($_get['ip']) ? $_get['ip'] : "27.46.236.176";
$content = file_get_contents("http://ip.taobao.com/service/getIpInfo.php?ip=$ip");
$res = json_decode($content);
$data = $res->data;
$city = $data->city;
echo $city;

```

###### 案例：根据城市获取天气预报（ajax嵌套）

- 所有的代码都写在一个function里面，数据混乱，容易出错。
- 维护困难

###### 演示：post请求数据

## 八、Promise

Promise是一个构造函数，所谓的Promise对象，就是通过new Promise()实例化得到的对象，用来传递异步操作的消息。它代表了某个未来才会知道结果的事件（通常是一个异步操作），并且这个事件提供统一的 API，可供进一步处理。

##### Promise 的三种状态

> Pending（未完成）可以理解为Promise对象实例new创建时候的初始状态
> Resolved（成功） 可以理解为成功的状态
> Rejected（失败） 可以理解为失败的状态

#### （一）静态方法

##### Promise.all([p1,p2,p3...])

- 将多个Promise实例，包装成一个新的Promise实例

- 所有参数中的promise状态都为resolved时，新的promise状态才为resolved

- 只要p1、p2、p3..之中有一个被rejected，新的promise的状态就变成rejected 

  ```
  Promise.all([p1,p2,p3]).then(function(res){
  	console.log(res);
  })
  
  ```

##### Promise.race([p1,p2,p3...]) // 竞速，完成一个即可

#### （二）原型方法

##### Promise.prototype.then(successFn[,failFn])

> Promise实例生成以后，可以用then方法分别指定Resolved状态和Rejected状态的回调函数。并根据Promise对象的状态来确定执行的操作:
> resolved时执行第一个函数successFn
> rejected时执行第二个函数failFn。

##### Promise.prototype.catch(failFn)

###### 演示：定时器结束后再执行某些操作

```
var p = new Promise(function(resolve, reject){ 
	//做一些异步操作 
	setTimeout(function(){ 
		console.log('执行完成'); 
		resolve('随便什么数据'); 
	}, 2000); }
); 
p.then(function(data){
    //data为随便什么数据
}) 

```

###### 演示：生成一个0-2之间的随机数，如果小于1，则等待一段时间后返回成功，否则返回失败：

```
function test(resolve, reject) {
    var timeOut = Math.random() * 2;
    console.log(timeOut);
    setTimeout(function () {
        if (timeOut < 1) {
            resolve('200 OK');
        }
        else {
            reject('timeout in ' + timeOut + ' seconds.');
        }
    }, 1000);
}
var p1 = new Promise(test);
var p2 = p1.then(function (result) {
    console.log('成功：' + result);
});
var p3 = p2.catch(function (reason) {
    console.log('失败：' + reason);
});

```

###### 演示：利用promise完善ajax嵌套

> 有了Promise对象，就可以将异步操作以同步操作的流程表达出来，避免了层层嵌套的回调函数 

###### 加载图片，获取图片信息（宽高）

```
var p = new Promise(function (resolve, reject) {
    var image = new Image();//生成img标签
    image.src = 'http://image.baidu.com/xxx.jpg;
    image.onload  = ()=>{
        resolve(image);
    }
    image.onerror = reject;
  });
//使用
p1.then((img)=>{
    document.body.appendChild(img);
    console.log(img.offsetWidth,img.offsetHeight);
}) 

```

## 九、try...catch

尝试执行代码，如果有错误则执行catch捕获错误(不报错)

```
try{
	console.log(666)
	//先尝试执行这里的代码
	show();
	//无报错，则忽略catch
	//如果报错，则执行catch，并传递错误信息
}catch(error){
	console.log(error)
}
console.log('end');

```

###### 演示：xhr的兼容写法

```
var req = null;
try{
    req = new XMLHttpRequest();
}catch(err){
    // ie低版本浏览有多种异步请求的实现
    try{
        req = new ActiveXObject("Msxml2.XMLHTTP");
    }catch(err){
        try{
            req = new ActiveXObject("Microsoft.XMLHTTP");
        }catch(err){
            alert('你的浏览器太low了，这个世界不适合你');
        }
    }
}

```

## 十、API

- 服务器API

  - 向服务器请求数据：
    接口地址：api/ajaxtest.php
    接口描述：返回一段字符串，无特殊功能

  - 判断用户名是否已被注册
    接口地址：api/checkname?regname=xiejinrong
    接口描述：该地址验证所提交的用户名是否存在，如果已存在，返回字符串no，不存在返回yes
    参数说明：regname:注册用户名，必填

    > 已经存在的名字：’张三’,’李四’,’王尼玛’,’奥巴马’

  - 微博消息获取：
    接口地址：api/weibo.php
    接口描述：返回包含多条微博记录的json数据

  - 分页获取数据：
    接口地址：api/football.php 
    接口描述：该地址请求多条微博信息，分页获取，pageNo指定获取第几页的数据
    参数说明：

    - pageNo:当前分页，默认1
    - qty:每页显示数量，默认10

  - 聊天室：
    获取本机ip地址：api/getip.php
    获取信息：api/chat.php?type=query
    发送信息：api/chat.php?type=send&sender=xiejinrong&msg=hello

  - 利用jsonp获取远程数据
    接口地址：api/jsonp.php
    接口描述：jsonp跨域解决方案

  - 获取CORS获取远程数据
    接口地址：api/cors.php
    接口描述：CORS跨域解决方案

- 利用jsonp实现百度搜索关键字建议
  `https://sp0.baidu.com/5a1Fazu8AA54nxGko9WTAnF6hhy/su?json=1&cb=getData&wd=html5`

- 利用CORS加载天气
  接口地址：`http://wthrcdn.etouch.cn/weather_mini?city=北京`
  接口描述：通过城市名字获得天气数据，json数据

- 利用服务器代理获取外网IP

  - api地址：api/ip.php

- 根据IP获取所在城市
  `http://int.dpool.sina.com.cn/iplookup/iplookup.php?format=json&ip=27.46.236.176`

 

# 9.17	Mysql

## 一、什么是数据库

数据库（Database）是按照数据结构来组织、存储和管理数据的仓库

**热门数据库**

- Oracle
- SQLServer
- MySQL
- MongoDB
- SQLite
- access
- DB2

## 二、结构化的数据

**仔细阅读上面这段话，如果让你提取这段文字的中心意思，你能做到吗？**

我相信对一个正常人来说都不是难事。可是，这段话如果交给计算机去处理呢？ 计算机没有人类的思维，这件事对它来讲恐怕就太难了，因此，有时候我们才需要将数据结构化。

结构化的数据是什么样子呢？以上面那段话为例，我们将它的信息提取出来，以表格的形式展现：

| 姓名   | 年龄 | 性别 | 性格     | 所在地 | 毕业院校 | 专业     |
| ------ | ---- | ---- | -------- | ------ | -------- | -------- |
| lemon  | 17   | 女   | 乐观     | 广州   | 清华     | 前端开发 |
| laoxie | 48   | 男   | 积极向上 | 广州   | 蓝翔     | 挖掘机   |

> 这样一来，我们把一段复杂的信息，进行了结构化处理，瞬间显得清爽多了。计算机处理起来也相当方便。 因此，这样的数据，我们就称之为结构化数据，而上面的表格称之为表。

## 三、关系型数据库

是建立在关系模型基础上的数据库，复杂的数据库表与表之间必定存在某种联系

| 姓名 | 身份证             | 银行卡号       | 余额      | 消费记录                                                     |
| ---- | ------------------ | -------------- | --------- | ------------------------------------------------------------ |
| 老谢 | 450721199805012611 | 8888 6968 9898 | 865424.00 | 2016.11.1 6000买iphone7, 2016.12.20 5800买note7, 2017.1.1 1665800买飞机 |

所有的购买记录这样的数据看起来是不是很别扭呢？ 因为它查询起来极不方便。

因此我们把它改造一下（把用户和消费记录分开）：

| 编号 | 姓名 | 身份证             | 银行卡号       | 余额      |
| ---- | ---- | ------------------ | -------------- | --------- |
| 1    | 老谢 | 450721199805012611 | 8888 6968 9898 | 865424.00 |
| 2    | 蓝梦 | 460751198007125628 | 8888 6968 9898 | 26424.00  |

| 编号 | 时间       | 消费金额 | 备注      | 用户编号 |
| ---- | ---------- | -------- | --------- | -------- |
| 1    | 2016.11.1  | 6000     | 买iphone7 | 1        |
| 2    | 2016.12.20 | 5800     | 买note7   | 1        |
| 3    | 2017.1.1   | 1665800  | 买飞机    | 2        |

我们把用户账号的信息，和消费记录信息分离开来，通过用户编号进行了关联 既把不同的数据进行了分离，使得查询数据更加方便。同时又保证了它们关系的正确性。

**这就是传统的关系型数据库。** 其中 <用户编号> 我们称之为**外键**

### 四、表（table）:

一个数据库通常包含一个或多个表，一个数据表有一个唯一名称，并有行和列组成。
表(table) 是数据库中一个重要的组成部分, 数据库只是一个框架，数据表才是其实质内容。
![数据库与表](//F:/mydoc/kphone/Outline3/Section2/7.0/22mysql/doc/img/img1.png)

- 表结构

| 身份ID | 姓名 | 性别 | 年龄 |
| ------ | ---- | ---- | ---- |
| 1      | 刘备 | 男   | 40   |
| 2      | 关羽 | 男   | 36   |
| 3      | 貂蝉 | 女   | 18   |
| 4      | 张飞 | 男   | 30   |

## 五、MySql的特点:

> MySql是目前最流行的关系型数据库管理系统，由瑞典MySQL AB公司开发，目前属于Oracle公司

- MySQL是开源的，免费。
- MySQL支持标准的SQL数据语句
- MySQL可以允许于多个系统上，并且支持多种语言。这些编程语言包括C、C++、Python、Java、Perl、PHP、Eiffel、NodeJS、Ruby和Tcl等。
- MySQL对PHP有很好的支持，PHP是目前最流行的Web开发语言。
- MySQL支持大型数据库，支持5000万条记录的数据仓库，32位系统表文件最大可支持4GB，64位系统支持最大的表文件为8TB。

## 六、数据库操作

### 表操作(了解)

- 连接数据库
  格式：`mysql -h主机地址 -u用户名 -p用户密码`

- 显示所有数据库
  格式：`show databases;`

- 创建数据库
  格式：`create database <数据库名>;`

- 使用数据库
  格式：`use <数据库名>;`

- 显示当前数据库所有表
  格式：`show tables;`

- 创建数据表
  格式：`create table <表名> (<字段名1> <类型1> [,..<字段名n> <类型n>]);`

  ```
      create table MyGuests (
      id int(6) unsigned auto_increment primary key, 
      firstname varchar(30) not null,
      lastname varchar(30) not null,
      email varchar(50),
      reg_date timestamp
      )
  
  ```

  以上创建一个名为 “MyGuests” 的表，包含5个列： “id”, “firstname”, “lastname”, “email” 和 “reg_date”，参数如下：

  - 数据类型:
    - INT(整型),
    - FLOAT(浮点),
    - CHAR(固定长度字符串),
    - VARCHAR(可变长度字符串),
    - BLOB(二进制),
    - TEXT(字符串)
    - TIMESTAMP(时间戳)
  - 列的其他属性
    - NOT NULL - 每一行都必须含有值（不能为空），null 值是不允许的。
    - DEFAULT value - 设置默认值
    - UNSIGNED - 使用无符号数值类型，0 及正数
    - AUTO_INCREMENT - 设置 MySQL 字段的值在新增记录时每次自动增长 1
    - PRIMARY KEY - 设置数据表中每条记录的唯一标识。 通常列的 PRIMARY KEY 设置为 ID 数值，与 AUTO_INCREMENT 一起使用。

- 删除表：
  格式：`drop table <表名>;`

  ```
  drop table MyGuests;
  drop table if exists MyGuests
  
  ```

  

- 查询表结构：
  `desc MyGuests`

- 修改表名。
  `rename table MyClass to YouClass;`

- 增加字段
  `alter table MyGuests add sku_id bigint(20) unsigned DEFAULT NULL COMMENT '商品销售码';`

- 复制表结构：
  `create table table1 like table;`

## 七、Navicat操作数据库

- 数据库创建
- 表创建
- 增删查改（CRUD）
- 数据导入
  - json
  - excel

## 八、数据操作（重点）

- 插入数据
  格式：`insert into <表名> [(<字段名1>[,..<字段名n > ])] values ( 值1 )[, (值n )];`

  ```
  //单条数据
  insert into MyGuests (firstname, lastname, email)
  values ('John', 'Doe', 'john@example.com')
  
  ```

  

- 删除表数据
  格式：delete from 表名 where 表达式

  ```
  //删除MyGuests表中id为1的数据
  DELETE FROM MyGuests where id=1;
  
  //删除所有数据
  DELETE FROM MyGuests
  
  ```

  

- 查询表中的数据
  格式： select <字段1, 字段2, …> from < 表名 > where < 表达式 >;

  ```
  //查看表 MyGuests 中所有数据
  select * from MyGuests;
  
  //查看表 MyGuests 中前10行数据：
  select * from MyGuests order by id limit 0,10;
  
  ```

  

  > select一般配合where使用，以查询更精确更复杂的数据。

- 修改表中的数据。
  格式：update 表名 set 字段=新值,… where 条件;

  ```
  update MyGuests set name='Mary' where id=1;
  
  ```

- 条件控制语句 

  - WHERE 语句：

    - > SELECT * FROM tb_name WHERE id=3;

- 相关条件控制符： 

  - =、>、<、<>、IN(1,2,3......)、BETWEEN a AND b
  - AND、OR、NOT
  - LIKE用法中 
  - % 匹配任意、
  - _ 匹配一个字符（可以是汉字）
  - LIMIT idx,qty：数量控制
    - SELECT * FROM goods LIMIT 2,5

  

- IS NULL 空值检测

- 排序ORDER BY

- asc 升序（默认）

- desc 降序

## 九、php操作数据库

### （一）连接 MySQL

PHP 5 及以上版本建议使用以下方式连接 MySQL :

- MySQLi extension (“i” 意为 improved)
  安装：Linux 和 Windows: 在 php5 mysql 包安装时 MySQLi 扩展多数情况下是自动安装

- ```
  <?php
          $servername = "localhost";
          $username = "username";
          $password = "password";
          $dbname = 'user';
  
          // 创建连接
          $conn = new mysqli($servername, $username, $password, $dbname);
  
          // 检测连接
          if ($conn->connect_error) {
              die("连接失败: " . $conn->connect_error);
          } 
  
          //查询前设置编码，防止输出乱码
          $conn->set_charset('utf8');
  
          echo "连接成功";
      ?>
  
  ```

  

- 执行sql语句查询结果集

  ```
      //编写sql语句
      $sql = 'select * from student';
  
      //获取查询结果集
      $result = $conn->query($sql);
  
      //使用查询结果集
      //得到数组
      $row = $result->fetch_all(MYSQLI_ASSOC);
  
      //释放查询结果集，避免资源浪费
      $result->close();
  
      //把结果输出到前台
      echo json_encode($row);
  
      // 关闭数据库，避免资源浪费
      $conn->close();
  
  ```

### （三）插入数据INSERT INTO

- 单条数据

  ```
  $sql = "INSERT INTO MyGuests (firstname, lastname, email)
  VALUES ('John', 'Doe', 'john@example.com')";
  
  if ($conn->query($sql)) {
      echo "新记录插入成功";
  } else {
      echo "Error: " . $sql . "<br>" . $conn->error;
  }
  
  ```

  

- 多条数据

  ```
      $sql = "INSERT INTO `projects` (`name`, `url`, `description`) VALUES ";
      foreach ($projects as $item) {
          $sql .= "('$item',NULL, NULL),";
      }
      $sql = substr($sql,0,-1);
  
      if ($conn->query($sql)) {
          echo "新记录插入成功";
      } else {
          echo "Error: " . $sql . "<br>" . $conn->error;
      }
  
  ```

### （四）读取数据

SELECT…FROM，得到查询结果集

- num_rows ：结果集中的数量，用于判断是否查询到结果
- fetch_all(MYSQLI_ASSOC) 得到所有结果
- fetch_assoc() 得到第一个结果
- fetch_row()

```
    $sql = "SELECT id, firstname, lastname FROM MyGuests";
    $result = $conn->query($sql);

    if ($result->num_rows > 0) {
        // 输出每行数据
        while($row = $result->fetch_assoc()) {
            echo "<br> id: ". $row["id"]. " - Name: ". $row["firstname"]. " " . $row["lastname"];
        }
    } else {
        echo "0 个结果";
    }

```

### （五）mySQL语句返回值

- 返回布尔值
  - insert
  - update
  - delete
- 返回查询结果集
  - select语句

# 9.18 面向对象

定义：利用对象进行编程的一种思想。object-oriented programming，简称oop。

## 一、面向过程及与面向对象的区别

###### 举例:五子棋游戏

```
//面向过程：
1、开始游戏，
2、黑子先走，
3、绘制画面，
4、判断输赢，
5、轮到白子，
6、绘制画面，
7、判断输赢，
8、返回步骤2，
9、输出最后结果。
//面向对象
1、黑白双方，这两方的行为是一模一样的.  位置、种类{[][]}
2、棋盘系统，负责绘制画面。盘、黑白子、[创建span，添加不同类名，位置。]
3、规则系统，负责判定诸如犯规、输赢等。判断是不是在同一条线上
//总结:面向对象是按照功能划分问题，保证了可扩展性。例如添加悔棋功能，如果是面向过程，那么从输入到判断到显示这一连串的步骤都要改动，甚至步骤之间的循序都要进行大规模调整。而面向对象，只需要让棋盘系统回溯到上一步即可，无需纠结1、3功能。

```

###### 演示：创建并描述对象

- 描述一个人
- 描述购物车

###### 总结：

```
面相对象指的就是把以前那种从上而下的代码，改成了用对象的方式划分去写
	*每个对象都有自己的任务和功能

```

## 二、如何创建对象

#### 1. 字面量

```
var student = {id:10,name:"小明",age:18}
	*创建思路：
		（1）创建对象（有什么，能干什么）
		（2）指挥对象
			例如 var meinv = {
                // 有什么
                name : "laoxie",
                age : 17,
                gender : "woman",
                //做什么
                coding : function(){
                    console.log("我会敲代码");
                },
                mashaji : function(){
                    console.log("金牌按摩师");
                }
            }
            meinv.mashaji();  //指挥对象

```

#### 2. 内置object构造函数创建

例如：

```
		var car = {
            //有什么
            step : 1,
            ele : ".output",
            // pay : ".payBtn",
            //能做什么
            init : function(){
                //判断第几步骤，执行不同的step代码
            }
            step1 : function(){
                // 如果将数据渲染到页面上
                car.ele = document.querySelector(car.ele);
                car.pay = ele.querySelector(.payBtn);
            }
        }

        var carItem = {
            //商品
            goodsArr : [],
            //增加按钮:
            addBtn :,
            //删除当前商品的按钮
            //清空购物车的按钮
            //方法:
            //初始化购物车的item部分
            init : function(){},
            add:function(){},
            remove:function(){},
            clear:function(){}
        }

备注：字面量与内置object构造函数不适合用于创建多个同一类型的对象，会出现很多重复的代码。一般用于只会存在一个该对象的地方

```

#### 3. 通过new关键字实例化对象

```
var student = new object();
student.id = 10;
student.name = '王铁锤';
student.age = 18;

//缺点：使用同一个接口创建很多对象，会产生大量重复代码

```

#### 4.工厂模式

定义：在ECMAScript中是无法创建类的，开发人员就发明了一种函数，用函数来封装特定接口创建对象的细节。

```
function createPerson(name, age, job) {
    var o = new Object();
    o.name = name;
    o.age = age;
    o.job = job;
    sayName = function () {
        alert(this.name);
    };
    return o;
}
var person1 = createPerson('zxj', 23, "Software Engineer");
var person2 = createPerson('sdf', 25, "Software Engineer");

//不足：在示例中我们可以看到，工厂模式虽然解决了创建多个相似对象的问题，但没有解决对象识别的问题（在示例中，得到的都是o对象，对象的类型都是Object）。

```

#### 5. 自定义构造函数（类的概念）

定义：ECMAScript中的构造函数可以用来创建特定类型的对象。像Object和Array的原生的构造函数，在运行时会自动出现在执行环境中。此外，也可以创建自定义的构造函数，从而定义自定义对象类型的属性和方法。

###### 演示：自定义构造函数相对于工厂函数的好处

```
function Student(name, age){
    this.name = name;
    this.age = age;
    this.sayName = function(){alert(this.name);};
}
var s1 = new Student("王铁锤", 18);
//可以通过控制台查看一下person1与s1的区别，更好理解。

```

#### 6. 构造函数与普通函数的区别

唯一区别：调用方式不同

- 任何函数，只要通过new操作符来调用，它就可以作为构造函数

- 而任何构造函数，如果不通过new操作符来调用，那它就跟普通函数无区别

  约定：构造函数名首字母大写

###### 演示：构造函数与普通函数执行方式的区别

```
function Dog(){
	this.name = '哈巴';
	this.color = '白色';
	this.jiao = function(){
    	console.log("我的名字叫"+this.name);
    }
}
// 普通函数执行方式
// Dog(); => 没有值return出来，所以输出结果为undefined
// 构造函数的调用方式
// new Dog(); => 输出结果为对象

```

#### * 调用自定义构造函数实际上会经历以下4个步骤：

1. 创建一个新对象（在内部隐式调用了new Object()）;
2. 将构造函数的作用域赋给新对象（把this绑定到实例对象）；
3. 执行构造函数中的代码（为这个新对象添加属性）；
4. 返回新对象。

```
/ 通过new调用函数==>构造函数
// 1. var obj = {}
// 2. Dog.bind(obj)
// 3. 执行构造函数中的代码：this为obj
// 4. return obj;

```

## 三、this

定义：函数中的this作为js的关键字，有特殊的含义，代表了当前对象，而当前对象是谁，由函数执行时所处的环境来决定

<!--this好比一句话, 出自不同人之口, 代表的人就不一样-->
<!--如A和B吵架：-->
<!--A对B说: “老子要砍死你! ” , 这里的老子指A-->
<!--B对A说: “老子要弄死你! ”, 这里的老子指B-->

用new关键字执行：this指向生成的实例对象
普通函数执行：this指向调用函数的对象

## 四、对象的组成部分

#### 1. 构造函数

```
	*this指向实例对象

```

#### 2. 实例对象

（1）用new关键字生成的对象称为实例，实例会复制构造函数内所有的属性和方法。

（2）可以实例对象获取原型对象：

```
__proto__  //Frefox,Chrome等浏览器可以通过私有属性
Object.getPrototypeOf(实例)； //ES5方式去获取

```

#### 3. 原型对象

- 我们创建的每个函数都有一个prototype属性，指向原型对象。
- 原型对象默认包含一个constructor属性，指向构造函数。
- **任何写在原型对象中的属性和方法，都可以让所有实例对象共享。**![单个构造函数与原型对象、实例对象的关系图](E:\H5每天\二阶段18.8.13\25.9.18\25-26.OOP&Inherit\doc\单个构造函数与原型对象、实例对象的关系图.png)

#### 4. 三者的关系

1. 每个构造函数都有一个原型对象（prototype），
2. 原型对象都包含一个指向构造函数的指针（constructor），
3. 而所有实例都通过`__proto__`指向同一个原型对象。（包含一个指向原型对象的内部指针（[[prototype]]））

#### 5.判断原型和实例的关系（返回布尔值）

constructor: 得到构造函数的引用，一般用于判断该实例是否由某一构造函数生成

```
实例.constructor == Student //true

```

instanceof: 检测某个对象是不是某一构造函数的实例，适用于原型链中的所有实例

```
实例 instanceof Student //true
实例 instanceof Object //true

```

isPrototypeOf: 判断当前对象是否为实例的原型对象

```
原型对象.isPrototypeOf(实例) //true

```

#### 6.实际应用

构造函数方法很好用，但是单独使用存在一个浪费内存的问题（所有的实例会复制所有构造函数中的属性/方法）。这样既不环保，也缺乏效率。

#### **解决方案:构造函数+原型对象**

- 使用构造函数添加私有属性
- 使用原型对象添加共享方法

**优点：**

- 实例对象都有自己的独有属性
- 实例共享了原型中的方法，最大限度的节省了内存
- 支持向构造函数传递参数

###### 演示：使用原型对象添加共享方法

```
function Person(name,age,gender){
    // 属性
    this.name = name;
    this.age = age;
    this.gender = gender;
    // 方法
    // this.say = function(){console.log('say');}
    // this.singing = function(){console.log('singing');}
}
 // 把方法提取到原型对象
 Person.prototype.say = function(){
    console.log('say');
 }
 Person.prototype.singing = function(){
    console.log('singing');
 }
 var lx = new Person('laoxie',18,'male');//2M	
 var lm = new Person('lemon',31,'femal');//5M	

```

###### 案例：弹幕效果

```
//1.生成页面元素对象
//属性有：整个弹幕区域、消息框、按钮
//方法有：
//	-初始化：获取元素，点击按钮，执行发送方法
//	-发送方法，获取消息框内容。实例化弹幕对象
let page = {
    ele:'#barrage',
    msg:'#msg',
	button:'#msg+button',
    init(){
        this.ele = document.querySelector(this.ele);
        this.msg = document.querySelector(this.msg);
        this.btn = this.msg.nextElementSibling;
        this.btn.onclick = ()=>{
            this.send();
        }
    },
    send(){
        let msg = this.msg.value;
        new Barrage(msg);
    }
}
2.自定义弹幕对象的构造函数
(1) 属性：内容、颜色、速度、字体大小、位置
(2) 方法：
    - 初始化init()：创建弹幕对象this.ele，添加内容类名及样式，添加到元素内
    - 运动move()：从右往左
    - 移除remove():移除弹幕
function Barrage(msg){
    this.color = randomColor();
    this.speed = randomNumber(-20,-5);
    this.size = randomNumber(12,48);
    this.position = randomNumber(10,page.ele.clientHeight-this.size-10);
    this.init(msg);
}
Barrage.prototype.init = function(msg){
    // 创建弹幕元素
    this.ele = document.createElement('span');
    this.ele.innerText = msg;
    this.ele.className = 'bar-item';
    // 定义样式
    this.ele.style.color = this.color;
    this.ele.style.fontSize = this.size + 'px';
    this.ele.style.top = this.position + 'px';
    // 写入页面
    page.ele.appendChild(this.ele);
    // 移动
    this.move();
}
Barrage.prototype.move = function(){
    this.timer = setInterval(()=>{
        let left = this.ele.offsetLeft;
        left += this.speed;
        if(left <= -this.ele.offsetWidth){
            clearInterval(this.timer)
            this.remove();
        }
        this.ele.style.left = left + 'px';
    },30);
}
Barrage.prototype.remove = function(){
    this.ele.parentNode.removeChild(this.ele);
}
// 页面元素对象的init方法开始执行
page.init();

```

###### 案例：烟花效果

```
1.页面 page （字面量：一个）

- 属性： 按钮、显示区域
- 方法： 初始化（获取元素，给this.ele绑定点击事件,获取光标位置，实例化烟花对象）
  let page = {
  ele:'body',
  btn:'#auto',
  init(){
      this.ele = document.querySelector(this.ele);
      this.btn = document.querySelector(this.btn);
      document.onclick = function(e){console.log(666)
          new Firework(e.pageX,e.pageY);
      }
  }

2.烟花 firework

- 属性：位置、爆炸数量、爆炸半径

- 方法：
  （1）初始化：生成span，添加类名，及当前的水平坐标，添加到页面中。执行移动方法
  （2）移动： 利用动画移动到光标top位置，同时将自身高度变小。执行爆炸方法，同时移除自身。
  （3）爆炸：利用数量计算角度，将圆心位置，半径及角度都传给火花实例对象
  （4）移除
  function Firework(x,y){
  this.left = x;
  this.top = y;
  // 爆炸数量
  this.qty = randomNumber(12,36);
  // 爆炸半径
  this.r = randomNumber(50,200);
  this.init();
  }
  Firework.prototype.init = function(){
  this.ele = document.createElement('span');
  this.ele.className = 'fire';
  this.ele.style.left = this.left + 'px';
  page.ele.appendChild(this.ele);
  this.move();
  }
  Firework.prototype.move = function(){
  animate(this.ele,{top:this.top,height:this.ele.clientWidth},()=>{
      this.boom();
      this.remove();
  })
  }
  Firework.prototype.boom = function(){
  for(var i=0;i<this.qty;i++){
      // 计算角度
      let deg = 360/this.qty*i;
      new Spark(this.left,this.top,this.r,deg);

  }
  }
  Firework.prototype.remove = function(){
  this.ele.parentNode.removeChild(this.ele);
  }
  3.爆炸烟火 spark	

- 属性：随机色、半径、弧度、圆心位置

- 方法：
  初始化：创建this.ele火花span、添加类名，设置初始化位置，写入页面
  火花移动:设置最终位置，利用动画移动到指定left、top值，及改变透明度。动画完成后移除
  移除火花
  function Spark(x,y,r,deg){
  this.color = randomColor();
  this.r = r;
  this.rad = Math.PI*deg/180;
  this.init(x,y);
  }
  Spark.prototype.init = function(x,y){
  this.ele = document.createElement('span');
  this.ele.className = 'spark';
  // 设置颜色
  this.ele.style.backgroundColor = this.color;
  // 设置初始位置
  this.ele.style.left = x + 'px';
  this.ele.style.top = y + 'px';
  // 写入页面
  page.ele.appendChild(this.ele);
  this.move(x,y)
  }
  Spark.prototype.move = function(x,y){
  var a = this.r * Math.cos(this.rad);
  var b = this.r * Math.sin(this.rad);
  var left = parseInt(x + b);
  var top = parseInt(y - a);
  animate(this.ele,{left,top,opacity:0.3},()=>{
      this.remove();
  })
  }
  Spark.prototype.remove = function(){
  this.ele.parentNode.removeChild(this.ele);
  }
  // 操作对象
  page.init()；

```

# 9.20

## 一、属性特性:ES5对象扩展(了解)

### （一）值属性的属性特写

- configurable

  - 可配置性，控制着其描述的属性的修改，表示能否修改属性特性

    ```
    解释：就是能不能修改下面这些属性，如果为true方可修改，正常情况下都为true
    	*若是直接通过点或者[]添加对象属性，属性特性（除了value）默认都为true。若通过Object.defineProperty()方法添加对象属性，属性特性默认都为false。
    
    ```

    

- enumerable

  - 可枚举性，表示能否通过for-in遍历得到属性

- writable

  - 可写性，表示能否修改属性的值

- value

  - 数据属性，表示属性的值。默认为undefined

### （二）与属性相关的写法

#### 1.设置属性特性

```
设置属性特写：

object.defineProperty(obj,property,descriptor)
	*给对象的某个属性设置属性特性
	
Object.defineProperties(object, descriptors) 
	*给对象的所有属性设置属性特性

备注： obj :你要设置的那个对象
	  property: 要添加的属性 //用双引号
	  descriptors：上面的各种特性
	例如： Object.defineProperty(page,"friut",{value:"apple",enumerable:true,writable:true,configurable:true});

```

#### 2. 获取属性特性

```
object.getOwnPropertyDescriptor(object, propertyname)
	object ：你要获取的那个对象
	propertyname ： 对象里面的属性的名字
		*返回的是属性特性，也就是上面的那些东西

获取对象的所有属性特性：
Object.keys(object) 只获取到可枚举的属性
Object.getOwnPropertyNames(object) 获取所有属性的名称（包含不能枚举的属性）

```

###### 演示：添加属性的相关方法（同时设置属性特性）

```
var obj = {
    a:1,
    b:"lemon"
}
//1.给对象添加一个属性，同时设置属性特性。此时其他的属性特性不设置默认都为false。
//即configurable为false，不可以修改属性特性。
//即enumerable为false，不可以枚举
//即writable为false，不可写，不可以修改属性值
Object.defineProperty(obj,"c",{value:"laoxie"})； //以上属性特性均可改成true，实现相应的功能。

// 2.同时修改多个属性特性
Object.defineProperties(obj, {
    b:{value:'css4',enumerable:false},
    c:{writable:true}  //报错，因为上面定义该属性的configurable为false，意思是不可以修改属性特性
})

//建议：用传统方式添加属性，利用defineProperty修改属性特性（configurable为true的前提下）

```

### （三）对象属性的遍历与判断

#### 1. for...in

定义：遍历对象中的所有可枚举属性，无论该属性在于实例中还是原型中

#### 2. in

```
if(name in s1){
	//只要通过对象能够访问到属性就返回true, 无论该属性存在于实例中还是原型中
}

```

#### 3. 对象.hasOwnProperty(属性)

```
解释：检测一个属性是存在于对象的本身中
	*返回true，说明属性存在对象中
	*返回false，说明属性不存在或在原型中
	
	检测一个属性是否存在于原型中：!obj.hasOwnProperty(name) && (name in obj) 

```

## 二、重置原型对象

定义：重置原型对象，可以一次性给原型对象添加多个方法，但切断了与原来原型对象的联系

```
function Popover(){}
Popover.prototype = {
    show:function(){},
    hide:function(){}
}
//- 注意覆盖问题（系统的原型对象不建议重写）
//- 注意识别问题（不可枚举性）
Object.defineProperty(Popover.prototype,"constructor",{value:"Popover",configurable:true})；	//添加constructor属性

```

## 三、内置的原型对象

使用内置原型对象可以给已有的构造函数添加方法

- 数组/字符串/数字等方法调用原理
- 扩展内置方法

```
if(!Array.prototype.norepeat){
            Array.prototype.norepeat = function(){
                return Array.from(new Set(this));	//// this：指向实例arr
            }
        }
        var arr = new Array(1,2,3,3,1,4,5,6,2);
        var res = arr.norepeat();
        console.log(res);

```

## 四、原型链

定义：实例与object原型对象之间的链条称为原型链

### （一）原型模式的访问机制（原型搜索机制）

1. 读取实例对象的属性时，先从实例对象本身开始搜索。如果在实例中找到了这个属性，则返回该属性的值
2. 如果没有找到，则继续搜索实例对象的原型对象，如果再原型对象中找到了这个属性，则返回该属性的值
3. 如果还是没找到，则向原型对象的原型对象查找，以此类推，直到object的原型对象（最顶层对象）
4. 如果在object的原型对象中还搜索不到，则抛出错误![与Object.prototype的关系](E:\H5每天\二阶段18.8.13\25.9.18\25-27.OOP&Inherit、闭包\doc\神笔马良\与Object.prototype的关系.png)

## （二）继承

定义：继承是面向对象中一个非常重要的特性。指的是：子类继承父类的属性和方法

```
我们可以通过继承的方式，在父类的属性和方法基础上，让子类也拥有这些属性和方法，并可以扩展


继承的解释：就是把父代的实例对象赋值给子代的原型对象，然后子代的实例对象就可以随意调用父代原型对象中的方法了
	* Dog.prototype = new Animal();

```

#### 1.  继承的好处

（1）子类拥有父类所有的属性和方法（代码复用）

（2）子类可以扩展自己的属性和方法（更灵活）

（3）子类可以重写父类的方法

### （三） 继承的方式

#### 1. 原型链继承

- 核心：拿父类实例来充当子类原型对象
- 缺点：
  - 无法操作父类构造函数的属性，若不传值给父类，父类的属性为undefined。

```
  function Animal(jiaosheng,color){
            this.jiaosheng = jiaosheng,
            this.color = color
        }
        Animal.prototype = {
            constructor : Animal,
            fanzhi : function(){
                console.log("卵生");
            },
            eat : function(){
                console.log("吃好吃的");
            }
        }
        function Dog(color){
            this.name = "旺财",
            this.age = age
        }
        // new Dog()->Dog.prototype->Animal.prototype
        // new Animal()->Animal.prototype
        // 一.继承
        // 1.原型链继承：将父类的实例作为子类的原型对象
        //  作用：一般都用于继承父类原型链里面的所有方法。
        //  例如：父类Animal 子类Dog  原型链：new Dog()-->new Animal()-->Animal.prototype
        //  缺点：无法操作父类的属性，若不传值给父类，父类的属性为undefined。
        // 2. 借用构造函数
        Dog.prototype = new Animal();
        var wangcai = new Dog(2);
        console.log(wangcai);

```

#### 2. 借用构造函数

核心：借用父类的构造函数来增强子类实例，相当于把父类的实例复制一份给子类实例

- call：

  - 格式：父类构造函数.call(子类实例，参数1，参数2，参数3...)

- apply：

  - 格式：父类构造函数.apply(子类实例,[参数1,参数2,参数3...])
    call与apply的唯一区别：传参方式不同，call多个参数，apply只有两个参数，第二个参数为数组

    ```
    //aplly用法：借用方法
    var arr = [20,2,40,33,21,8,22,46,32]
    Math.max.apply(null,arr)
    
    ```

    ```
    function Animal(jiaosheng,color){
                this.jiaosheng = jiaosheng,
                this.color = color
            }
            Animal.prototype = {
                constructor : Animal,
                fanzhi : function(){
                    console.log("卵生");
                },
                eat : function(){
                    console.log("吃好吃的");
                }
            }
            function Dog(color){
                Animal.call(this,"旺",color);//传参
            }
         
    
    
         
            Dog.prototype = new Animal();
            var wangcai = new Dog("black");
            console.log(wangcai);
    
    
    
    ```

    

#### 3. 组合继承

由于以上继承方法的缺点，实际开发中不可能单纯的只使用一种继承方法，而是利用他们的优点，规避它们的缺点，所以就有了组合继承法

- 继承属性：借用构造函数
  - 只在构造函数中定义属性
- 继承方法：原型链继承
  - 把所有的方法写入原型对象
    - 例如

```
  function Animal(jiaosheng,color){
            this.jiaosheng = jiaosheng,
            this.color = color
        }
        Animal.prototype = {
            constructor : Animal,
            fanzhi : function(){
                console.log("卵生");
            },
            eat : function(){
                console.log("吃好吃的");
            }
        }
        function Dog(color){
            Animal.call(this,"旺",color);
        }

```

##### 组合继承是最常用的继承模式

缺点（原型链继承法的缺点）：

- 在原型对象中生成多余的属性
- 多次执行父类构造函数

```
//原型链继承基础上补充借用构造函数
function Man(name,age){
    Person.call(this,name,age,'男');
}

```

#### 4. 原型式继承

- 核心：先创建了一个临时性的构造函数，然后将传入的对象作为这个构造函数的原型，最后返回了这个临时类型的一个新实例
- 解决原型链继承法的缺点：生成多余的属性

```
function object(o){
    function F(){}
    F.prototype = o;
    return new F();
}
Man.prototype = object(Person.prototype);

```

```
   function Animal(jiaosheng,color){
            this.jiaosheng = jiaosheng,
            this.color = color
        }
        Animal.prototype = {
            constructor : Animal,
            fanzhi : function(){
                console.log("卵生");
            },
            eat : function(){
                console.log("吃好吃的");
            }
        }
        function Dog(color){
            Animal.call(this,"旺",color);
        }
     
        function object(o){
            function F(){}
            F.prototype = o;
            return new F();
        }
        Dog.prototype = object(Animal.prototype);
        ============================================
        // es5原型式继承：
        Dog.prototype = Object.create(Animal.prototype);


        // Dog.prototype = new Animal();
        var wangcai = new Dog("black");
        console.log(wangcai);

```



###### ES5版本的原型式继承：Object.create()

```
   Dog.prototype = Object.create(Animal.prototype);

```

![1.组合继承原型链图](E:\H5每天\二阶段18.8.13\25.9.18\25-27.OOP&Inherit、闭包\doc\神笔马良\1.组合继承原型链图.png)

#### 5. 寄生组合继承法

完美的继承方法

- 核心：
  - 继承属性：借用构造函数
  - 继承方法：原型式继承

## 五、ES6继承

### class定义类

- 写在类里面的方法实际是给Person.prototype添加方法
- constructor方法是类的默认方法，相当于在构造函数内生成属性

### extends继承

- 子类继承父类，在子类构造函数中必须调用super方法
- 子类的constructor方法没有调用super之前，不能使用this关键字，否则报错，而放在super方法之后就是正确的

```
class Animal{
            constructor(jiaosheng,color){
                this.jiaosheng = jiaosheng;
                this.color = color;
            }
            fanzhi(){
                console.log("卵生");
            };
            static eat(){
                console.log("吃好吃的");
            }
        }
        class Dog extends Animal{
            constructor(jiaosheng,color){
                super(jiaosheng,color);
                this.love = "gutou";
                // this.jiaosheng = jiaosheng;
                // this.color = color;
            }
        }

        class Cat extends Animal{
            
        }



        var wangcai = new Dog("旺","black");
        // wangcai.eat();
        Animal.eat();
        Dog.eat();

```

### 静态方法

如果在一个方法前，加上static关键字，这就称为“静态方法”

- 静态方法方法不会被实例继承，而是直接通过类来调用`Person.getInfo()`

- 父类的静态方法，可以被子类继承`Man.getInfo()`

  ```
  class Person{
      constructor(name,age,gender){
          this.name = name;
          this.age = age;
          this.gender = gender;
      }
      // 此处的方法写入原型对象中
      say(){console.log(大家好,我叫${this.name})}；
      static eat(){console.log('我是吃货');}
  }
  let lemon = new Person('lemon',32,'女');
  // 继承方法
  class Man extends Person{
      constructor(name,age){
          // 继承属性
          super(name,age,'男');
          this.hobby = ['吃','喝'];
      }
  }
  let laoxie = new Man('laoxie',18);
  
  ```

## 六、call和apply的使用

```
* 求数组中最大数和最小数
    * Math.max()
    * Math.min()
* 类数组使用map
* 判断数据类型
    * typeof
    * Object.prototype.toString()

```

## 七、闭包

闭包是这样一种机制: 函数嵌套函数, 内部函数可以引用外部函数的参数和变量,参数和变量不会被垃圾回收机制所收回.

这里涉及到几个概念:

1. 函数嵌套函数
2. 作用域(全局变量和局部变量)
   变量的访问规则
3. 垃圾回收机制(garbage collection)
   js内部不断扫描内存,并清理无引用对象(自动完成);

```
    function aa(){
        var num=10;
        function bb(){
            num++
            console.log(num);
        }
        return bb;
    }
    //bb(); //无法直接访问函数内部的函数

    aa()();//11
    aa()();//11
    aa()();//11

    var closure = aa();
    closure();//11
    closure();//12
    closure();//13

```

### 闭包的好处

1. 可以让一个变量长期驻扎在内存当中不被释放
2. 避免全局变量的污染, 和全局变量不同, 闭包中的变量无法被外部使用
3. 私有成员的存在, 无法被外部调用, 只可以自己内部使用

> 结论：

- 闭包是指有权访问另一函数作用域中的变量的函数
- 闭包，可以访问函数内部的局部变量，并让其长期驻留内存
- 由于闭包会携带包含它的作用域(运行环境)，因此会比其他函数占用更多内存，过度使用闭包可能会造成性能问题。

# 封装案例讲解

## 弹窗插件

```
function Popover(options){
	//1.设置默认值，与传进来的对下那个进行合并
	var defaults = {
		width:600,
		height:'auto',//可以是数值
		position:'center',//可以传进来对象{x,y}
		title:'弹窗标题',
		content:'',
		draggable:true,
		overlay:0.3 //数字：有遮罩层，false：无遮罩层
	}
    var opt = Object.assign({},defaults,options);
    this.position = opt.position;
    this.init(opt);
}
Popover.prototype = {
	init(opt){
		//2.初始化方法：
		//（1）创建弹窗this.ele，设置宽高
		this.ele = document.createElement('div');
		this.ele.className = 'popover';
    	this.ele.style.width = opt.width + 'px';
    	if(typeof opt.height === 'number'){
    		this.ele.style.height = opt.height + 'px';
    	}
		//（2）标题和内容（设置类名title、content）
    	var title = document.createElement('div');
    	title.className = 'title';
    	title.innerHTML = opt.title;
    	this.ele.appendChild(title);
    	var content = document.createElement('div');
    	content.className = 'content';
    	content.innerHTML = opt.content;
    	this.ele.appendChild(content);
    	// (3)遮罩层(判断overlay是数字则为透明度，为false则不设置遮罩层)（类名、透明度）
    	if(opt.overlay !== false){
    		this.bg = document.createElement('div');
    		this.bg.className = 'overlay';
    		this.bg.style.opacity = opt.overlay;
    		document.body.appendChild(this.bg);
    	}
    	// （4）删除按钮（类名、内容）
    	var btnClose = document.createElement('span');
    	btnClose.className = 'btn-close';
    	btnClose.innerHTML = '&times;';
    	this.ele.appendChild(btnClose);
    	// （5）弹窗写入页面，并显示弹窗
        document.body.appendChild(this.ele);
        this.show();
    	// （6）设置关闭事件
    	btnClose.onclick = function(){
    		this.close();
    	}.bind(this);
        //（7）拖拽
        if(opt.draggable){
            this.drag();
        }
	},
	//3.1显示：设置成块，同时调用定位方法
	show(){
		this.ele.style.display = 'block';
		if(this.bg){
			this.bg.style.display = 'block';
		}
		this.setPosition();
	},
	//3.2隐藏：
	close(){
		this.ele.style.display = 'none';
		if(this.bg){
			this.bg.style.display = 'none';
		}
	},
	//4.定位：判断是否传参
	//（1）若没有参数，即x值为undefined，则判断this.postion的值为center还是对象，设置x、y值
	//（2）给元素设置样式
	setPosition(x,y){
		if(x===undefined){
			// 如果元素没有添加(并显示)到页面，获取不到宽高
			if(this.position === 'center'){
				x = (window.innerWidth - this.ele.offsetWidth)/2;
				y = (window.innerHeight - this.ele.offsetHeight)/2;
			}else if(typeof this.position === 'object'){
				x = this.position.x;
				y = this.position.y;
			}
		}
		this.ele.style.left = x + 'px';
		this.ele.style.top = y + 'px';
	},	
	//5.拖拽
	drag(){
		var self = this;
		var pop = self.ele;
		pop.onmousedown = e=>{
			var ox = e.clientX - pop.offsetLeft;
			var oy = e.clientY - pop.offsetTop;
			// 只能在标题位置拖拽
			if(oy>pop.children[0].offsetHeight){
				return;
			}
			document.onmousemove = function(evt){
				var x = evt.clientX - ox;
				var y = evt.clientY - oy;
				self.setPosition(x,y);
				evt.preventDefault();
			}
		}
		document.onmouseup = function(){
			document.onmousemove = null;
		}
	}

```

#### 弹窗继承

```
//确认对话框
function Confirm(options){
	var defaults = {
		width:300,
		title:false,
		content:'你确定这个操作吗',
		overlay:false,
		confirm:function(){},
		cancel:function(){}
	}
    var opt = Object.assign({},defaults,options);
    //1.借用构造函数，拿到弹窗对象属性this.ele及this.position
    Popover.call(this,opt);
}
// 2.继承Popover的方法
Confirm.prototype = Object.create(Popover.prototype);
//3.添加/重置方法
Confirm.prototype.init = function(opt){
	//3.1把你需要的部分复制下来
	//3.2添加确认取消按钮
	this.confirmBtn = document.createElement('button');
	this.confirmBtn.className = 'btn-confirm';
	this.confirmBtn.innerText = '确认';

	this.cancelBtn = document.createElement('button');
	this.cancelBtn.className = 'btn-cancel';
	this.cancelBtn.innerText = '取消';
	this.ele.appendChild(this.confirmBtn);
	this.ele.appendChild(this.cancelBtn);
	
	// 3.3点击确认取消按钮，执行方法
	this.confirmBtn.onclick = ()=>{
		opt.confirm();
		this.close();
	}
	this.cancelBtn.onclick = ()=>{
		opt.cancel();
		this.close();
	}

```

## 时间格式化

```
if(!Date.prototype.format){
    Date.prototype.format = function(fmt){
        //fmt格式：“YYYY-MM-DD hh:mm:ss”
        var o = {
            "M+" : this.getMonth()+1,
            "D+" : this.getDate(),
            "h+" : this.getHours(),
            "m+" : this.getMinutes(),
            "s+" : this.getSeconds()
        };
        if(/(Y+)/.test(fmt)){
            var res = String(this.getFullYear()).substr(4-RegExp.$1.length);
            fmt = fmt.replace(RegExp.$1,res);
        }
        for(var str in o){
            var reg = new RegExp('('+str+')');
            if(reg.test(fmt)){
                var res = RegExp.$1.lenth>1? ("00"+o[str]).substr(String(o[str]).length) : o[str];
                //9===>009.substr(1)
                //0012===>0012.substr(2)
                fmt = fmt.replace(RegExp.$1,res);
            }
        }
        return fmt;
    }
}

```

```
var str = "X98Y87Z65";
// 三个数字部分加了小括号，表示子表达式
var reg = /^X(\d+)Y(\d+)Z(\d+)$/;
reg.test(str); // 此处使用exec()等其他正则表达式的匹配方法也可，下同
document.writeln(RegExp.$1); // 98
document.writeln(RegExp.$2); // 87
document.writeln(RegExp.$3); // 65

```

## 简化DOM节点操作

```
* 面向对象的DOM操作
* show()：显示
* hide()：隐藏
* on()：事件绑定
* css()：获取/设置Css样式
* addClass()：添加类名
* removeClass()：移除类名
* attr():获取/设置html属性值
* html()：设置/获取html内容
* text()：设置/获取文本内容

```



```
class xJquery{
	// 1.this.ele获取初始化
	constructor(selector){
		// 1.1若不是传入字符串，则可能传入DOM节点（判断选择器的标签名是否存在）或类数组Array。
		// this.ele得到值，退出该函数
		if(typeof selector != 'string'){
			if(selector.tagName){
				this.ele = [selector];
			}else{
				this.ele = selector;
			}
    		return;
		}
		//1.2若传入的是选择器
        try{
            this.ele  = document.querySelectorAll(selector);//Nodelist
        }catch(error){
            var selectorName = selector.slice(1);
            if(/^#/.test(selector)){
                //变成数组为的是后面的遍历
                this.ele = [document.getElementById(selectorName)];//Array
            }else if(/^\./.test(selector)){
                try{
                    this.ele = document.getElementsByClassName(selectorName);//HTMLCollection
                }catch(err){
                    this.ele = [];
                    var res = document.getElementByTagName('*');
                    for(var i=0;i<res.length;i++){
                        var className = res[i].className.split(' ');
                        if(className.indexOf(selectorName)>=0){
                            this.ele.push(res[i]);
                        }
                    }
                }
            }else{
                //getElementsByTagName
                this.ele = document.getElementsByTagName(selector);
            }
		}
	}
	//2.显示隐藏方法
	show(){
        Array.prototype.forEach.call(this.ele,function(ele){
            ele.style.display = 'block';
        });
        // 方便链式调用
        return this;
    }
    hide(){
        Array.prototype.forEach.call(this.ele,function(ele){
            ele.style.display = 'none';
        });
        return this;
    }
    // 3.事件绑定
    on(type,handler,isCapture){
        Array.prototype.forEach.call(this.ele,function(ele){
            try{
                ele.addEventListener(type,handler,isCapture)
            }catch(error){
                try{
                    ele.attachEvent('on' + type,handler);
                }catch(err){
                    ele['on'+type] = handler;
                }
            }
        });
        return this;
    }
    // 4.获取/设置Css样式
    css(key,value){
        // 若没有传入value，则代表获取值，只获取第一个元素的值
        if(value === undefined){
            if(window.getComputedStyle){
                return getComputedStyle(this.ele[0])[key]
            }else if(this.ele[0].currentStyle){
                return this.ele[0].currentStyle[key]
            }else{
                return this.ele[0].style[key]
            }
        }
        // 设置，则设置所有元素的值
        Array.prototype.forEach.call(this.ele,function(ele){
            ele.style[key] = value;
        })
        return this;
    }
    // 5.给所有元素添加类名
    addClass(name){
        Array.prototype.forEach.call(this.ele,function(ele){
            try{
                ele.classList.add(name);
            }catch(error){
                var className = ele.className.split(' ');
                if(className.indexOf(name) == -1){
                    className.push(name);
                }
                ele.className = className.join(' ');
            }
        })
    }
    // 6.移除所有元素的该类名
    removeClass(name){
        Array.prototype.forEach.call(this.ele,function(ele){
            ele.classList.remove(name)
        });
    }
    // 7.设置/获取html内容
    html(html){
        // 获取第一个元素的html内容
        if(html === undefined){
            return this.ele[0].innerHTML
        }
        // 设置所有元素的html内容
        Array.prototype.forEach.call(this.ele,function(ele){
            ele.innerHTML = html;
        });
        return this;
    }
    // 设置/获取文本内容
    text(txt){}
}
//执行$(selector)，返回实例对象
let $ = function(selector){
	return new xJquery(selector);
}

```

# 9.25 jQuery

## 一、了解jQuery

JQuery是一个兼容多浏览器的javascript类库，核心理念是write less,do more(写得更少,做得更多)。是一个快速的简洁的javascript框架，可以简化查询DOM对象、处理事件、制作动画、处理Ajax交互过程。在2006年1月由美国人John Resig在纽约的barcamp发布。 

作者：John Resig

官方网站：<http://jquery.com/> 

![zz](E:\H5每天\二阶段18.8.13\28.9.25\29-31jquery\doc\img\zz.jpg)

## 二、jQuery版本

- 1.x.x
  - 兼容低版本浏览器IE8-
  - 代码过于庞杂，性能不高
  - 最新版本1.12
- 2.x.x
  - 已经不支持IE低版本浏览器IE8-
  - 最新版本2.
- 3.x.x
  - 3.0 版本是从 2.0 版本分支出来的，但由于改动过大，因此更新了主版本号
  - 不支持IE低版本浏览器
  - 性能大幅度提高（推荐使用）
- *.*.* (主版本-次版本-补丁 

## 三、下载与安装

- 官网下载
  <http://jquery.com/download/>

CDN

- <https://code.jquery.com/jquery-3.0.0.js>
- <https://code.jquery.com/jquery-3.0.0.min.js>

## 四、jQuery实现原理

- jQuery构造函数
- jQuery实例对象

```
Query('#box');//得到jquery对象（实例）

```

```
**jquery对象只能用jquery的方法** 

```

#### 1. jQuery实例属性

```
length ：返回jQuery对象中匹配元素的个数
jQuery ：当前jQuery类库版本号
下标（索引）：	DOM节点

```

#### 2. jQuery的别名 : $

#### 3. 延迟代码执行：jQuery(document).ready(fn)

```
此方法传入一个匿名函数;
页面DOM渲染完成时执行;
简写方式:jQuery(function(){});
安全使用$:jQuery(function($){});
	解释：就是相当于document.addeventlistener("DOMContentLoaded",function(){})
	jQuery(function($){}); //直接写成这样既可

```

#### 4. 编写jQuery代码只需两步

```
1.选择元素
2.操作元素

```

```
var $box = $(".box");
//$box.css("border","5px solid #58bc58");
box.css({'border':'5px solid #58bc58',padding:'20rem'})
//获取$box下面的button
//let btns = $('button',$box);
let btns = $('button','.box');


```

###### 加：

```
$("#output .son")

$(".son",$output)
	*两个为一样的意思，第一个为正常写法双引号把两个包住，第二个是父元素不用包，前面表示它的子元素。

```

```
jQuery(function($){
            // $("#output .son").css("color","red");
            // var $output =  $("#output");
            // $("#output .son").css({color:'red',width:'200px',backgroundColor:'#58bc58'});
            $(".son",$output).css({color:'red',width:'200px',backgroundColor:'#58bc58'});
        })
        
        
解释：1.获取元素可直接通过$()的方式获取，括号里面为你要获取的元素，是id就为#，是类就为.
	例如：var $output =  $("#output");
	2.给元素添加样式，直接.css既可。有两种方式：
	（1）("color","red");
	（2）(color:'red')
	3.获取jQuery得到的都是数组
		*如何利用得到的jquery，判断是否存在该元素:jQuery("#lemon").length !=0

```

## 五、选择器

定义：选择页面中的元素，得到jQuery实例对象

- ID选择器$(“#save”)

- 类选择器$(“.class”)

- 标签选择器$(“div”)

- 复合选择器 $(“div,span,p.myClass”)

- 属性选择器$(‘[id=box]’)

  - (‘li[data-index]’):获取有data-index属性的所有元素
  - $(‘li[data-index!=10]’):data-index属性不等于10的元素,css目前未支持
  - $(‘li[data-index^=10]’):data-index属性以10开头的元素
  - $(‘li[data-index$=10]’):data-index属性以10结尾的元素
  - $(‘li[data-index*=10]’):data-index属性包含10的元素

- 表单选择器$(‘:input’)

  - :radio //匹配所有单选按钮
  - :checkbox //匹配所有复选按钮
  - :selected //获取已选择的option元素
  - :checked //匹配所有被选中的元素(复选框、单选框等，select中的option)
  - :submit //匹配所有提交按钮
  - :reset //匹配所有重置按钮
  - :button //匹配所有按钮
  - :text //匹配所有的单行文本框
  - :password //匹配所有密码框

- 可见性

  :hidden //匹配所有不可见元素(display:none)，或者type为hidden的元素
  :visible //匹配所有可见元素

> 以上两个选择器配合is()方法通常用于判断，返回布尔值
>
> ```
> if(box.is(':visible')){
>     box.css('display','none');
> }
> 
> ```

## 六、常用操作

### （一）

- jquery对象与原生对象的转换
  - jquery转原生
    - get(0)/[0]获取集合中第一个DOM节点
    - get()不传参得到集合中所有的dom节点1
  - 原生转jquery:$(dom)
- 判断是否为jquery对象

```
var box = $('#box');
if(box.jquery){

}

```

- 判断一个jquery对象是否存在(是否能获取到元素)
  - length
  - 转成原生对象再判断

### （二）筛选

定义：利用选择器得到的结果不一定是我们想要的最终结果，有时需要进一步筛选

#### 1.基本筛选

- :odd/even,gt(n)/:lt(n) 筛选范围（索引支持负数）
- :contains（奥巴马）筛选出包含“奥巴马”这三个字的元素

例如：

```
 $('table td:contains("蓝梦")').css("backgroundColor","#58bc58");

```

#### 2. 筛选方法

- first()/last() ：获取集合中第一个/最后一个元素
- eq(index|-index) ：获取第N个元素，n支持负数（表示从后面查找）
- filter(expr|obj|ele|fn) ：筛选出与指定表达式匹配的元素集合。这个方法用于缩小匹配的范围。用逗号分隔多个表达式

```
 filter(选择器|jquery对象|dom节点|fn): 过滤得到满足条件的jquery对象。

```

- map(fn): 将一组元素转换成其他数组（不论是否是元素数组）

- slice(start,[end]): 选取一个从start到end(不包括end)匹配的子集

- has(expr|ele): 保留包含特定后代的元素，去掉那些不含有指定后代的元素。

  ```
  $('table tr').has('.aa').css("backgroundColor","#58bc58")
  
  解释：table里面包含.aa的那个tr都变成绿色
  
  ```

  

- not(expr|ele|fn): 删除与指定表达式匹配的元素

```
$('table td').not('.aa').css("backgroundColor","#58bc58");

解释：table里面的td里面除了.aa以外的元素都是绿色

```

## 七、查找

定义：利用当前元素去查找其他元素

#### 1. 查找子元素

- find(expr|obj|ele): 查找后代元素	

  ```
  $("#yeye").find("div").css("backgroundColor","red");
  备注：find是查找yeye的所有后代包括孙子那辈
  
  ```

  

- children([expr]): 取得匹配元素的所有子元素。(原生js:children)

```
$("#yeye").children("div").css("backgroundColor","red");
备注：children是只查找yeye的下一辈，查不到孙子那辈

```

#### 2. 查找父级元素

- parent([expr]): 获取父元素

- parents([expr]): 取得所有父级元素

- closest(expr|obj|ele): 从元素本身开始，逐级向上级元素匹配，并返回最先匹配的元素

  ```
   $(".nver").closest("span").css("backgroundColor","red");
   备注：离它最近的那个span父元素
  
  ```

- offsetParent(): 返回第一个有定位属性(absolute,relative,fixed)* 的父元素,如果没有定位父级，则返回html元素

```
$(".nver").offsetParent().css("backgroundColor","red");
备注：离他最近的有定位的父元素

```

#### 3. 查找兄弟元素

- next([expr]): 返回下一个同辈元素 ==> nextElementSibling
- prev([expr]): 获取前一个同辈元素 ==> previousElementSibling
- nextAll([expr]): 获取当前元素之后所有的同辈元素
- prevAll([expr]) 获取当前元素之前所有的同辈元素
- siblings([expr]) 获取当前元素的所有兄弟元素（除自身以外的所有兄弟元素 = * prevAll + nextAll）

# 9.26

# DOM节点操作

## 一、增删改

#### 1. 创建节点

```
$("<标签/>)
例如：$("<div/>")
	 $("<div>这是一个div</div>")

```

#### 2. 元素添加

```
（1）内部添加（添加为子元素）
		*append(content|obj|ele|fn)  追加到父元素里面，最后面
		jq对象.append(子节点) //作为最后一个子节点
（2）	   *prepend
		 jq对象.prepend(子节点) 作为第一个子节点
		 	*子节点.appendTo(jq对象)
		 	*子节点.prependTo(jq对象)
备注：下面这两个带To的和上面的意思是一样的，都是将内容追加到父节点里面
	例如：$('<div>创建的div</div>').appendTo($father);
		 $("body").prepend($('<div>创建的div</div>'));

```

#### 3. 作为兄弟节点插入

```
jq对象.before(节点) //在jq对象前面插入
jq对象.after(节点)	//在jq对象后面插入
	*节点.insertBefore(jq对象)
	*节点.insertAfter(jq对象)	//同上面两个意思一样
例如：$father.before('<p>hello</p>');

```

#### 4.  删除

```
remove(); 删除元素，虽然元素从文档中删除了，但js内部仍然保留对它的引用
empty();  清空内容
例如：(this).closest("tr").remove();

```

#### 5. 复制

```
clone() 把整个jq对象复制，包括里面的内容、
	*Event：是否复制当前jq对象的行为，默认为false
	*deepEvent:是否复制子元素的行为，默认为Event的值
解释：当clone里面的第一个参数为true时，把里面的所有东西都复制了，包括子元素什么的；
	 当第一个参数为true时，第二个也默认为true，当第二个也为true时，就连它的行为也复制了，也就是它的方法函数等等
	 例如：$('body').append($father.clone(true,false));

```

## 二、盒模型相关

- .offset():获取匹配元素相对于根元素的偏移量
  返回一个对象，包含当前元素的top,left值
- position():获取匹配元素相对(有定位属性)父元素的偏移量，如果没有定位父级，则相对于根元素(html)，返回一个对象，包含当前元素的top,left值。
- width(v) = width; //取值/赋值,当传入v时，相当于css(‘width’,v);
- innerWidth() = width + padding; <==> clientWidth
- outerWidth() = width + padding + border; <==> offsetWidth
- outerWidth(true) = width + padding + border + margin;

```
 	   client
             -width
             -height  (padding + content)
        scroll
            -left 
            -top 元素滚动条滚动过后的距离 

```

## 三、jQuery动画

### （一）基本动画效果

#### 1. 显示隐藏：show()/hide()

- hide(duration)通过改变元素的高度、宽度、和不透明度，直到这三个属性值到0
- show(duration)通过改变元素的高度、宽度、和不透明度，直至内容完全可见

#### 2. 滑动（通过改变高度）

- slideDown([speed,callback])：

1. 显示元素
2. 不断改变高度，直到样式内设定的值

- slideUp([speed,callback])： 
  1. 不断改变高度，直到0
  2. 隐藏元素
- slideToggle([speed,callback])
  当元素隐藏时调用slideDown()，当元素显示时调用slideUp()

#### 3. 淡入淡出（通过改变不透明度）

- fadeIn:
  1)显示元素
  2)不断改变透明度直到1
- fadeOut:
  1)不断改变透明度直到0
  2)隐藏元素
- fadeToggle([speed,callback])
- fadeTo([[speed],opacity,[fn]]) 不断改变透明度opacity，直到设定的值，并在动画完成后可选地触发一个回调函数。

PS：jQuery动画由三种预设速度slow,normal,fast（600，400，200） 

### （三）自定义动画

- animate (params,[speed],[fn])
- :animated
  获取正在执行动画的元素，一般与is()方法配合使用，用于判断元素是否处于动画状态

### （四）动画队列

- 一个元素上的动画：
  - 当animate中存在多个属性时，动画同时发生
  - 当同一个元素链式调用animate时，动画是按顺序发生(队列)
- 不同元素上的动画：
  - 默认情况下，动画同时发生
  - 回调函数内的动画等到当前动画执行完后才接着执行
- stop([clearQueue],[jumpToEnd])
  不加参数：停止当前元素所有《正在运行》的动画。
  - clearQueue:值为true时，清除队列
  - jumpToEnd:值为true时，跳到当前动画的最后一帧
- delay(duration)
  设置一个延时来推迟执行队列中之后的动画。
  - duration:延迟的时间

## 四、事件

### （一）常用事件方法

- 鼠标事件
  - click([[data],fn]) //点击时触发 click = mousedown + mouseup
  - dblclick([[data],fn]) //双击事件 dblclick = 2*click
  - mousedown([[data],fn])
  - mouseup([[data],fn])
  - mousemove([[data],fn])
  - mouseout([[data],fn])
  - mouseover([[data],fn])
  - mouseenter([[data],fn]) //事件不会冒泡
  - mouseleave([[data],fn]) ) //事件不会冒泡
- 键盘事件
  - keydown([[data],fn]) //键盘按下时触发
  - keypress([[data],fn])//字符按键
  - keyup([[data],fn]) //键盘弹起时触发
- 表单事件
  - blur([[data],fn]) //失去焦点时触发
  - focus([[data],fn]) //获得焦点
  - change([[data],fn]) //值改变并失去焦点时触发
  - submit([[data],fn])
- 其他事件
  - resize([[data],fn]) //元素大小改变时触发
  - scroll([[data],fn]) //滚动时触发

### （二）jquery事件绑定与移除

- on(type,[selector],fn)
  - selector: 把本来绑定给selector的事件委托给它的父级
  - 事件命名空间, 自定义事件（对事件加以细分）
    `格式：事件类型.自定名字`
  - 一次性绑定多个事件，事件之间以空格隔开
  - 支持自定义事件的绑定
    `$(ele).on('laowang',function(){})`
    触发自定义事件：$(ele).trigger(‘laowang’);
- off: 清除绑定事件
  - off(‘click’);//清除当前元素的点击事件
  - off();//清除当前元素所有事件
  - off(‘click mouseover’) 一次性清除多个事件，事件之间以空格隔开
  - off(‘click.output’) 清除命名空间事

### （三）其他事件方法

- hover(enter[,leave])
  - enter:鼠标移入时执行
  - leave:鼠标移出时执行

> hover方法内部使用mouseenter + mouseleave来实现效果 

- trigger(type): 手动触发事件（即使事件没有发生，也能执行事件处理函数）
- triggerHandler(type): 这个方法会触发指定的事件类型上所有绑定的处理函数。但不会执行浏览器默认行为，也不会产生事件冒泡
- 阻止浏览器默认行为
  event.preventDefault();
- 阻止事件传播
  event.stopPropagation();
- 两者一起阻止：
  return false;

## 五、ajax

- $.ajax(settings)
  - type:请求类型，默认GET
  - url:数据请求地址（API地址）
  - data:发送到服务器的数据对象，格式：{Key:value}。
  - success:请求成功时回调函数。
  - dataType:设定返回数据的格式，json, jsonp, text(默认), html, xml, script
  - async：是否为异步请求，默认true
- $.get(url,[data],[fn],[dataType]) // type:’get’
- $.post(url,[data],[fn],[dataType]) // type:’post’
- $.getJSON(url,[data],[fn]) // type:’get’, dataType:’json’
- $.getScript(url,[callback]) // type:’get’, dataType:’script’
- load(url,[data],[callback]) 载入远程 HTML 文件代码并插入页面中。

## 六、常用jQuery原型对象的方法

定义：写在jquery原型对象中的方法，通过jquery实例调用

#### 1. css(attr[,val]): 获取/改变元素style属性（内联样式）

- 取值：css(attr),css([‘color’,’text-align’]) <==> getComputedStyle[attr]
- 赋值：css(attr,val),css({attr:val});

#### 2. val(v): 获取/设置匹配表单元素的值（等同于原生js中的value属性）

- 取值：
  `input.val()`
- 赋值：
  `input.val(v)`
  - v:字符串
  - v:数组（一般用于单选/复选框的勾选）
  - v:函数function(idx,val){ return 值}//函数内部一定要返回值

#### 3. html(): （等同于原生js中的innerHTML）

- 取值div.html()：取得第一个匹配元素的html内容 
- 赋值div.html(‘:’)：设置匹配元素的内容 
- text(): 取得所有匹配元素的文本内容。
- addClass()/removeClass(): 添加/删除类,支持多个类同时添加或删除
  - toggleClass(): 如果存在（不存在）就删除（添加）类。
  - hasClass(‘con’): 判断当前元素是否包含con这个类，返回布尔值（不支持多个类进行判断）
- eq(n) 获取第N个jquery对象（元素）,n支持负数（表示从后面查找）
- index():获取当前元素在同辈元素中的索引值

```
$(this).index();

```

#### 4. 显示/隐藏

- show()：显示元素
- hide()：隐藏元素
  - 带参数：同时改变width,height,opacity的动画
- is(expr|obj|ele|fn) 根据选择器、DOM元素或 jQuery 对象来检测匹配元素集合，其中如果有一个元素符合这个给定的选择器表达式就返回true。如果没有元素符合，或者表达式无效，都返回false。
- attr(name[,val]) 设置/获取html标签属性

#### 5. prop(attr[,val]) 获取/设置DOM节点属性（一般修改布尔类型属性）

- 获取：获取在匹配的元素集中的第一个元素的属性值。
- 赋值：给集合中所有元素属性赋值
  - val为函数 

```
$(':checkbox').prop('checked',function(idx,oldVal){
    return !oldVal;
}

```

#### 6. each(function(idx,ele){}) //用于遍历jquery对象

- return true;// 跳过当前循环，进入下一个循环（等效原生js中得continue）
- return false;// 退出整个each循环（等效原生js中得break）

## 七、jquery大部分方法的共性

```
1. 无参数时为取值，带参数时为赋值。
2. 取值，取得第一个匹配元素的值。
3. 赋值，设置所有匹配元素的值。
4. 隐式迭代（隐式遍历），看不见的遍历，大部分的jquery方法都支持隐式迭代。

```

## 八、col-xs       col-sm      col-md     col-lg

```
 xs 768px以下      sm 768-992px           md992-1200     lg1200
 	*例如：
 	  <div class="col-xs-4 col-sm-6 col-md-8 col-lg-12"></div>
      <div class="col-sm-4 col-md-4 col-lg-12"></div>

```

## 九、常用jQuery静态方法

- $.each(arr|obj,callback)：通用遍历方法，用于遍历对象和数组。
  - callback(idx,item)
- $.map(arr|obj,callback)：根据现有数组生成一个新的数组，新数组的元素为callback内return的值
  - callback(item,idx)
- $.type(n)：检测参数n的数据类型
- $.makeArray(obj) //将类数组对象转换为数组。
- $.parseJSON(json) //接受一个JSON字符串，返回解析后的对象。类似原生js中的JSON.parse
- $.inArray(value,array,[fromIndex]) //确定value在数组array中的位置，从0开始计数(如果没有找到则返回 -1 )，一般用于判断数组中是否包含某一字符。
- serialize()/serializeArray() : 只能在form表单中使用，并且表单元素必须有name属性

# 9.30 gulp

定义：gulp是当下最流行的自动化工具 ，可以自动化完成我们开发过程中大量的重复工作。如：

> 编译：
> 	less->css
> 	sass->css
> 	coffeescript->js
> 	es6->es5(兼容)
> 合并: css, js
> 压缩 ：css, js, html
> 优化：图片优化

- 官网：<http://gulpjs.com/> 
- 中文网：<http://www.gulpjs.com.cn/> 

### gulp的安装及运行

##### 1.全局安装 gulp：

```
npm install --global gulp    //全局安装gulp目的是为了通过它执行gulp任务

```

##### 2.本地安装gulp：

作为项目的开发依赖（devDependencies）安装：

```
npm install --save-dev gulp //本地安装gulp是为了调用gulp插件的功能

```

- –save-dev 保存配置信息至 package.json 的 devDependencies 节点
- 这步操作前先新建package.json文件（npm init）
- 这步完成后就可以安装各种gulp插件了

##### 3.安装gulp插件

大部分插件都可以在http://www.npmjs.com找到，任何插件的使用都要经历以下三步：

> 安装插件：npm
> npm install  gulp-htmlmin

PS：可一次性安装多个插件，插件间用空格隔开

###### 常用gulp插件

> html压缩：gulp-htmlmin
>
> css压缩：gulp-clean-css
>
> js压缩：gulp-uglify
>
> 合并文件：gulp-concat
>
> 文件重命名：gulp-rename
>
> 编译Sass: gulp-sass
>
> 编译 Less：gulp-less

###### 其他常用插件

> - 浏览器同步测试：browser-sync
> - 创建node服务器：http-server 
>
> npm install -g http-server

##### 4.创建gulpfile.js文件（gulp任务）

- ！！！项目根目录下 创建
- gulp项目的配置文件，内容如下：

```
var gulp = require('gulp');
gulp.task('任务名', function() {
  // 将你的默认的任务代码放在这
});

```

##### 5.运行 gulp：

在命令行执行以下命名，如果不写任务名称，则自动运行default任务（如果有）

```
gulp <任务名称>

```

###### 演示：编译scss文件为css文件

```
//1.安装gulp-sass插件
//2.gulpfile.js:
//(1)引包：require()：返回对象或者函数
let gulp = require('gulp');//得到对象
let sass = require('gulp-sass');//得到函数
//(2)创建任务
gulp.task('compileSass',function(){
	// （3）执行gulp工作流程
	gulp.src('./src/sass/*.scss') // 返回文件流（液体，文件在内存中的状态）
	.pipe(sass({outputStyle:'expanded'}).on('error', sass.logError))
	.pipe(gulp.dest('./src/css/'))
});
	
outputStyle参数（gulp-sass）：
    nested(默认）
    expanded：展开
    compact：单行
    compressed：压缩
on('error', sass.logError)：忽略错误，继续编译

```

### gulp工作流程

1. 选通过gulp.src(globs) 方法获取到想要处理的文件，并返回文件流
2. 然后文件流通过 pipe 方法导入到 gulp 的插件中
3. 经过插件处理后的文件流，再通过pipe方法导入到 gulp.dest() 方法中
4. 最后通过gulp.dest() 方法把流中的内容写入到文件中

> PS：文件流=>文件在内存中的状态

   5.监听文件修改，并执行相应任务gulp.watch(glob,[‘任务名’])

###### 演示：监听scss文件修改，自动编译

```
gulp.task('jtSass',function(){
	gulp.watch('./src/sass/*.scss',['compileSass'])
})

```

### globs语法

globs需要处理的源文件匹配符路径，语法如下

- 匹配单个文件：
  `gulp.src('src/js/index.js')`

- 匹配多个文件：
  `gulp.src(['src/js/index.js','src/js/detail.js']) //多个文件以数组形式传入`

- 匹配所有文件
  `gulp.src('src/js/*.js')`

- 匹配符：
  `!`：排除文件，

  ```
  gulp.src(["./src/sass/**/*.scss","!./src/sass/var.scss"])
  
  ```

  `*`：匹配所有文件，
  `**`：匹配0个或多个子文件夹，
  `{}`：匹配多个属性

备注：若想实现某个文件不受匹配控制，在文件名前面加_

# Sass

SASS是一个成熟、稳定、强大的 CSS 扩展语言解析器，提供变量、嵌套、混合、继承等特性，大大节省了设计者的时间，使得CSS的开发变得简单和可维护 .

###### 了解工具：css转scss

### 嵌套(Nesting)

css中重复写选择器是非常恼人的。如果要写一大串指向页面中同一块的样式时，需要一遍又一遍地写同一个ID。

```
#content article h1 { color: #333 }
#content article p { margin-bottom: 1.4em }
#content aside { background-color: #EEE }

```

sass写法：

```
#content {
  article {
    h1 { color: #333 }
    p { margin-bottom: 1.4em }
  }
  aside { background-color: #EEE }
}

```

- 在嵌套中用&表示父元素选择器

### 注释

```
body {
  color: #333; // 单行注释：不会出现在生成的css文件中
  padding: 0; /* 多行注释：内容会出现在生成的css文件中 */
}

```

### 变量

sass的变量必须是$开头，后面紧跟变量名，而变量值和变量名之间就需要使用冒号(:)分隔开（就像CSS属性设置一样）。

###### 演示：变量写法

```
// 主颜色
$mainColor:#5b8c58;
// 高亮颜色
$highlight:#fc0;
// 内边距
$padding:5px 10px;
//使用变量
a:hover{color:$mainColor;}

```

##### 全局变量与局部变量

定义在任何选择器之外的变量被认为是全局变量，定义在选择器内的变量称之为局部变量。

但启用了global后，即使写在局部也能覆盖全局变量（sass 3.4版本后可用）

```
$color:#fff !global;

```

##### 默认变量

sass的默认变量仅需要在值后面加上!default即可。

```
$fontSize:12 !default;

```

##### 变量特殊用法

一般我们定义的变量都为属性值，可直接使用，但是如果变量作为属性或在某些特殊情况下等则必须要以#{$variables}形式使用

```
$direction:top !default;
//应用于class和属性
.border-#{$direction}{
  border-#{$direction}:1px solid #ccc;
}

```

##### 多值变量

多值变量分为list类型和map类型，简单来说list类型有点像js中的数组，而map类型有点像js中的对象。

```
//list类型
$pd: 5px 10px 20px 30px;
//使用
.content{padding:$pd;}
.btop{border-top:nth($pd,1);}

//map类型
$headings: (h1: 2em, h2: 1.5em, h3: 1.2em);
//使用
h1{map-get($headings,h1)}

```

### 运算

sass具有运算的特性，可以对数值型的Value(如：数字、颜色、变量等)进行加减乘除四则运算。请注意运算符前后请留一个空格，不然会出错。 

### 条件判断及循环

##### @if判断

@if可一个条件单独使用，也可以和@else结合多条件使用

```
@if $type == ocean {
    color: blue;
} @else if $type == matador {
    color: red;
} @else {
    color: black;
}

```

##### @for循环

```
@for $var from <start> through <end>（包含end值）
@for $var from <start> to <end>（不包含end值）

```

###### 演示:for循环

```
@for $i from 1 through 6{
	h#{$i}{
		font-size:36px/($i/2);
	}
}

```

### 函数

Sass中的数字函数提要针对数字方面提供一系列的函数功能：

##### 常用函数：

> percentage($value)：将一个不带单位的数转换成百分比值；
> round($value)：将数值四舍五入，转换成一个最接近的整数；
> ceil($value)：将大于自己的小数转换成下一位整数；
> floor($value)：将一个数去除他的小数部分；
> abs($value)：返回一个数的绝对值；
> min($numbers…)：找出几个数值之间的最小值；
> max($numbers…)：找出几个数值之间的最大值。
> lighten($color,$num) $color颜色值，$num:0-100
> darken($color,$num) $num:0-100

```
演示：函数的使用
background-color:lighter($mainColor,percentage($i/10))

```

##### 自定义函数

格式：@fuction 函数名

```
$oneWidth: 10px;  
$twoWidth: 40px;  
@function widthFn($n) {  
  @return $n * $twoWidth + ($n - 1) * $oneWidth;  
}  
.leng {   
    width: widthFn($n : 5);  //！！传参格式注意
} 

```

### 继承

使用选择器的继承，要使用关键词@extend

- 继承一般样式
  @extend h1
- 占位选择器%

```
// % 无实际样式，不会被编译出来
%pop{
	width:600px;height:300px;position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);
}
.box{
	width:800px;
	color:#ccc;
	background-color:#000;
}
.container{
	@extend .box;
	margin:10px;
}
.login{
	@extend %pop;
	background-color:$mainColor*2;
}

```

### 导入 @import

sass中导入其他sass文件，最后编译为一个css文件，优于纯css的@import

```
@import 'reset';

```

###### 演示：同时编译多个scss文件为css，演示_文件名不会编译效果。演示bootstrap源码

```
//var.scss:
$mainColor: #58bc58;
$container: 800px;
$padding:5px 10px 15px 20px;
//list.scss:
.box{
	width:$container;
	color:$mainColor;
	padding:$padding;
	background-color:#fff;
	border:1px soild $mainColor;
}

```

# gulp插件的使用

### js压缩及合并、重命名

```
// js压缩
let uglify = require('gulp-uglify');
let pump = require('pump');
let concat = require('gulp-concat');
let rename = require('gulp-rename');
gulp.task('compressJs',function(cb){
    pump([
        gulp.src('./src/js/*.js'),
        // 合并
        concat('index.js'),
        gulp.dest('./dist/js/'),
        // 压缩
        uglify(),
        // 重命名
        rename({
            suffix:'.min'
        }),
        gulp.dest('dist/js/')
    ],cb );
});    

```

### browser-sync

```
// 静态服务器
gulp.task('server',()=>{
	browserSync({
		// 服务器路径
		// server:'./src/',
		// 代理服务器
		proxy:'http://localhost:1806',
		// 端口
		port:666,
		// 监听文件修改，自动刷新
		files:['./src/**/*.html','./src/css/*.css','./src/api/*.php']
	});
	// 监听sass文件修改，并自动编译
	gulp.watch('./src/sass/*.scss',['compileSass'])	
}）
//监听的文件修改，页面html对应修改。

```

静态服务器：开启服务，不能识别后端语言

wampserver:php解析器

# Sass

定义：SASS是一个成熟、稳定、强大的 CSS 扩展语言解析器，提供变量、嵌套、混合、继承等特性，大大节省了设计者的时间，使得CSS的开发变得简单和可维护 

## 一、语法

#### 1.注释

sass有两种注释方式（与js相同）

- 多行注释/* */
- 单行注释//

```
body {
  color: #333; // 这种注释内容不会出现在生成的css文件中
  padding: 0; /* 这种注释内容会出现在生成的css文件中 */
}

```

#### 2.变量

sass的变量必须是$开头，后面紧跟变量名，而变量值和变量名之间就需要使用冒号(:)分隔开（就像CSS属性设置一样）。

- 全局变量与局部变量
  定义在任何选择器之外的变量被认为是全局变量，定义在选择器内的变量称之为局部变量。

  但启用了global后，即使写在局部也能覆盖全局变量（sass 3.4版本后可用）

  ```
  $color:#fff !global;
  
  ```

- 默认变量：sass的默认变量仅需要在值后面加上!default即可。

```
    $fontSize:12 !default;

```

覆盖的方式也很简单，只需要在默认变量之前重新声明下变量即可（一般用于文件引用）：

```
    $fontSize:16;
    $fontSize:12 !default;//此行代码是另一个文件中的代码（查看@import）

```

变量特殊用法，一般我们定义的变量都为属性值，可直接使用，但是如果变量作为属性或在某些特殊情况下等则必须要以#{$variables}形式使用

```
    $borderDirection:top !default;
    //应用于class和属性
    .border-#{$borderDirection}{
      border-#{$borderDirection}:1px solid #ccc;
    }

```

多值变量，多值变量分为list类型和map类型，简单来说list类型有点像js中的数组，而map类型有点像js中的对象。

```
//list类型
$pd: 5px 10px 20px 30px;

//使用
.content{padding:$pd;}
.btop{border-top:nth($pd,1);}


//map类型
$headings: (h1: 2em, h2: 1.5em, h3: 1.2em);

//使用
h1{map-get($headings,h1)}

```

#### 3.嵌套(Nesting)

css中重复写选择器是非常恼人的。如果要写一大串指向页面中同一块的样式时，往往需要 一遍又一遍地写同一个ID

```
    #content article h1 { color: #333 }
    #content article p { margin-bottom: 1.4em }
    #content aside { background-color: #EEE }

```

sass写法：

```
    #content {
      article {
        h1 { color: #333 }
        p { margin-bottom: 1.4em }
      }
      aside { background-color: #EEE }
    }

```

- 在嵌套中用&表示父元素选择器

#### 5.混合器(了解)

变量可以实现简单样式的重用（如color,width等），但是当你的样式变得越来越复杂，你需要大段大段的重用样式的代码，可以通过sass的混合器实现重用

sass中使用`@mixin`声明混合，通过@include来调用

- 无参数mixin
- 有参数mixin：参数名以$符号开始
- 多个参数mixin：多个参数以逗号分开
- @content：多用于媒体查询的封装

```
    @mixin max-screen($res){
      @media only screen and ( max-width: $res )
      {
        @content;
      }
    }
    @include max-screen(480px) {
      body { color: red }
    }

```

> PS：@mixin通过@include调用后解析出来的样式是以拷贝形式存在的，而下面的继承则是以联合声明的方式存在的，所以从3.2.0版本以后，建议传递参数的用@mixin，而非传递参数类的使用下面的继承%。

#### 6.继承

使用选择器的继承，要使用关键词@extend

- 继承一般样式
  @extend h1
- 占位选择器%

```
//占位符编译后不存在css样式中
    %ir{
      color: transparent;
      text-shadow: none;
      background-color: transparent;
      border: 0;
    }
    @extend %ir;

```

#### 7.函数

定义：Sass中的数字函数提要针对数字方面提供一系列的函数功能：

- 常用函数：

  - percentage($value)：将一个不带单位的数转换成百分比值；

  - round($value)：将数值四舍五入，转换成一个最接近的整数；

  - ceil($value)：将大于自己的小数转换成下一位整数；

  - floor($value)：将一个数去除他的小数部分；

  - abs($value)：返回一个数的绝对值；

  - min($numbers…)：找出几个数值之间的最小值；

  - max($numbers…)：找出几个数值之间的最大值。

  - lighten($color,$percent) $color颜色值，$percent百分比

  - darken($color,$num) $num:0-100

  - 自定义函数

    - 格式：@fuction 函数名      

      $oneWidth: 10px;  

        $twoWidth: 40px;

    @function widthFn($n) {  
      @return $n * $twoWidth + ($n - 1) * $oneWidth;  
    }  

    .leng {   
        width: widthFn($n : 5);  
    } 

#### 8.运算

定义：sass具有运算的特性，可以对数值型的Value(如：数字、颜色、变量等)进行加减乘除四则运算。请注意运算符前后请留一个空格，不然会出错。

- 条件判断及循环

  - @if判断
    @if可一个条件单独使用，也可以和@else结合多条件使用

- - ```
    @if $type == ocean {
        color: blue;
    } @else if $type == matador {
        color: red;
    } @else {
        color: black;
    }
    
    ```

    

  - for循环

    ```
        @for $var from <start> through <end>（包含end值）
        @for $var from <start> to <end>（不包含en值）
    
    ```

    

- 导入
  sass中导入其他sass文件，最后编译为一个css文件，优于纯css的@import

  ```
  @import 'reset';
  
  ```

## 二、编译

- gulp-sass
  - 参数outputStyle：
    - nested(默认）
    - expanded：展开
    - compact：单行
    - compressed：压缩

```
gulp.task('sass', function () {
        return gulp.src('./sass/**/*.scss')
        .pipe(sass({outputStyle: 'compressed'}).on('error', sass.logError))
        .pipe(gulp.dest('./css'));
    });

    //文件监听（文件有修改自动编译）
    gulp.task('sassWatch',function(){
        gulp.watch('./src/sass/*.scss',['sass']);
    });

```

> 文件名以_开头的sass文件不会被编译成css文件

# Git

定义：Git是一个开源的分布式版本控制系统，可以有效、高速的处理从很小到非常大的项目版本管理 !

## 一、安装与配置

- 下载与安装
  下载地址：<https://git-for-windows.github.io>

- 配置个人信息（名字与邮箱）
  使用Git的第一件事就是设置你的名字和email,这些就是你在提交commit时的签名

  ```
  git config --global user.name "Your Name"
  git config --global user.email "email@example.com"
  
  ```

  

  > 查看是否配置成功，用命名git config

## 二、git的使用（命令行）

### （一）创建本地仓库

- git init：把当前目录变成一个git仓库，并自动创建master分支

> 以上命令会在当前目录下创建了一个.git 隐藏目录，它就是所谓的Git 仓库。生成仓库后的目录就不是普通的文档目录了，我们将其称为工作区，所以工作区中都包含一个git仓库，而一个git仓库中又包含一个暂存区和一个版本库

### （二）工作区与版本库概念

Git有三大区：工作区、暂存区、版本库（如上图 ）

- 工作区（Working Directory）：电脑中的目录
- 仓库：工作区有一个隐藏目录.git，这个不算工作区，而是Git仓库。
  - 暂存区（stage/index）：一个临时的存储区域
  - 版本库 （Repository）![git的三大区](E:\H5每天\二阶段18.8.13\30.9.29\33.git\git的三大区.png)

### （三）添加文件到版本库的步骤（重点）

1. 创建（修改）文件
   往工作区中添加/修改文件
2. 添加到暂存区：`git add <file>`
   把修改存放到暂存区

- git add 文件夹：把文件夹下的所有修改添加到暂存区
- git add .：添加所有修改到暂存区
- 如果想过滤部分文件，请查看 过滤清单

1. 提交到版本库：

```
git commit -m "备注"

```

使用git commit 命令可将暂存区的内容提交至版本库中，这个过程称为提交，每一次提交都意味着版本在进行一次更新（会自动生成一个commit id）

> PS：如果不写-m回车会进入vim编辑界面，退出方法：

- 进入编辑状态：i
- 退出编辑状态：ESC
- 同时按下Shift和冒号（:），接着输入输入：q（退出不保存），wq（保存并退出）

### （四）其他辅助命令

- 查看仓库变更状态：`git status`
  用status查看仓库会有几种状态：untracked、unstaged、uncommitted 

## 三、git远程仓库

### （—）注册登录

- github(国外):<https://github.com/>
- coding(国内):<https://coding.net>

### (二)关联本地仓库与远程仓库

> 有两种方式关联：ssh和https两种协议，https比较简单，但提交时每次都分输入用户名和密码，如使用https协议，直接跳过以下第1、第2步

1. 创建SSH Key：`ssh-keygen -t rsa -C 'email地址'`
   以上命令会在当前window用户的目录里创建.ssh目录，里面有id_rsa（私钥）和id_rsa.pub（公钥）两个文件

   将公钥写到github的ssh keys 上

2. 添加SSH Key到Git服务器 
   添加完成后测试线路是否连通：`ssh -T git@github.com`

3. 建立本地仓库与远程仓库的连接

   **方式1：适用于先有本地仓库，后有远程仓库的情况
   格式：`git remote add 远程仓库名 远程仓库地址`

```
git remote add origin git@github.com:xxx/view.git

```

> 测试是否成功`git remote -v`
>
> PS：删除远程仓库连接：`git remote remove 远程仓库名`

​	**方式2：克隆（适用于先有远程库，后有本地仓库的情况）

格式：

```
git clone 远程仓库地址

```

> 当你从远程仓库克隆时，实际上Git自动把本地的master分支和远程的master分支对应起来了，并且，远程仓库的默认名称是origin

### （三）推送到远程仓库（重点）

- git push

 格式：`git push 远程仓库名 本地分支名:远程分支名`

把本地分支内容推送到远程分支（远程分支名省略表示推送到与本地分支相同的分支 

```
git push origin master

```

### （四）拉取与合并（重点）

同步本地与远程仓库

- git pull

格式：`git pull 远程仓库名 远程分支名:本地分支名`
拉取远程分支内容到本地并与本地分支进行合并（本地分支名省略表示合并到与远程分支名相同的分支）

```
git pull origin master

git pull origin master --allow-unrelated-histories

```

- git fetch

拉取远程分支内容

- git merge

合并分支内容

```
git pull origin master

//以上命令相当与以下命令等效
git fetch origin master
git merge origin/master

```

> **push和pull后的分支顺序格式：<来源地>:<目的地>
>
> 模拟解决冲突问题

## 四、版本回退

#### 1.回退命令：git reset

- 回退到上一个版本
- git reset --hard HEAD^
- 回退到指定版本：
- git reset --hard [commit id] 版本号没必要写全，前几位就可以了，Git会自动去找。
- 回退指定文件
- git reset --hard [commit id] <file>
- 参数说明
  - –hard:工作区、暂存区、版本库的文件同时回退
  - –mixed：暂存区、版本库的文件回退（默认）
  - –soft：仅仅回退版本库中的文件

#### 2.当前版本：HEAD

 上一个版本：HEAD^ 上上个版本：HEAD^^ … 依此类推 前100个版本：HEAD~100 

#### 3.显示从最近到最远的提交日志：`git log`

- –pretty=oneline（显示简要信息id+备注）
- –graph（图形显示版本走向）
- –abbrev-commit（显示简写的id）
- 一大串类似3628164…882e1e0的是commit id（版本号）
- 查看命令历史：`git reflog`
- 撤销文件修改
  - `git checkout -- <file>`：放弃工作区的修改
  - `git rm --cache <file>`：撤销暂存区的修改
  - `git reset HEAD <file>`：撤销暂存区的修改
- 对比文件：`git diff <file>`

## 五、git过滤配置(过滤清单)

一般来说每个Git项目中都需要一个“.gitignore”文件，这个文件的作用就是告诉Git哪些文件不需要添加到版本管理中。

```
#过滤node_modules根目录下的文件（不过滤其他目录下的node_modules文件夹）
/node_modules

#过滤所有mtk文件夹
mtk/ 

#过滤所有.zip文件
*.zip 
*.mp3
*.mp4

#过滤某个具体文件
/mtk/do.c 

```

- `#为注释`
- 很简单吧，被过滤掉的文件就不会出现在你的GitHub库中了，当然本地库中还有，只是push的时候不会上传。
- 演示sass遗留的依赖包问题：npm init创建package.js，npm install根据package.js下载包

## 六、分支操作（了解）

- 创建分支：`git branch 分支名`

- 切换分支：`git checkout 分支名`

  > 以上两步合并为：`git checkout -b 分支名`

- 查看分支：git branch
  列出所有分支，当前分支前面会标一个*号

- 合并分支：git merge 分支名

  - git merge dev：把dev分支合并到当前分支
  - Fast-forward：快速合并
    - 禁用快速合并： –no-ff （保持分支信息）
    - 合并要创建一个新的commit，所以加上-m参数，把commit描述写进去

- 删除分支：`git branch -d 分支名`
  强行删除，需要使用命令`git branch -D feature-vulcan`

- 获取远程分支

1. 先获取（git fetch）
2. 然后在本地创建一个同名分支,并将远程分支映射到此分支（git branch dev origin/dev）

**加：在实际开发中，我们应该按照几个基本原则进行分支管理：**
首先，master分支应该是非常稳定的，也就是仅用来发布新版本，平时不能在上面干活；

那在哪干活呢？干活都在dev分支上，也就是说，dev分支是不稳定的，到某个时候，比如1.0版本发布时，再把dev分支合并到master上，在master分支发布1.0版本；

你和你的小伙伴们每个人都在dev分支上干活，每个人都有自己的分支，时不时地往dev分支上合并就可以了。

所以，团队合作的分支看起来就像这样：

http://www.ruanyifeng.com/blog/2011/05/how_to_choose_free_software_licenses.html 

# 三阶段 第一天10.15

# Node

**介绍**：Node.js®是基于[Chrome的V8 JavaScript引擎](https://developers.google.com/v8/)构建的JavaScript运行时。 

**解释**：就好比谷歌的控制台，可以单独的运行js代码

## 一、使用Node的条件

- 安装[node](https://nodejs.org/zh-cn/)环境
- `npm install gulp`
- 写一份**gulpfile.js**配置gulp的参数
- gulp命令执行js来完成代码处理（压缩，重命名）

## 二、install

如果没有安装的node环境去[node官网](https://nodejs.org/zh-cn/)安装维护版本

查看版本号，在cmd中执行，

```bash
node -v
```

## 三、introduce

### （一）前端（浏览器端）

> 要运行JS，必须借助于HTML文件，没有HTML文件和浏览器环境，那JS是无法运行     （要有HTML文件，也要有浏览器环境）
> 浏览器=界面+控制台
> JS是必须运行在浏览器上，所以只能控制浏览器

### （二）后端（服务器端）

> 要运行JS，（既不需要HTML文件，也不需要浏览器环境，只需要Node环境），node替代了HTML文件，也替代了浏览器
> 服务器(node)=控制台
> JS有了node环境，可以运行在非浏览器环境下，因为node是装在系统上，所以JS可以操作系统
> node(浏览器的控制台===chrome的V8引擎)<浏览器

## 四、运行

<u>如何使用node</u>

- 写一份JS代码
- 在命令行定位到此代码的位置，运行命令`node JS文件的名字.js`

## 五、模块化

### （一）自定义模块化

#### 1. 前端

- 写多条`<script>引入JS`在html分开引入
- 利用`require.js`

```html
<script src="jquery.js"></script>
<script src="cookie.js"></script>
<script src="module.js"></script>
	解释：*就是我们平常正在用的那种script里面的src引入
		 *利用require.js引入，二阶段讲的那种	
```

#### 2. node（后端）

- 它没有html，所以需要借助于两个js方法
- 导出，借助于`module.exports`

```js
function plus(a, b) {
	return a + b
}

function sub(a,b){
	return a-b
}

module.exports = {
	plus,
	sub
}
```

- 导入,借助于`require`,建议用相对路径

```js
var tool = require("./plus.js");
	*解释：就是相当于你要用jquery封装好的方法一样，只不过现在的你没有了HTML和浏览器环境，所以你必须要用这种模块化的方式引入到你要运行的js里面
```

### （二）内置模块

- 不需要自己写，就是node环境自带，它自己写好给你的，引入即可
- Node拿来违PHP的一种替代（多一种可选的方案）
- PHP能做的，Node也能做

```
解释：模块就相当于js中的jquery库一样，你只需要引入之后调用方法即可
```

| 模块       | 名字 |
| ---------- | ---- |
| 读写文件   | fs   |
| 创建服务器 | http |
| 查看系统   | os   |
| 压缩文件   | zip  |
| ...        | ...  |

其他模块参考 [node官网内置模块API文档](https://nodejs.org/dist/latest-v8.x/docs/api/)

### （三）HTTP

- HTTP超文本传输协议
- 前端最多就是ajax（http协议的一种前端实现方案）GET/POST

| GET          | POST         |
| ------------ | ------------ |
| 参数在url上  | 参数在请求体 |
| 有可能有长度 | 没长度限制   |
| 不安全       | 安全         |

| 状态码 |                     |
| ------ | ------------------- |
| 1xx    | 开始执行            |
| 2xx    | 成功                |
| 3xx    | 重定向              |
| 4xx    | 客户端错误,浏览器端 |
| 5xx    | 服务端              |

**apache(wamp集成环境)+php**

```
window
apache
mysql
php
```

### （四）创建服务器

```js
var http = require('http');
console.log(http);
var server = http.createServer(Function(request,response){
	response.end("hello world");
})
server.listen(12345);//(0,65535)
console.log("启动服务器");
```

出现跨域，加一个头部来解决

```php
header("Access-Control-Allow-Origin:*")
```

# 第三方模块

# 第二天 10.16

## 一、参考教程

[runoob菜鸟教程](https://www.runoob.com/nodejs/nodejs-tutorial.html)

## 二、异步

### （一）前端（浏览器端）

**前端异步只有以下几种情况**

```
ajax xmlhttprequest 	//ajax请求
setInterval/setTimeout	//定时器
jsonp				  //json	JSONP的原理是通过script标签发起一个GET请求来取代XHR请求。
```

### （二）后端（服务器端node）

**比前端多很多，很多方法都是异步的**

```
fs.readFile 	//异步
fs.readFileSync //同步
```

**解释：**

- 异步一般是配合回调函数，回调函数能让异步变得有意义
- 同步比异步少了回调函数
- 同步阻塞，相对稳定，不需要回调
- 异步非阻塞，相对不稳定，配合回调才有意义



```js
//同步
var data = fs.readFileSync('./test.txt');
console.log(data.toString());

//异步
fs.readFile('./test.txt',function(err,data2){
	console.log(data2.toString());
});
```

## 三、回调嵌套

**如果出现多个回调嵌套的时候，建议用`promise`去解决这个回调地域**

```js
function buyPizza() {
	return new Promise((resolve, reject) => {
		setTimeout(() => {
			console.log("买披萨");
			resolve()
		}, 1000);
	})
}
function buyDrink() {
	return new Promise((resolve, reject) => {
		setTimeout(() => {
			console.log("买饮料");
			resolve()
		}, 1000);
	})
}
function eatMeal() {
	return new Promise((resolve, reject) => {
		setTimeout(() => {
			console.log("吃东西");
			//resolve()
		}, 1000);
	})
}
buyPizza().then(buyDrink).then(eatMeal);
```

## 四、request

**任何前端请求都有**

- 请求头（浏览器信息），请求体（POST请求，请求参数会放在这个地方）用户不可见的
- 响应头（服务器信息），响应体（页面的内容，用户可见）
- [request模块文档](https://www.npmjs.com/package/request)

### （一）爬虫

爬取网站的内容，然后可以保存到本地，或者分析页面获取有价值的信息

```js
var request = require('request');
var fs = require('fs');
request('http://www.umei.cc/', function(error, response, body) {
	//console.log('error:', error); // Print the error if one occurred
	//console.log('statusCode:', response && response.statusCode); // Print the response status code if a response was received
	console.log('body:', body); // Print the HTML for the Google homepage.
//	fs.writeFile('test.html', body, function(err) {
//		console.log("成功保存")
//	})
});
console.log("开始请求");
```

### （二）cheerio

- [cheerio使用文档](https://www.npmjs.com/package/cheerio)

实现网页内容分析，用法类似于jQuery，node版本jQuery,可以用它爬取文字，图片，音频

```js
var request = require('request');
var cheerio = require('cheerio');
request('http://www.umei.cc/', function(error, response, body) {
	//console.log('body:', body); // Print the HTML for the Google homepage.
	const $ = cheerio.load(body);
	$("img").each((i,e)=>{
		console.log($(e).attr("src"))
	})
});

console.log("开始请求");
```

**并非所有网站都是能爬，有些网站是防爬虫，还有一些网页是前端JS动态生成**

> 解释：* 爬虫的意义就是：利用request链接到网站，爬取它的内容；
>
> ​	    * 然后在请求出来的内容中用cheerio筛选出你要的有用的信息

# 10.17 express

- [npm的express文档](https://www.npmjs.com/package/express)

定义：切换不同的路由就进入不同的逻辑，也就是浏览器输入不同路径，页面就有不同的返回效果

```js
var express = require('express')
var app = express()
 
app.get('/', function (req, res) {
  res.send('Hello World')
})

app.get('/home', function (req, res) {
  res.send('home页面')
})
 
app.listen(3000)

解释：就是当你app后面的括号里面斜杠“/”后是不同的东西的时候，就是不同的页面，就好像是不同的PHP页面一样，有不同的功能（index.php,login.php ....）
```

## 一、express的脚手架

#### 1.先安装 express

```
npm install express

在安装这个express之前要先npm init一份package.json文件
```

#### 2 .全局安装

```bash
npm install -g express-generator@4
```

#### 3. 在一个文件夹里面用`express`命令创建应用架构

```bash
express test
cd test
```

#### 4. 进入test文件夹安装依赖，推荐cnpm安装所有依赖

```bash
npm install
```

#### 5. 启动应用

```bash
SET DEBUG=test:*	//这句是必须要加的，否则会出错
npm start
```

#### 6. 访问在浏览器3000端口号

```bash
http://localhost:3000
```

## 二、创建路由

定义：

- 进入到test的routes文件夹，然后复制`users.js`
- 你可以改变`/home`这里的路径

```bash
var express = require('express');
var router = express.Router();
router.get('/home', function(req, res, next) {
  res.send('hello world');
});
module.exports = router;
```

- 在`app.js`添加以下两条，该路由就完成了

```js
var homeRouter = require('./routes/home');	//7,8行后面加
//code
app.use('/test', homeRouter);			  //25,26行后面加

解释：* 上面蓝色的字，必须和下面逗号后的字一样
	 * 下面的test为虚拟路径，你加上它之后，访问的时候就要 
			http://localhost:3000/test/home
注意：* 访问这种路由的时候，跟你放在哪个文件夹没有关系，只跟你的虚拟目录有关系
	 * post请求的页面时看不到的
```

- 访问该路径

```js
http://localhost:3000/test/home
```

## 三、mysql

#### 1. 连接数据库

- 要用mysql一样要下第三方模块

```
npm install mysql
```

```
var mysql = require('mysql');
var connection = mysql.createConnection({
	host: 'localhost',
	user: 'lemon',
	password: '123456',
	database: '1806'
});
connection.query('INSERT INTO students SET ?', [{
	username: req.body.username,
	password: req.body.password
}], function(error, results, fields) {
	if(error) throw error;
	res.send("success");
});
connection.end();


//select * from students where username = 
```

#### 2. 对mysql的封装函数

```
//db.js文件下

    var mysql = require('mysql');
    var config = require("./config.js")

    function query(sql, params, callback) {
        var connection = mysql.createConnection({
            host: config.host,
            user: config.user,
            password: config.password,
            database: config.database
        });
        connection.connect();
        connection.query(sql, params, function(error, results, fields) {
            if(error) throw error;
            callback(results);
            connection.end();
        });
    }

    module.exports = {
        query: query
    }
```

```
//config.js 文件夹下

    module.exports = {
        host: 'localhost',
        user: 'lemon',
        password: '123456',
        database: '1806'
    }
```

**用法**

```
var db = require("./db.js");
console.log(db)
db.query("SELECT * FROM students where ?",[{
	username:'qq'
}],function(data){
	console.log(data)
})

=====================================================================

var db = require("./db.js");
console.log(db)
db.query("SELECT * FROM students",[],function(data){
	console.log(data)
})
```

#### 3. 注册案例

```
var express = require('express');
var router = express.Router();

/* GET users listing. */
router.get('/live', function(req, res, next) {
	res.send('你已经进入直播间了');
});

router.post('/login', function(req, res, next) {
	console.log(req.body)
	if(req.body.username === 'ly' && req.body.password === '123') {
		res.send('success');
	} else {
		res.send('fail');
	}
});

router.post('/register', function(req, res, next) {
	console.log(req.body)
	var mysql = require('mysql');
	var connection = mysql.createConnection({
		host: 'localhost',
		user: 'lemon',
		password: '123456',
		database: '1806'
	});

	connection.connect();

	function isExistSameName() {
		return new Promise(function(resolve, reject) {
			connection.query('select * from students where ?', [{
				username: req.body.username,
			}], function(error, results, fields) {
				console.log(results)
				if(error) throw error;
				if(results.length > 0) {
					connection.end();
					res.send("fail")
				}else{
					resolve()
				}
			});
		})
	}

	function isInsertUser() {
		return new Promise(function(resolve, reject) {
			console.log(req.body.username,req.body.password)
			connection.query('INSERT INTO students SET ?', [{
				username: req.body.username,
				password: req.body.password
			}], function(error, results, fields) {
				if(error) throw error;
				res.send("success");
				connection.end();
			});
		})
	}
	isExistSameName().then(isInsertUser)

});

module.exports = router;
```

#### 4. 登录案例

```
var express = require('express');
var router = express.Router();
var mysql  = require('mysql');
var app = express();
var arr = [];
/* GET users listing. */
router.get('/', function(req, res, next) {
  res.send('respond with a resource');
});
================注册==================
router.post('/login', function(req, res, next) {
    // console.log(req.body);
    
    var connection = mysql.createConnection({
      host     : 'localhost',
      user     : 'root',
      password : '',
      database : 'lianxi'
    });
    connection.query('INSERT INTO login SET ?', [{
    username: req.body.username,
    password: req.body.password
    }], function(error, results, fields) {
    if(error) throw error;
    res.send("success");
    });
  // res.send('respond with a resource');
});
==================登录======================
router.post('/denglu', function(req, res, next) {
    // console.log(req.body);
    
    var connection = mysql.createConnection({
      host     : 'localhost',
      user     : 'root',
      password : '',
      database : 'lianxi'
    });
    
    connection.query('select * from login where ?', [{
        username: req.body.username,
      }],function(error, results, fields) {
        if(results.length <=0){
           connection.end();
           res.send("fail");
        }
        if(results.length>0){
            if(req.body.password == results[0].password){
              connection.end();
              res.send("success");
            }else{
              connection.end();
              res.send("fail");
            }
        }
      })
                
});

module.exports = router;


```

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title></title>
    </head>
    <body>
        <script src="../javascripts/jquery-3.2.1.js"></script>
        <input type="text" id="username" />
        <input type="password" id="password" />
        <button id="login">登录</button>
        <script>
            $("#login").click(function(){
                $.ajax({
                    type:"post",
                    data:{
                        username:$("#username").val(),
                        password:$("#password").val()
                    },
                    url:"http://localhost:3000/users/denglu",
                    async:true,
                    success:function(data){
                        console.log(data);
                    }
                });
            })
        </script>
    </body>
</html>


```

**备注：你在前端链接的路径，也是虚拟路径**

```
  url:"http://localhost:3000/users/denglu",
  
  下面app.js里面有多少个东西，上面就有多少个js文件

```

# 10.18 express

## 一、multer

**参考文档**

- [multer模块](https://github.com/Wscats/node-tutorial/tree/master/uploadFiles)
- [multer npm官方文档](https://www.npmjs.com/package/multer)

### （一）上传单文件项目

#### 1. 安装`multer`模块

```
npm install multer --save-dev

```

#### 2.配置参数

```js
// 上传配置的必须的参数
var multer = require('multer');
var storage = multer.diskStorage({
	//设置上传后文件路径，uploads文件夹会自动创建。
	destination: function(req, file, cb) {
		cb(null, './uploads')	//文件路径
	},
	//给上传文件重命名，获取添加后缀名
	filename: function(req, file, cb) {
		var fileFormat = (file.originalname).split(".");
		//给图片加上时间戳格式防止重名名
		//比如把 abc.jpg图片切割为数组[abc,jpg],然后用数组长度-1来获取后缀名
		cb(null, file.fieldname + '-' + Date.now() + "." + fileFormat[fileFormat.length - 1]);
	}
});
var upload = multer({
	storage: storage
});
```

#### 3.写入文件案例

[参考链接老姚的](https://github.com/Wscats/node-tutorial/blob/master/uploadFiles/%E5%A4%9A%E5%9B%BE%E4%B8%8A%E4%BC%A0/express.js)

```
============uploads.html=============

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Document</title>
    <script type="text/javascript" src="javascripts/jquery-3.2.1.js"></script>

</head>
<body>
<form id="uform">
    <input type="file" id="file" name="avatar"  multiple/>
</form>
        <script type="text/javascript">
        $fileNode = $("#file");
        $fileNode.on("change",function(){
             var data = new FormData();
        
             $($fileNode[0].files).each(function(idx,item){
                data.append("avatar",item);
                
             })
            
            $.ajax({
                type:"post",
                data:data,
                // new FormData($("#uform")[0]),
                url:"http://localhost:3000/tesy/uploads",
                processData: false,
                contentType: false,
                async:true,
                success:function(data){
                    console.log(data)
                }
            });
        })

    </script>
</body>
</html>

======================file.js=====================

var express = require('express');
var router = express.Router();
// var db = require('../lib/db.js');

var multer = require('multer');

var storage = multer.diskStorage({
    //设置上传后文件路径，uploads文件夹会自动创建。
    destination: function (req, file, cb) {
        //console.log(file)
        cb(null, 'public/page') //上传文件夹
    },
    //给上传文件重命名，获取添加后缀名
    filename: function (req, file, cb) {
        var fileFormat = (file.originalname).split(".");
        //给图片加上时间戳格式防止重名名
        //比如把 abc.jpg图片切割为数组[abc,jpg],然后用数组长度-1来获取后缀名
        cb(null, file.fieldname + '-' + Date.now() + "." + fileFormat[fileFormat.length - 1]);
    }
});
var upload = multer({
    storage: storage
});


/* GET users listing. */
router.get('/', function (req, res, next) {
    res.send('respond with a resource');
});

router.post('/uploads', upload.any(), function (req, res, next) {
    console.log(res);
    next();
}, function (req, res, next) {
    res.send("upload success");
});

module.exports = router;

```

## 二、mongodb

定义：nosql数据库，不需要sql语句的数据库，里面一切都是类似于JSON文件

- [mongodb教程](https://github.com/Wscats/node-tutorial/issues/20)

### （一）安装

- 双击安装`mongodb.msi`文件
- 找回安装完`mongodb`文件夹`bin`的路径

```
C:\Program Files\MongoDB\Server\3.2\bin

```

**里面有多个exe文件**

- 在`bin`该目录下，打开`cmd`命令行，执行以下命令，该目录有数据连接此数据库，该目录没库就是创建数据库成功，

```bash
mongod --dbpath [文件夹的路径]
	解释：文件夹路径随便写，你想把数据库建在哪，就写哪
```

![1539951778729](C:\Users\WANG\AppData\Local\Temp\1539951778729.png)

- 安装`robo3t`的可视化软件来管理`mongodb`数据库，没有表的概念，只有集合(类似于mysql的表))
- 配合node来使用`mongodb`数据库,在项目目录下用cmd安装

```bash
npm install mongodb
```

- 新建`server.js`,执行以下代码

```
const MongoClient = require('mongodb').MongoClient;
const assert = require('assert');
 
// Connection URL
const url = 'mongodb://localhost:27017';
 
// Database Name
const dbName = '1806';
 
// Use connect method to connect to the server
MongoClient.connect(url, function(err, client) {
  assert.equal(null, err);
  console.log("Connected successfully to server");
  const db = client.db(dbName);
  client.close();
});

```

==================================GitHub===========================

# 安装配置

在`Mongodb`官网下载最新版本的[Mongodb下载地址](https://cloud.mongodb.com/)

下载`msi`的`window`安装包，可以装到C盘或者D盘目录下

# 配置

由于我是安装在D盘的环境下

```
D:\Program Files (x86)\MongoDB\Server\3.2\bin

```

所以在bin文件夹下找到mongod.exe命令，然后通过管理员执行`mongod --dbpath x路径x`，路径可以是任何地方，我这里选择在D盘的MongoDB目录下，当然路径不要包含特殊的字符串，比如`Program Files (x86)`也不行

```
mongod --dbpath D:\mongodb\data\db

```

[![image](https://user-images.githubusercontent.com/17243165/31977540-fc0a5a6e-b96f-11e7-9a2b-34d66d7241c4.png)](https://user-images.githubusercontent.com/17243165/31977540-fc0a5a6e-b96f-11e7-9a2b-34d66d7241c4.png)

# 命令行

经过上面的配置之后，就可以返回bin目录下找到`mongo.exe`命令，并管理员下执行，就可以出现mongodb的命令行模式

```
D:\Program Files (x86)\MongoDB\Server\3.2\bin

```

[![image](https://user-images.githubusercontent.com/17243165/31978099-57bce3ca-b972-11e7-88bd-30f5d68036ed.png)](https://user-images.githubusercontent.com/17243165/31978099-57bce3ca-b972-11e7-88bd-30f5d68036ed.png)

然后就可以使用下面的命令来测试了

```
db.help()//帮助
db.stats()//统计

```

# 显示数据库

```
show dbs

```

检查当前选择的数据库

```
db

```

# 添加数据库

**数据库名**为数据库创建的名字，使用该命令后会默认切换到对应的数据库，并且在数据库中添加选项，数据库信息才显示，如果默认就有该数据库，那就是切换到对应的数据库里面

```
use 数据库名

```

# 删除数据库

先切换到对应的数据库，然后再执行`db.dropDatabase()`删除该数据库

```
use 数据库名
//switched to db 数据库名
db.dropDatabase()

```

# 显示集合

用一下命令可以检查创建的集合

```
show collections

```

# 添加集合

在创建完数据库之后，我们就可以创建集合

```
db.createCollection(集合名字name，设置参数options[对象类型])

```

**name**是要创建的集合的名称。 **options**是一个文档，用于指定集合的配置

| 参数    | 类型     | 描述                               |
| ------- | -------- | ---------------------------------- |
| name    | String   | 要创建的集合的名称                 |
| options | Document | (可选)指定有关内存大小和索引的选项 |

**options**参数是可选的，因此只需要指定集合的名称。 以下是可以使用的选项列表：

| 字段        | 类型    | 描述                                                         |
| ----------- | ------- | ------------------------------------------------------------ |
| capped      | Boolean | (可选)如果为true，则启用封闭的集合。上限集合是固定大小的集合，它在达到其最大大小时自动覆盖其最旧的条目。 如果指定true，则还需要指定size参数。 |
| autoIndexId | Boolean | (可选)如果为true，则在_id字段上自动创建索引。默认值为false。 |
| size        | 数字    | (可选)指定上限集合的最大大小(以字节为单位)。 如果capped为true，那么还需要指定此字段的值。 |
| max         | 数字    | (可选)指定上限集合中允许的最大文档数。                       |

由于**option**是可选，我们也可以不带配置项创建集合

```
db.createCollection("mycollection")

```

# 删除集合

`db.collection.drop()`用于从数据库中删除集合

```
db.集合名.drop()

```

比如我们可以测试以下操作

```
db.createCollection("wscats")//创建名为wscats的集合
show collections//显示该数据库所有集合   wscats
db.wscats.drop()//删除名为wscats的集合

```

# 查看文档

最简单查看文档的方法就是`find()`，会检索集合中所有的文档结果

```
db.集合名.find()

```

要以格式化的方式显示结果，可以使用`pretty()`方法。

```
db.集合名.find().pretty()

```

## 1.固值寻找

寻找age集合里面所有含有属性值为wscats的文档结果，相当于`where name = 'wscats'`

```
db.age.find({name:"wscats"})

```

## 2.范值寻找

| 操作     | 语法       | 示例                                        | 等效语句              |
| -------- | ---------- | ------------------------------------------- | --------------------- |
| 相等     | {:}        | `db.age.find({"name":"wscats"}).pretty()`   | where name = 'wscats' |
| 小于     | {:{$lt:}}  | `db.age.find({"likes":{$lt:50}}).pretty()`  | where likes < 50      |
| 小于等于 | {:{$lte:}} | `db.age.find({"likes":{$lte:50}}).pretty()` | where likes <= 50     |
| 大于     | {:{$gt:}}  | `db.age.find({"likes":{$gt:50}}).pretty()`  | where likes > 50      |
| 大于等于 | {:{$gte:}} | `db.age.find({"likes":{$gte:50}}).pretty()` | where likes >= 50     |
| 不等于   | {:{$ne:}}  | `db.age.find({"likes":{$ne:50}}).pretty()`  | where likes != 50     |

## 3.AND和OR寻找

### AND

在find()方法中，如果通过使用`，`将它们分开传递多个键，则mongodb将其视为**AND**条件。 以下是AND的基本语法

寻找`_id`为1并且`name`为wscats的所有结果集

```
db.age.find(
   {
      $and: [
         {"_id": 1}, {"name": "wscats"}
      ]
   }
)

```

### OR

在要根据OR条件查询文档，需要使用`$or`关键字。以下是OR条件的基本语法

寻找`name`为corrine或者`name`为wscats的所有结果集

```
db.age.find(
   {
      $or: [
         {"name": "corrine"}, {“name“: "wscats"}
      ]
   }
)

```

### AND和OR等结合

相当于语句`where title = "wscats" OR ( title = "corrine" AND _id < 5)`

```
db.age.find({
  $or: [{
    "title": "wscats"
  }, {
    $and: [{
      "title": "corrine"
    }, {
      "_id": {
        $lte: 5
      }
    }]
  }]
})

```

# 插入文档

文档的数据结构和JSON基本一样。
所有存储在集合中的数据都是BSON格式。
BSON是一种类json的一种二进制形式的存储格式,简称**Binary JSON**。

要将数据插入到mongodb集合中，需要使用mongodb的`insert()`或`save()`方法。

```
db.集合名.insert(document)

```

比如我们可以插入以下数据

```
db.wscats.insert({
   _id: 100,
   title: 'MongoDB Tutorials', 
   description: 'node_tutorials',
   by: 'Oaoafly',
   url: 'https://github.com/Wscats/node-tutorial',
   tags: ['wscat','MongoDB', 'database', 'NoSQL','node'],
   num: 100,
})

```

也可以支持插入多个，注意传入的是数组形式

```
db.wscats.insert([{
   _id: 100,
   title: ‘Hello’
},{
   _id: 101,
   title: ‘World’
}])

```

在插入的文档中，如果不指定_id参数，那么mongodb会为此文档分配一个唯一的ObjectId
要插入文档，也可以使用`db.post.save(document)`。如果不在文档中指定_id，那么`save()`方法将与`insert()`方法一样自动分配ID的值。如果指定_id，则将以save()方法的形式替换包含**_id**的文档的全部数据。

```
db.wscats.save({
   _id: 111,
   title: 'Oaoafly Wscats', 
})

```

# 更新文档

## 1.update()方法

寻找第一条title为wscats的值，并且更新值title为corrine和age为12

```
db.age.update({
  'title': 'wscats'
}, {
  $set: {
    'title': 'corrine',
    'age': 12
  }
})


```

默认情况下，mongodb只会更新一个文档。要更新多个文档，需要将参数`multi`设置为true，还可以配合find方法里面的各种复杂条件判断来筛选结果，然后更新多个文档

寻找所有title为wscats的值，并且更新值title为corrine和age为12

```
db.age.update({
  'title': 'wscats'
}, {
  $set: {
    'title': 'corrine',
    'age': 12
  }
}, {
  multi: true
})


```

## 2.save()方法

将`_id`主键为3的文档，覆盖新的值，注意`_id`为必传

```
db.age.save({
  '_id':3,
  'title': 'wscats'
})


```

# 删除文档

删除主键`_id`为3的文档，默认是删除多条

```
db.age.remove({
  '_id':3
})


```

建议在执行`remove()`函数前先执行`find()`命令来判断执行的条件是否正确

如果你只想删除第一条找到的记录可以设置**justOne**为1，如下所示

```
db.age.remove({...},1)


```

全部删除

```
db.age.remove({})


```

# Limit与Skip方法

## Limit

如果你需要在mongodb中读取指定数量的数据记录，可以使用mongodb的Limit方法，`limit()`方法接受一个数字参数，该参数指定从mongodb中读取的记录条数。

```
db.age.find().limit(数量)


```

## Skip

我们除了可以使用`limit()`方法来读取指定数量的数据外，还可以使用`skip()`方法来跳过指定数量的数据，skip方法同样接受一个数字参数作为跳过的记录条数。

```
db.age.find().limit(数量).skip(数量)
//skip()方法默认值为0


```

所以我们在实现分页的时候就可以用limit来限制每页多少条数据(一般固定一个值)，用skip来决定显示第几页(一个有规律变动的值)

# 排序

在mongodb中使用使用`sort()`方法对数据进行排序，`sort()`方法可以通过参数指定排序的字段，并使用1和-1来指定排序的方式，其中1为升序排列，而-1是用于降序排列。

| 1    | 升序排列 |
| ---- | -------- |
| -1   | 降序排列 |

```
db.集合名.find().sort({键值(属性值):1})


```

把`age`集合表重新根据`_id`主键进行降序排列

```
db.age.find().sort({
  "_id": -1
})


```

# Node.js连接

安装mongodb的模块

```
npm install mongodb


```

## 1.连接数据库

```
var MongoClient = require('mongodb').MongoClient;
//结尾是选择数据库名
var DB_CONN_STR = 'mongodb://localhost:27017/wscats';
MongoClient.connect(DB_CONN_STR, function(err, db) {
  console.log("连接成功！");
});


```

## 2.查询数据

注意查询回来的结果需要toArray来遍历处理

```
var MongoClient = require('mongodb').MongoClient;
var DB_CONN_STR = 'mongodb://localhost:27017/wscats';

MongoClient.connect(DB_CONN_STR, function(err, db) {
  console.log("连接成功！");
  //选中age集合，并用find方法把结果集拿回来进行处理
  db.collection("age").find({title: "cba"}).toArray(function(err, result) {
    if (err) {
      console.log('Error:' + err);
      return;
    }
    console.log(result);
  });
});


```

## 3.插入数据

insert函数第一个参数是需要插入的值(可以一个也可以多个)，第二个参数是接受一个回调函数，当值插入成功后回返回插入值得一些关键信息，比如`_id`

```
var MongoClient = require('mongodb').MongoClient;
var DB_CONN_STR = 'mongodb://localhost:27017/wscats';

MongoClient.connect(DB_CONN_STR, function(err, db) {
  console.log("连接成功！");
  db.collection("age").insert([
    {
      title: "插入的值A"
    }, {
      title: "插入的值B"
    }
  ], function(err, result) {
    if (err) {
      console.log('Error:' + err);
      return;
    }
    console.log(result)
  })
});


```

## 4.更新数据

注意如果不加$set就是完全替换原来的那份(没有设置的属性值将会丢失)，加上$set则只是更新对应的属性值，其余不做改变

```
var MongoClient = require('mongodb').MongoClient;
var DB_CONN_STR = 'mongodb://localhost:27017/wscats';

MongoClient.connect(DB_CONN_STR, function(err, db) {
  console.log("连接成功！");
  db.collection("age").update({
    "_id": 1
  }, {
    $set: {
      title: "你好，世界",
      skill: "js"
    }
  }, function(err, result) {
    if (err) {
      console.log('Error:' + err);
      return;
    }
    //console.log(result);
  });
});


```

## 5.删除数据

```
var MongoClient = require('mongodb').MongoClient;
var DB_CONN_STR = 'mongodb://localhost:27017/wscats';

MongoClient.connect(DB_CONN_STR, function(err, db) {
  console.log("连接成功！");
  db.collection("age").remove({
    "_id": 1
  }, function(err, result) {
    if (err) {
      console.log('Error:' + err);
      return;
    }
    //console.log(result);
    //关闭数据库
    db.close();
  });
});


```

## 6.关闭数据库

```
db.close();


```

# 封装自定义模块

新建`mongo.js`写入以下代码，封装自定义模块，方便其他路由复用，注意`assert`是node自带的断言模块，用于测试代码

参考

- [官网API文档](http://nodejs.cn/api/assert.html)
- [Node.js的断言模块assert进行单元测试](https://www.cnblogs.com/hong7zai/p/5909914.html)

```
const MongoClient = require('mongodb').MongoClient;
const assert = require('assert');
const url = 'mongodb://localhost:27017';
const dbName = 'shop';
function query(callback) {
	MongoClient.connect(url, function(err, client) {
		assert.equal(null, err);
		console.log("Connected successfully to server");
		const db = client.db(dbName);
		callback(db);
		client.close();
	});
}
module.exports = {
	query
}


```

在路由文件中引入和使用

```
var mongo = require('./mongo.js')
router.post('/addproduct', function(req, res, next) {
	mongo.query(function(db) {
		db.collection("product").insertMany([req.body], function(err, result) {
			console.log("Inserted 1 document into the collection");
			res.send('respond with a resource');
		});
	})
});


```

# 可视化

- [Robo 3T](https://robomongo.org/)
- [Studio3t](https://studio3t.com/download-thank-you/?OS=win64)

# 参考文档

- [易百-MongoDB教程](http://www.yiibai.com/mongodb/)
- [菜鸟-MongoDB教程](http://www.runoob.com/mongodb/mongodb-tutorial.html)

# 三、Robo使用方法

- 右键在New Connection
- 选create Database创建一个数据库
- 然后在新创的数据库中，找到下面的Collections右键
- 选Creat Collection新建表

# 10.19

## 一、mongod插入

```
var express = require('express');
var router = express.Router();
var db = require('../lib/db.js');
var mongo = require('../lib/mongo.js')
router.post('/addproduct', function(req, res, next) {
	console.log(req.body);	//接收前端返过来的信息
	console.log(db);
	db.query(function(db) {	//这里要用函数
		db.collection("product").insertMany([req.body], function(err, result) {
			console.log("Inserted 1 document into the collection");
			res.send('respond with a resource');
		});
	})
});

```

## 二、mongod查询数据库内容

```
router.get('/showproductlist', function(req, res, next) {
	console.log(req.body);
	console.log(db);
	db.query(function(db) {
		db.collection("product").find({}).toArray(function(err, docs) {
			console.log(docs)	//find中可写条件
			res.json({
				product: docs
			});
		});
	})
});

```

## 三、websocket

- [socket.io](https://github.com/Wscats/node-tutorial/issues/7)

ajax

1. 前端主动发，后端被动收（req,res）

websocket

1. 前端主动发，后端被动收（req,res）
2. 后端主动发，前端被动收（req,res）

socket.io包含两部分，一部分在node的express下设置，另一部部分浏览器页面下加载`socket.io.client.js`

### 前端

要下载客户端[socket.io.js](https://github.com/socketio/socket.io-client)文件，在页面中引入

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
	</head>
	<body>
		<script src="javascripts/socket.io.js"></script>
		<script>
			var socket = io('http://localhost:3001');
			socket.on('connect', function() {});
			socket.on('event', function(data) {});
			socket.on('disconnect', function() {});
			//监听
			socket.on('getServerMessage', function(data) {
				console.log(data)
			});
		</script>
	</body>
</html>
```

### 后端

在express中使用，以下代码

```js
var app = require('express')();
var server = require('http').createServer(app);
var io = require('socket.io')(server);
io.on('connection', function(){ /* … */ });
server.listen(3000);
```

| 接口            | 描述     |
| --------------- | -------- |
| `socket.on()`   | 接收信息 |
| `socket.emit()` | 发送信息 |

```js
var app = require('express')();
	var server = require('http').createServer(app);
	var io = require('socket.io')(server);
	io.on('connection', function(socket) {
		//发送socket信息的逻辑写在这里
		/* … */
		//监听
		//socket.on();
		//发送
		setInterval(()=>{
			socket.emit('getServerMessage',parseInt(Math.random()*100));
		},1000)
	});
	server.listen(3001);
```

**加**：[前端小插件](http://www.h-ui.net/Hui-overview.shtml)

# 10.29 vue介绍

[vue官网](https://cn.vuejs.org/)

## 一、用vue必做

#### 1. 先下载`vue.js`，然后在html文件中引入

```
<script src="https://cdn.jsdelivr.net/npm/vue@2.5.17/dist/vue.js"></script>
//中间的网址即为下载地址

```

#### 2.jquery与vue的异同

- `jquery.js`提供`$或者jquery`全局变量
- `vue.js`提供`vue`全局变量
- Vue的核心库只关注视图层，读音`view`
- 双向数据绑定，选项data里面数据变视图跟着变
- 如果页面注重操作节点，用jquery
- 如果页面数据比较多，建议用vue

## 二、开发工具

#### 1.用git下载工具，然后方便我们开发vue项目

```bash
git clone https://github.com/vuejs/vue-devtools.git
```

- 最好用npm下载不出错误
- 此时你会看到文件中多了一个`vue-devtools`文件
- 进入到这个文件npm install，安装依赖包； 
- 安装成功之后npm run build 
- 若不执行以上命令会报错，无法加载背景脚本"build/background.js"   //......
- 打开shells>chrome>manifest.json并把json文件里的"persistent":false改成true  //........
- 打开chrome浏览器，打开更多工具>扩展程序； 
- 再点击加载已解压的扩展程序，然后把shells>chrome文件夹放入 

```
备注：如果没有报错，则不用执行上面两个步骤

```

## 三、helloworld

#### 1.先实例化`Vue`,里面允许我们放很多选项(https://cn.vuejs.org/v2/api/),可以放**数据，DOM，生命钩子，资源和组合**

```js
var vm = new Vue({
  // 选项
})
```

#### 2.你用jQ，第一要有数据，第二要有节点，没节点，数据没意义

```js
$.ajax()//
$(el).html(data)
//寻找节点，然后放数据
```

#### 3.放入必要的选项，el和data是必须要有的

el就是寻找节点（找作用域），data就是配合`{{}}`来渲染数据

```js
var vm = new Vue({
    // 选项
    data:{
        name:"lemon1"
    },
    el:"#demo"
})
```

#### 4.在view层的`id`为`demo`的作用域里面配合`{{}}`绑定数据

```html
<div id="demo">
    <p>{{num+1+'1'}}</p>
</div>
```

## 四、jQuery和Vue的表达式和指令

#### 1.文本值

```
jq写法
$().text();

vue写法
<p>{{name}}</p>
<p v-text="name"></p>

```

#### 2.属性值

- `:style`和`:class`是必须接受一个对象

  ```
   <style>
          .red{
              color:red
          }
          .bg{
              background-color:yellow
          }
          .size{
              font-size:28px
          }
      </style>
      <div id="demo">
          <p :name="name" :id="name+'&laoxie'">属性</p>
          <p :style="style1">样式1</p>
          
          ===========================================
          <p :style="{
              color:'red',
              fontSize:'14px',
              backgroundColor:'yellow'
          }">样式2</p>
          <p :class="class1">样式1</p>
      </div>
      =====================================================
      <script src="../../js/vue.js"></script>
   
   var vm = new Vue({
              // 选项
              // 数据选项
              data:{
                  name:"lemon",
                  style1:{
                      color:'red',
                      fontSize:'14px',
                      backgroundColor:'yellow'
                  },
                  class1:{
                      red:true,
                      bg:false,
                      size:true
                  }
              },
              el:"#demo"
          })
    
    解释：就是你要是写style样式，或者是要以类名的方式添加样式，就要在下面写成对象的方式，然后再给上面添加变量即可
  
  ```

  

- `:xxx`都可以接受任何变量

```
jq写法
$().attr();
$().css();
$().addClass();

vue写法
<p :name="name"></p>

```

- 插入html结构

```
$().html()

<div v-html="html"></div>

```

- 显示或者隐藏，本质是控制css，节点一直存在的，频繁切换（选项卡，加载的动画）

```
jq写法
$().show()
$().hide()

vue写法
<div v-show="!bool">你好</div>

```

- 对节点增加或者删除，节点要不存在或者不存在

```
jq写法
$().append()
$().remove()

vue写法
<div v-if="!bool">你好</div>
<div v-else>假的</div>

```

- v-for放哪里，那个节点就跟着遍历对应的数组,支持嵌套其他指令`v-for,v-if和v-show`

```html
jq写法
$().each()

vue写法
<div v-for="item in arr" v-text="item.name"></div>

备注：
v-for 指令需要以 site in sites 形式的特殊语法， sites 是源数据数组并且 site 是数组元素迭代的别名。
v-for 可以绑定数据到数组来渲染一个列表
```

- `v-on:click`简写为`@click`，就是把原生的onmousedown->@mousedown，把on改为@，把事件监听函数方法选项的`methods`里面

```html
jq写法
$().on()
$().click()

vue写法
<button @click="loadMore">查看更多</button>
```

- `v-bind:xxx`简写为`:xxx`

```html
<p v-bind:name="name">测试</p>
==============================
<p :name="name">测试</p>
备注：两种写法为一个意思
```

- `v-model`是把视图的值，带回选项`data`里面，只能用在这三个标签里面
- 视图层影响数据层`v-model`或者`v-on:click`

```
<input v-model="name" />
<select>
<textarea>

备注：v-model相当于把你文本框里输入的值赋给name,然后再把name赋给p标签

```

# 指令使用示意图

<img src="E:/H5%E6%AF%8F%E5%A4%A9/%E4%B8%89%E9%98%B6%E6%AE%B510.15/6.10.29~vue/vue/public/vue/day1/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-10-29%20%E4%B8%8B%E5%8D%883.38.33.png" />

## 五、data、methods、{{}}

- data用于定义属性

```
例如：
data:{
    name:"lemon",
    style1:{
    color:'red',
    fontSize:'14px',
    backgroundColor:'yellow'
},

```

- methods 用于定义的函数，可以通过 return 来返回函数值。 

```
methods: {
    testClick: function () {
    console.log("你触发了点击事件")
    },
    testKeyup() {
    console.log("你触发了输入事件")
    },
    loadMore() {
    this.arr.push({
    name: 'laotian',
    age: 16,
    skill: ['xmind']
    })
    }
}

```

- {{ }} 用于输出对象属性和函数返回值。 

```
<div id="demo">
        <p>{{name}}</p>
        <p>{{arr}}</p>
        <p>{{arr[0]}}</p>
    </div>

```

## 六、模板语法

- 使用v-html指令用于输出html代码

```
<div id="demo">
        <div v-html="html"></div>
    </div>
    <script src="../../js/vue.js"></script>
    <script>
        new Vue({
            el: "#demo",
            data: {
                html: "<p>123<span>456</span>789</p>"
            }
        })
    </script>

备注：v-html一般用于输出HTML结构

```

# 10.30

## 一、vue脚手架安装步骤

https://cli.vuejs.org/

#### 1.全局安装

```bash
npm install -g @vue/cli
```

#### 2.安装完，会在全局有vue命令

```bash
vue -V
```

#### 3.创建项目

```bash
vue create weibo
```

#### 4.定位到该文件夹

```
cd weibo

```

#### 5.启动服务器

```
npm run serve

```

# 11.12

- 利用路由传递参数

```
this.$route.push({path:'/xxx',query:{id:1}});//类似get传参，通过URL传递参数
this.$route.push({path:'/xxx',params:{id:1}});//类似post传参

```

- 接收参数

```
this.$route.query.id
this.$route.params.id

```

- 利用emit发送数据

```
this.$emit('showCityName',data);

```

- 利用on接收数据

```
this.$on('increment',function(msg){
                //获取$emit方法传递的第二个参数
                console.log(msg);
                alert("1");
            })

```

# 11.12

## 一、react脚手架安装步骤

```
$ cnpm install -g create-react-app	//全局安装react
$ create-react-app my-app			//创建脚手架
$ cd my-app/						
$ npm start

```

## 二、react添加取消类名方式

#### 1. 添加取消类名

> 思路：现在上面定义一个变量，例如：isShowSearchBar:true，然后给你要点击的那个东西添加onClick={}事件，然后根据变量的true和false来决定添加取消类名，

```
 className={this.state.isShowSearchBar? "weui-search-bar": "weui-search-bar weui-
search-bar_focusing"}

============定义变量阶段================
 constructor(props){
        super(props);
        this.state = {
            isShowSearchBar:true
        }
    }
    
=============改变变量阶段================
changeSearchBar(){
        this.setState({
            isShowSearchBar:!this.state.isShowSearchBar
        })
 }
 
 ==================绑定事件阶段==========
<a href="javascript:" onClick={this.changeSearchBar.bind(this)} className="weui-search-bar__cancel-btn" id="searchCancel">取消</a>


========================================================



```

#### 2. tab切换形式

> 思路：先定义一个变量为0，以索引的形式切换，把点击事件写给你要点击的东西，当你点击的时候，把索引传给函数，通过函数事件把index赋给你定义的变量，然后在下面根据你的变量等于索引的三元表达式形式，添加类名，例子如下：

```
class Xfooter extends Component {
    constructor(props){
        super(props);
        this.state = {
            tab:0,
            tabs:[{
                title:"微信",
                href:"wechat",
                num:8,
                dot:false
            },{
                title:"通讯录",
                href:"contact",
                num:0,
                dot:true
            },{
                title:"发现",
                href:"research",
                num:0,
                dot:false
            },{
                title:"我",
                href:"mine",
                num:0,
                dot:false
            }]
        }
    }
====================================================
 toggloClass(index,e){
        this.setState({
            tab:index
        })
    }
    
 ===================================================
  <a href="javascript:;" key={index} onClick={this.toggloClass.bind(this,index)} className={this.state.tab==index? "weui-tabbar__item weui-bar__item_on": "weui-tabbar__item"}>

```



## 三、文本框聚焦

> 思路：先给你要聚焦的文本框绑定ref=“变量名”，然后在你的点击事件里面写，this.refs.变量名.focus();既可聚焦

```
==================
this.refs.imput.focus();

==========================================
<input ref="imput" type="search" className="weui-search-bar__input" id="searchInput" placeholder="搜索" required="" />


```

## 四、获取文本框的value方法

> 思路：先给文本框绑定onChange事件，记住要用大括号的形式{}，在上面的事件函数里面传个e，就直接获取e.target.value,然后再上面this.state里面定义一个变量，例如：searchValue:"",然后通过this.setState({})的方法把值赋给那个变量既可。

```
==============定义阶段===============
  constructor(props){
        super(props);
        this.state = {
            isShowSearchBar:true,
            searchValue:""
        }
    }
    
    
    ==========获取文本框值阶段========
    
  getInputValue(e){
       this.setState({
            searchValue:e.target.value
       })
        console.log(e.target.value)
    }

```

## 五、函数式编程

> 思路：函数式编程就相当于vue里面的v-for一样，你需要在上面先定义好数组，然后在下面遍历数组，把东西return出来

```
步骤：1.先在上面定义一个数组
	 2.然后在下面写一个自执行的函数，例如：{(()=>{
	 	return this.state.tabs.map((item,index)=>{
                
	 		})
	 	
	 })()}

```

## 六、axios请求、渲染页面

> 思路：如果你需要一进页面就进行渲染，你需要把你进行ajax请求的函数，挂载到componentDidMount里面去执行，就是你在上面render()前进行ajax请求，到render()里面写函数，
>
> 到componentDidMount去执行，例如：

```
  ==========axios请求阶段============
  loadMore () {
    var self = this;
    // React.axios.get("http://tingapi.ting.baidu.com/v1/restserver/ting",{
    React.axios.get('music.json', {
      params: {
        method: 'baidu.ting.billboard.billList',
        type: 1,
        size: 10,
        offset: 0

      }
    }).then((response) => {
      console.log(response.data.song_list)
      self.setState({
        song:response.data.song_list
      })
    }).catch(function (error) {
      console.log(error)
    })
  }
  ================渲染阶段==================
       {(() => {
          return this.state.song.map((item,index) =>{
            return (
              <a href='javascript:void(0);' key={index} className='weui-media-box weui-media-box_appmsg'>
            <div className='weui-media-box__hd'> <img className='weui-media-box__thumb' src={item.album_500_500}
                alt='' /> </div>
            <div className='weui-media-box__bd'>
              <h4 className='weui-media-box__title'>{item.title}</h4>
              <p className='weui-media-box__desc'> {item.si_proxycompany}</p>
            </div>
          </a>
            )
          })
        })()}
        
 =====================挂载阶段======================       
     componentDidMount(){
    	this.loadMore();
   
  }

```

## 七、路由的用法

#### 1. 路由的起步

- 下载路由模块

```
npm install react-router-dom

```

- 在index.js引入

```
import { BrowserRouter as Router, Route, Link } from "react-router-dom";

```

- 在index.js外面包上`<Router></Router>`

```
ReactDOM.render(
  <Router>
    <div>
      <Xheader />
      <Xsearch />
      <Xpannel />
      <Xfooter />
    </div>
  </Router>,
  document.getElementById('root'))

```

#### 2. 路由的跳转实现及步骤

- 建议在index.js页面引入哈希路由

```
import { HashRouter  as Router, Route } from 'react-router-dom'

```

- 在ReactDOM.render下面写上

```
ReactDOM.render(
  <Router>
    <div>
      <Route path="/home/" component={Home} />			//判断路径如果是/home/就去home组件
      <Route path="/Detail/" component={Detail} />		//判断路径如果detail就去detail组件

      {/* <Redirect from="/home" to="/home/wechat" /> */}

    </div>
  </Router>,
  document.getElementById('root'))

```

- 然后在home页面引入路有插件和小组件

```
import { Route } from 'react-router-dom'

import Wechat from '../Wechat/Wechat'
import Contact from '../Contact/Contact'
import Research from '../Research/Research'
import Mine from '../Mine/Mine'

```

- 根据路径判断调到那个路由

```
<Route path="/home/wechat"  component={Wechat} />
<Route path="/home/contact" component={Contact} />
<Route path="/home/research" component={Research} />
<Route path="/home/mine" component={Mine} />

```

- 去Xfooter页面引入路由组件

```
import { Link } from 'react-router-dom'

```

- 把`a`标签改为`Link`，然后在里面写`to{/home/${item.href}}`

```
<Link to={`/home/${item.href}`}></Link>
解释：你的href要在上面就定义好，然后直接调用，例如：
{title:"微信",
href:"wechat",
num:8,
dot:false}

```

#### 3. 设置默认路由

- 进入页面引入时加`Redirect`

```
import { HashRouter  as Router, Route , Redirect ,Switch} from 'react-router-dom'

```

- 下面写默认路由

```bash
ReactDOM.render(
    <Provider store={store}>
        <Router>
            <div className="container iphonex_padding">
                <Switch>
                    <Route path="/home/" component={Home} />
                    <Redirect from="/" exact  to="/home/HomeIndex" />
                </Switch>
            </div>
        </Router>
  </Provider>, document.getElementById('root'));
  
  ======================
 <Link to={ {pathname:`/home/${item.href}` }}  replace >
 </Link>
```

## 八、redux组件通信

- 先下载这两个模块

```
npm install --save react-redux
npm install --save redux

```

- 在index.js引入

```
//redux
import {Provider, connect} from 'react-redux';
import {createStore} from 'redux';

```

- 创建仓库

```
const store = createStore(function(state={

},action){})

```

- 在下面用`Provider`包住

```bash
ReactDOM.render(
  <Provider store={store}>		//注入store
  <Router>
    <div>
      <Route path="/home/" component={Home} />
      <Route path="/Detail/" component={Detail} />

      <Redirect from="/home" to="/home/wechat" />

    </div>
  </Router>
  </Provider>,
  document.getElementById('root'))
```

- 在你要用redux的仓库引入

```
import { connect} from 'react-redux';

```

- 在最下面写

```
export default connect((state)=>{
    return state	//把你从仓库拿到的东西return出来
},(dispatch)=>{
    return {
        toggleSheet() {			//把你改的东西return出去
          dispatch({
            type: 'toggleSheet',
            isShowActionSheet: false
          })
        }
      }
})(XactionSheet)


================在结构里面写的=================
 <div className="weui-skin_android" onClick={this.props.toggleSheet} id="androidActionsheet" style={{
            opacity: 1,
            display:this.props.isShowActionSheet ? "block": "none"
         }}>

```

- 在index.js里面接收回你改的东西

```bash
const store = createStore(function(state={
    isShowActionSheet:false		//初始化设置为false
},action){

    switch (action.type) {
      case 'toggleSheet':	//如果类型为 ‘toggleSheet’
        return {		
            ...state,		//展开state
            isShowActionSheet:action.isShowActionSheet	//设置为接收回来的状态
        }
      default:
        return state	//默认返回state的东西
    }
})
```

## 九、组件

- 里面包含html，css，js

```
.vue

```

- react是把所有的html，css都放进js文件里面
- react定义组件，先创建`xxx.js`，在文件里面引入`react`模块

```js
import React, { Component } from 'react';
```

- 所有组件继承于`Component`

```
class 组件名字 extends Component {}

```

- 导出组件

```js
export default App;
```

#### 1. antdUI用时

```bash
用`antdui`时记得要把`css`找到，要不然出不来
```

#### 2. redux记住switch

```bash
使用redux时，记住一定要把东西在仓库就先return出来，要不然外边拿不到
  switch (action.type) {
    //   case 'toggleSheet':
    //     return {
    //         ...state,
    //         isShowActionSheet:action.isShowActionSheet
    //     }
      default:
        return state
    }
```

#### 3. react路由设置、及重定向

```bash
路由冲定向时会报错，记得要引入	**import { HashRouter  as Router, Route , Redirect ,Switch} from 'react-router-dom'

===========
用switch包住你的路由判断那里
<Switch>
    <Route path="/home/" component={Home} />
    <Redirect from="/" exact  to="/home/HomeIndex" />
</Switch>

===============
在link里面要把普通的`to`改成`to={ {pathname:`/home/${item.href}` }}  replace`

```

#### 4. redux修改仓库中数组的某一项、实现联动效果

```bash
如果你要是想通过点击事件触发仓库中的某一个值，是数组的情况下，你需要遍历仓库中的数组，把你要变得索引传过来，然后让其他的不变，例如：
const store = createStore(function (state = {
    navs: [{
      title: '推荐',
      href: 'recommend',
      isShow:true,
      recommend: []
    }, {
      title: '少儿',
      href: 'children',
      isShow:false,
      children: []
    }, {
      title: '成人',
      href: 'adult',
      isShow:false,
      adult: []
    }, {
      title: '父母',
      href: 'parents ',
      isShow:false,
      parents: []
    }, {
      title: '家庭',
      href: 'family',
      isShow:false,
      family: []
    }, {
      title: '旅行',
      href: 'travel',
      isShow:false,
      travel: []
    }]
  } ,action) {
  switch (action.type) {
      case 'isActive': 
      var  {navs}  = state		 // 把仓库赋值给navs
      for(var i=0;i<navs.length;i++){	 // 遍历navs仓库，找到你要的东西
        navs[i].isShow=false
        navs[action.index].isShow =action.isShow
        console.log(navs[i])
      }
      navs.isShow = action.noShow
        return {
            ...state,
            isShow:false
        }
    default:
      return state
  }
})
===============触发那边==============

export default connect((state)=>{
    return state    
} , (dispatch) => {
    return {
        isActive(index){
            console.log(this.props)
            this.setState({
                isActive:index		//修改本地的内容
            })
            dispatch({
                type:"isActive",
                index: index,	//传索引`index`
                isShow:true		//传状态
              })
        }
    }
})(Xnav);
```

#### 5. 不要写错路由`字母`

#### 6. 路由嵌套问题

> 在哪个页面的二级路由，就写在哪个页面，例如：你要在首页写二级路由，你就把二级路由写在首页，
>
> 然后一级路由会基于你二级路由跳转的路径跳转，所以你要加个斜杠`/`在一级路由那里`/${item.href}` 

```bash
 ===================二级路由home写法=====================
 <Route path='/home/Xrecommend' component={Xrecommend} />
 <Route path="/home/Xchildren"  component={Xchildren} />
 <Route path="/home/Xadult" component={Xadult} />
 <Route path="/home/Xparents" component={Xparents} />
 <Route path="/home/Xfamily" component={Xfamily} />
 <Route path="/home/Xtravel" component={Xtravel} />
 
 =============一级路由跳转稳的写法=============
  <Link to={ {pathname:`/${item.href}` }}  replace key={index} onClick={this.toggleClass.bind(this,index)}  className={this.state.tab===index? "public_tab_item active" : "public_tab_item"} id={item.dataId}>
  <div className="public_tab_info">
  <p className={`public_tab_icon ${item.dataClass}`}></p>
  <p>{item.title}</p>
  </div>	
  </Link>
```

#### 7. 类名打回来

> 如果你要是想要类名刷新打回来，必须获取到路径，根据路径的变化，判端打在那个东西下面，例如：
>
> `window.location.hash.slice(2) `[参考链接](http://www.cnblogs.com/icaihua/p/9869846.html)

```bash
 switch (window.location.hash.slice(2)) {
        case "/home/Xrecommend":
          this.state.tab=0
          break;
          case "bestchoice":
          this.state.tab=1
          break;
          case "search":
          this.state.tab=2
          break;
          case "mine":
          this.state.tab=3
          break;
        default: this.state.tab=0
          break;
      }
  }
  **然后下面根据路径变化打类名
  
 =============正常方法================
 // 根据路径给togoleclass赋值
     switch (props.location.pathname) {
      case "/home/Xrecommend":
      this.state.togolleClass=0
        break;
        case "/home/Xchildren":
      this.state.togolleClass=1
        break;
        case "/home/Xadult":
      this.state.togolleClass=2
        break;
        case "/home/Xparents":
      this.state.togolleClass=3
        break;
    case "/home/Xfamily":
      this.state.togolleClass=4
        break;
    case "/home/Xtravel":
      this.state.togolleClass=5
        break;
      default:
        this.state.togolleClass=0
        break;
    }
    ===========传值给子组件==========
    <Xnav tab={this.state.togolleClass}/>
    ==========接收============
    this.props = props; 
    ===========赋值==============
    this.state = {
        isActive:this.props.tab
       
    }
  //然后下面根据三元正常判断即可  
```

#### 8. 严选页根据点击事件世事变化，切换选项卡问题

> 不能用redux，因为你的props不能当你每点击一次都能实时更新，只有当你刷新页面时才会更新，所以用`发布订阅模式`emit发送，on监听接收，以达到实时的效果，例如：

```bash
=============发送数据`索引`==============
store.emit("show",index);

=============接收数据，把数据存到本地仓库=====================
  componentDidMount(){
        store.on("show",(data)=>{
            console.log(data);
            this.setState({
                content:data
            })
        })
    
    }
 然后根据this.state.content的`数值索引`出现不同的选项卡
```

#### 9.邮箱验证码步骤及思路

> 思路：当你点击发送验证码时，发起ajax请求，后端生成验证码，发送到你上面`注册`的邮箱，后端缓存验证码，留到用户拿到验证码输入时进行比对，正确，则插入数据库，失败不插入

- 先下载模块`nodemailer`

```bash
cnpm install nodemailer --save-dev
```

- 引入模块

```bash
const nodemailer = require('nodemailer');	//引入模块
let transporter = nodemailer.createTransport({
    service: 'qq',	//类型qq邮箱
    port: 465,
    secure: true, // true for 465, false for other ports
    auth: {
        user:'854453495@qq.com', // 发送方的邮箱
        pass: 'vrtjembbhfcmbegj' // smtp 的授权码
    }
});


function sendMail(mail,code,call){
    // 发送的配置项
    let mailOptions = {
        from: '"Fred Foo 👻" <854453495@qq.com>', // 发送方
        to: mail, // 接收方
        subject: '欢迎注册“小雨伞”保险！', // 标题
        text: 'Hello world?', // 文本内容
        html: `<h1>您的验证码是:${code},请注意安全性，该验证码有效期为 5分钟</h1>`//页面内容
    };

   //发送函数
    transporter.sendMail(mailOptions, (error, info) => {
    if (error) {
       call(-1)
    }
     call(0)//因为是异步 所有需要回调函数通知成功结果

    });

}

module.exports={sendMail}
```

- 接收前端路由处

```bash
var express = require('express');
var router = express.Router();
var db = require('../lib/db.js');
var email = require('./sendEmail.js');	//引入封装好的函数
console.log(email)
//解决跨域问题
router.all('*', function (req, res, next) {
  res.header('Access-Control-Allow-Origin', '*');
  //Access-Control-Allow-Headers ,可根据浏览器的F12查看,把对应的粘贴在这里就行
  res.header('Access-Control-Allow-Headers', 'Content-Type');
  res.header('Access-Control-Allow-Methods', '*');
  res.header('Content-Type', 'application/json;charset=utf-8');
  next();
});

/* GET users listing. */
router.get('/', function(req, res, next) {
  res.send('respond with a resource');
});


let check={}	//声明一个对象缓存邮箱和验证码，留着
router.post('/email', function(req, res, next) {
    console.log(req.body.params)
    let mail=req.body.params.email
    if (!mail) {return res.send('参数错误')}	//email出错时或者为空时
    let code = parseInt(Math.random(0,1)*10000)	//生成随机验证码
    check[mail]=code
    //发送邮件
     email.sendMail(mail,code,(state)=>{
            if (state) {
                res.send('验证码发送成功')
            }else{
               res.send('验证码发送失败')
            }
            
      })
   
  
});
router.post('/login', function(req, res, next) {
    console.log(req.body.params)
     db.query(function(db) { //这里要用函数
        db.collection("login").insertMany([req.body.params], function(err, result) {

            res.send('succees');
        });
    })

});
module.exports = router;




```

#### 10.路由获取方法

> 思路：在最大的组件获取到路由，通过props方法传到需要的子组件去
>
> 备注：因为小组件拿不到props

```bash
var url = this.props.loction.pathname
<Xheader url={url}/>
```

#### 11.路由跳转的两种方式

> 备注：如果不是需要注册登录那种判断，用Link即可，快、准、狠！

- Link方式

```bash
import { Link  } from 'react-router-dom'

<Link to={ {pathname:`/${item.href}` }}  replace > </Link>
```

- withRouter 方式

```bash
import { withRouter   } from 'react-router-dom'
===========React-Router 2.4.0版本以上=========
import { withRouter } from 'react-router';
clsss ABC extends Component {
}
module.exports = withRouter(ABC);

===========React-Router 3.0.0版本以上=========
this.props.router.push('/home/Xrecommend')

===========React-Router 4.0版本以上===========
this.props.history.push('/home/Xrecommend')
```

> 稳稳的写法

```bash
 import { withRouter   } from 'react-router-dom'
 =============================================
 goCar(){
    this.props.history.push('/carOrder')
  }
 ============================================= 
  export default withRouter(Xorder)
```



#### 12.参数的获取

```bash
使用`this.props.match.params.xxx` 可以获取到当前路由的参数
```

#### 13.react `cookie`用法

- 先下载模块

```bash
cnpm install  react-cookie --save-dev
```

- 引入

```
import cookie from 'react-cookies'

```

- 存入`cookie`

```visual basic
cookie.save('userId', this.state.value)；
```

- 删除`cookie`

```
cookie.remove('userId')

```

- 获取`cookie`

```
select([regex])
this.state =  { userId: cookie.load('userId') };

```

#### 14.React的Sass配置

- 先下载

```bash
npm install sass-loader node-sass --save-dev
```

- 找到配置文件，

```bash
node_modules/react-scripts/config/webpack.config.dev.js
```

- 找到module下的rules，然后找到最后一个配置，修改成如下的样子 

```bash
{

    exclude: [/\.js$/,/\.html$/,/\.json$/,/\.scss$/],

    loader: require.resolve('file-loader'),

    options: {

            name: 'static/media/[name].[hash:8].[ext]',

        },

},

{

    test:/\.scss$/,

    loaders:['style-loader','css-loader','sass-loader']

}

备注：如果不行的话，再把`webpack.config.prod.js`也变成同样的配置
```

#### 15.loading效果

> veu、react通用

- 下载、引入axios

```bash
========react=========
cnpm install axios --save-dev
import axios from 'axios'
=========vue==========
cnpm install mint-ui --save-dev
import Mint from 'mint-ui';
Vue.use(Mint);
```

- 下载引入antd-mobile 

```bash
=========react==========
import { Toast } from 'antd-mobile';
import './assets/antd-mobile.css'
==========vue===========
```

- 引入样式

```bash
备注：样式在node-modues里面，可自行找路径，或复制过来
import './assets/antd-mobile.css'
*vue如需引用样式，同理
import 'mint-ui/lib/style.css';
```

- 在index.js写如下代码

```bash
=============请求之前loading==============
axios.interceptors.request.use((config) => {
  Toast.loading('', 3,true);
	return config;
}, (err) => {
	return Promise.reject(err)

})
===========请求成功之后取消loading=======
axios.interceptors.response.use((response) => {
	Toast.hide(); //关闭loading
	return response;
}, (err) => {
	return Promise.reject(err);

})
```

- 在vue的main.js中

```bash
============请求之前loading==============
Axios.interceptors.request.use((config) => {
	Mint.Indicator.open({ //打开loading
		text: '加载中...',
		spinnerType: 'fading-circle'
	});
	return config;
}, (err) => {
	return Promise.reject(err)

})
==============请求成功之后取消loading=======
Axios.interceptors.response.use((response) => {
	Mint.Indicator.close(); //关闭loading
	return response;
}, (err) => {
	return Promise.reject(err);

})
```

#### 16.回退`goback()`用法

```bash
===========后退=========
goback(){
      this.props.history.goBack()  
  }
===========前进========
 push(){
      this.props.history.push()  
  }
备注：需要写个点击事件
```

#### 17.解决异步渲染`axios`问题

> 思路：先定义一个开关为`false`，然后在回调里面设置为`true`，根据`true`跟`false`判断是否渲染

```
    this.state = {
        showRender:false,
    }
    
    =========================
    if(this.state.showRender){
        //渲染
    }

```

# 11.26 小程序

### 一、小程序起步

1.先去[微信小程序官网](https://mp.weixin.qq.com/cgi-bin/wx)注册账号

> 备注：如果要是个人用的话注册隔热即可

2.进入官网看文档

## 二、微信小程序路由配置

- 在`pages`里面新建pages会在`pack.json`自动生成路由

```bash
  "pages": [
    "pages/index/index",
    "pages/logs/logs",
    "pages/mine/mine",
    "pages/serach/search",
    "pages/find/find"
  ],
```

- `tabBar`写在window后面

```bash
  "tabBar": {
    "selectedColor": "#666",	//选中时的样式
    "list": [
      {
        "pagePath": "pages/index/index",
        "text": "首页",
        "iconPath": "./pages/images/首页-未选中.png",	//字体图标路径
        "selectedIconPath": "./pages/images/首页-选中.png"	//选中时字体图标路径
      },
      {
        "pagePath": "pages/serach/search",
        "text": "发现",
        "iconPath": "./pages/images/发现未选中.png",
        "selectedIconPath": "./pages/images/发现-选中.png"
      },
      {
        "pagePath": "pages/logs/logs",
        "text": "日志",
        "iconPath": "./pages/images/日志.png",
        "selectedIconPath": "./pages/images/日志选中.png"
      },
      {
        "pagePath": "pages/mine/mine",
        "text": "我的",
        "iconPath": "./pages/images/我 的.png",
        "selectedIconPath": "./pages/images/我的选中.png"
      }
    ]
  },
```

## 三、数据绑定及渲染

#### 1.渲染用两个`{{}}`花括号

```bash
<view> {{ message }} </view>

Page({
  data: {
    message: 'Hello MINA!'
  }
})
```

- `wx:if`用法

> 备注：这种属性方法的都要用`"{{}}"`这种形式，例如，`wx:for="{{}}"`、
>
> `wx:if="{{}}"`、`checked="{{false}}"`，还有三元运算`hidden="{{flag ? true : false}}"`

#### 2.列表渲染`wx:for`

> 在组件上使用 `wx:for` 控制属性绑定一个数组，即可使用数组中各项的数据重复渲染该组件。
>
> 默认数组的当前项的下标变量名默认为 `index`，数组当前项的变量名默认为 `item`

```
<view wx:for="{{array}}">
  {{index}}: {{item.message}}
</view>

```

## 四、做音乐播放器小程序步骤

#### 1.先创建你需要的页面及路由

> 例如：先创建一个首页、一个详情页、搜索页

#### 2.引入`weui` 、search组件、pannel组件

#### 3.新建`components`在里面写小组件

#### 4.在index.js发起ajax请求，利用组件通信传到pannel组件里面

```ruby
Page({
  data:{
    song_list:[],	//定义一个空数组
    offset:0
  },
  onReady(){
    this.loadMore()
  },
  onLoad: function () {
    this.setData({
      icon20: base64.icon20,
      icon60: base64.icon60
    });
  },
  onPullDownRefresh() {
    this.loadMore()
  },
  loadMore() {
    var self = this;
    wx.request({
      url: 'https://tingapi.ting.baidu.com/v1/restserver/ting', //仅为示例，并非真实的接口地址
      data: {
        method: "baidu.ting.billboard.billList",
        type: 1,
        size: 10,
        offset: this.data.offset
      },
      header: {
        'content-type': 'application/json' // 默认值
      },
      success(res) {
        wx.stopPullDownRefresh()
        self.setData({
          offset:++self.data.offset
        })
        console.log(res.data.song_list)
   //把请求回来的数据合并到空数组，因为是上拉刷新，所以就要用新数组合并旧数据，以达到每次上面都是新的
        self.setData({
          song_list: res.data.song_list.concat(self.data.song_list) 
        })
      }
    })
  }
```

#### 5.利用组件通信传数据到子组件

```ruby
<xpannel songList="{{song_list}}"></xpannel>
```

#### 6.接收父组件传过来的数据

```ruby
 properties: {
    songList: { // 属性名
      type: Array, // 类型（必填），目前接受的类型包括：String, Number, Boolean, Object, Array, null（表示任意类型）
      value: '', // 属性初始值（可选），如果未指定则会根据类型选择一个
      observer: function (newVal, oldVal, changedPath) {
        console.log(newVal)
        this.setData({
          song: newVal	//把接收过来的数组存到本地
        })
        // 属性被改变时执行的函数（可选），也可以写成在methods段中定义的方法名字符串, 如：'_propertyChange'
        // 通常 newVal 就是新设置的数据， oldVal 是旧数据
      }
    },
  },
```

#### 7.动态渲染接收过来的数据

```bash
 <navigator url="{{'/pages/detail/detail?songId='+item.song_id}}" wx:for="{{song}}" 		class="weui-media-box weui-media-box_appmsg" hover-class="weui-cell_active">
     <view class="weui-media-box__hd weui-media-box__hd_in-appmsg">
     <image class="weui-media-box__thumb" src="{{item.pic_big}}" />
     </view>
     <view class="weui-media-box__bd weui-media-box__bd_in-appmsg">
     <view class="weui-media-box__title">{{item.album_title}}</view>
     <view class="weui-media-box__desc">{{item.country}}-{{item.author}}</view>
     </view>
 </navigator>
```

#### 8.传`songid`到详情页

> 传songid到详情页的目的是，让详情页根据你传过来的id发起ajax请求，渲染数据

```bash
<navigator url="{{'/pages/detail/detail?songId='+item.song_id}}" wx:for="{{song}}" class="weui-media-box weui-media-box_appmsg" hover-class="weui-cell_active">

备注：通过拼接字符串的形式传送 url="{{'/pages/detail/detail?songId='+item.song_id}}" 
```

#### 9.接收传过来的`id`,设置给本地变量

```bash
  onLoad: function (options) {
    // console.log(options.songId)
    this.setData({
      songId: options.songId
    })
    
    this.getSong();
    this.getlrc()
    console.log(this.data.songId)
  }
备注：`options`为形参，好比vue和react中的`props`
```



#### 10.在详情页引入`audio`组件

- html页面

```bash
<!-- audio.wxml -->
<audio poster="{{poster}}" name="{{name}}" author="{{author}}" src="{{src}}" id="myAudio" controls loop></audio>

<button type="primary" bindtap="audioPlay">播放</button>
<button type="primary" bindtap="audioPause">暂停</button>
<button type="primary" bindtap="audio14">设置当前播放时间为14秒</button>
<button type="primary" bindtap="audioStart">回到开头</button>
```

- js页面

```bash
// audio.js
Page({
  onReady: function (e) {
    // 使用 wx.createAudioContext 获取 audio 上下文 context
    this.audioCtx = wx.createAudioContext('myAudio')
  },
  data: {
    poster: 'http://y.gtimg.cn/music/photo_new/T002R300x300M000003rsKF44GyaSk.jpg?max_age=2592000',
    name: '此时此刻',
    author: '许巍',
    src: 'http://ws.stream.qqmusic.qq.com/M500001VfvsJ21xFqb.mp3?guid=ffffffff82def4af4b12b3cd9337d5e7&uin=346897220&vkey=6292F51E1E384E06DCBDC9AB7C49FD713D632D313AC4858BACB8DDD29067D3C601481D36E62053BF8DFEAF74C0A5CCFADD6471160CAF3E6A&fromtag=46',
  },
  audioPlay: function () {
    this.audioCtx.play()
  },
  audioPause: function () {
    this.audioCtx.pause()
  },
  audio14: function () {
    this.audioCtx.seek(14)
  },
  audioStart: function () {
    this.audioCtx.seek(0)
  }
})
```

#### 11.把引入的`audio`参数全变成变量

```bash
  data: {
    songId:"",
    poster: '',
    name: '',
    author: '',
    src: '',
    lrc:"",
    time:0
  },
```

#### 12.发起ajax请求把请求回来的数据赋给data里面的变量

```bash
 getSong() {
    var self = this;
    wx.request({
      url: 'https://tingapi.ting.baidu.com/v1/restserver/ting', //仅为示例，并非真实的接口地址
      data: {
        method:"baidu.ting.song.play",
        songid:this.data.songId
      },
      header: {
        'content-type': 'application/json' // 默认值
      },
      success(res) {
      console.log(res.data)
      self.setData({
        poster: res.data.songinfo.pic_big,
        name: res.data.songinfo.title,
        author: res.data.songinfo.author,
        src: res.data.bitrate.file_link
      })
      }
    })
  }
  备注：此时就可以播放歌曲了
```

#### 13.歌词处理

```bash
 getlrc() {
    var self = this;
    wx.request({
      url: 'https://tingapi.ting.baidu.com/v1/restserver/ting', //仅为示例，并非真实的接口地址
      data: {
        method:"baidu.ting.song.lry",
        songid:this.data.songId
      },
      header: {
        'content-type': 'application/json' // 默认值
      },
      success(res) {
        // console.log(res.data)
        let obj = self.parseLyric(res.data.lrcContent)	//执行函数拿到歌词
        console.log(obj)
        self.setData({
          lrc: obj
        })
      
   
      }
    })
  },
  //把歌词处理成一段一段的
  parseLyric(lrc) {
    var lyrics = lrc.split("\n");
    var lrcObj = {};
    for (var i = 0; i < lyrics.length; i++) {
      var lyric = decodeURIComponent(lyrics[i]);
      var timeReg = /\[\d*:\d*((\.|\:)\d*)*\]/g;
      var timeRegExpArr = lyric.match(timeReg);
      if (!timeRegExpArr) continue;
      var clause = lyric.replace(timeReg, '');
      for (var k = 0, h = timeRegExpArr.length; k < h; k++) {
        var t = timeRegExpArr[k];
        var min = Number(String(t.match(/\[\d*/i)).slice(1)),
          sec = Number(String(t.match(/\:\d*/i)).slice(1));
        var time = min * 60 + sec;
        lrcObj[time] = clause;
      }
    }
    return lrcObj;
  },
```

#### 14.渲染歌词

> 你可以在本地设置个时间为time:0,然后再设置个定时器，让time每秒+1，根据time渲染歌词

```bash
   data: {
    songId:"",
    poster: '',
    name: '',
    author: '',
    src: '',
    lrc:"",
    time:0	//设置tiem
  },
  ======================
  audioPlay: function () {
    this.audioCtx.play();
    timer=setInterval(() => {
      this.setData({
        time: ++this.data.time
      })
    },1000)
  },
  //按暂停时清除定时器	
    audioPause: function () {
    this.audioCtx.pause();
    clearInterval(timer);
  },
  //渲染歌词
<text>{{lrc[time]}}</text>
```

#### 15.搜索歌曲做法

> 1.serach组件复用`<xsearchBar status="find"></xsearchBar> `
>
> 2.接收search`status`

```ruby
  properties: {
    status: String // 简化的定义方式
  },
===============================
  ready() {
    console.log(this.data.inputVal)
    if (this.data.status == "find") {
      this.setData({
        inputShowed: true	//显示取消和输入光标
      });
    } else {
      this.setData({
        inputShowed: false
      });
    }
  }
```

> 3.点击取消回到首页

```
 showInput: function () {
      wx.navigateTo({
        url: "/pages/find/find"
      })

```

> 4.输入文字发起ajax请求

```bash
 data: {
    inputShowed: false,
    inputVal: "",
    renderSong:[]
  },
    ===================================
    inputTyping: function (e) {
      this.searchSong(e.detail.value)	//执行搜索歌曲函数，传入输入框的`value`
      this.setData({
        inputVal: e.detail.value
      });
      
      console.log(this.data.inputVal)
    },
   ===========================================
   searchSong(keyword) {
      var self = this;
      wx.request({
        url: 'https://tingapi.ting.baidu.com/v1/restserver/ting', //仅为示例，并非真实的接口地址
        data: {
          method: "baidu.ting.search.catalogSug",
          query: keyword
        },
        header: {
          'content-type': 'application/json' // 默认值
        },
        success(res) {
          console.log(res.data)
          self.setData({
            renderSong: res.data.song ? res.data.song:""	//把得到的数据赋给本地变量
          })
          
          console.log(self.renderSong)
        }
      })
    },
```

#### 16.点击的时候把数据传到详情页

```bash
<navigator url="{{'/pages/detail/detail?songId='+item.songid}}" class="weui-cell" wx:for="{{renderSong}}" hover-class="weui-cell_active">
                <view class="weui-cell__bd">
                    <view>{{item.artistname}}-{{item.songname}}</view>
                </view>
 </navigator>
 备注：传songid到详情页 url="{{'/pages/detail/detail?songId='+item.songid}}"
```

