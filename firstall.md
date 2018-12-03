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

######  1.margin取值:遵循上右下左原则，缺省的值找反义词的值

######  2.margin-方位

######  3.注意：margin可以为负值

# 第六天

# 一、元素类型

##   (一) 块级元素

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

##  三、命名锚点

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

##  一、宽高自适应

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

###         (一) html表单标签

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

####  1.边框阴影box-shadow

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



##    三、过渡 transition  过渡：让变化在一段时间内进行

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

###  （一）自定义动画 

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