正则：
\d 数字
\D 非数字
\w 字母 数字 下划线
\W 非字母 数字 下划线
\s 空白字符
\S 非空白字符

* 多次（包含0）
+ 多次 (不包含0)
？ 最多出现一次
{n} 出现n次
{n,m} 出现n到m次
{n,} 至少出现n次


[]范围
[abc123] 匹配abc123任意字符
[a-z0-9] 匹配a到z 0到9

^开始
$结束

HTML 页面结构
CSS 页面表现
JavaScript 页面行为

JavaScript 是运行在浏览器中的脚本，由浏览器解释执行

嵌入javascript方式
<script type="text/javascript">
	$(document).ready(function() {
		alert("test")
	})
</script>

<script type="text/javascript" src="jquery-1.12.4.js"></script>

类型 5中基本类型 1种复合类型
number string boolean undefined null
object 

document内置对象 可以通getElementById 获取元素
脚本执行由上至下，获取位于脚本之后的元素使用 window.onload = function()


函数
JavaScript解析过程分为两个阶段，1.编译阶段，2.执行阶段，在编译阶段会将function定义的函数提前，并且将var定义的变量声明提前

数组
定义：
1 var aList = new Array(1,2,3)
2 var aList = [1,2,3]

数组中的元素类型可以不同

定时器

setTimeout（）执行一次的定时器
clearTimeout() 清除定时器
setInterval() 反复执行的定时器
clearInterval() 关闭反复执行的定时器

封闭函数
封闭函数是javascript中匿名函数的一种，创建一个开始就执行的函数

(匿名函数)
～匿名函数
！匿名函数

JQuery是目前使用最广泛的javascript函数库，JQuery的版本分为1.x，
2.x，3.x 其中1.x版本支持低版本浏览器，使用最广泛

JQuery是一个js文件，函数库

Write Less，Do More

window.onload 可以简写为以下两种方式

$(document).ready(function() {
	//do something
})

$(function() {
	//do something
})

选择器
$("#div") select elements which id is "div"
$(".div_class") select elements which class is "div_class"
$("li") select elements whose tag is 'li'


operate style

$("#div").css('width','30px')
$("#div").css({width: '30px', height: '30px'})


click event
$("#btn1").click(function() {
	
})

get html 

var htmlValue = $("#div1").html()
$("#div1").html('this is a div')

loop

$('.list li').each(function() {
	
})

事件委托

$("#list li").click(function() {
	$(this).css({background: 'red'})
})


$("#list").delegate('li', 'click', function() {
	$(this).css({background: 'red'})
})


json 是 JsonScript Object Notation 简写

{
	name: 'tom',
	age: '16',
	getName: function() {
		return name
	} 
}

{
	"name": "tom",
	"age": "16",
}



ajax技术目的是javascript发送http请求，本质上是通过实例化xmlHttp对象，使用此对象与后台通信，ajax请求的页面或者资源只能是同一个域下面的资源（这是当时基于安全考虑）,需要跨域请求使用jsonp，JQuery对这两种方式进行了封装



cookie 存储在本地，容量大小为最大4k








