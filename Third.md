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

