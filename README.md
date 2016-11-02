
# javascript 

标签（空格分隔）： js 
---

##JS事件

| 事件        | 描述   |
| --------   | -----  |
| onclick     | 用户点击 HTML 元素 |
| onload        |  浏览器已完成页面的加载  | 
| onmouseover        |    用户在HTML元素上移过   |
| onmouseout        |    用户从一个HTML元素上移开鼠标 |
| onkeydown        |    用户按下键盘按键 |
| onchange |   HTML元素改变  |

##JS数据类型
> string 字符串
> number 数字
> boolean 布尔
> array 数组
> object 对象
> null 空
> undefined  未定义

##变量名
> 1.变量必须使用字母、下划线(_)或者美元符($)开始。

> 2.然后可以使用任意多个英文字母、数字、下划线(_)或者美元符($)组成。

> 3.不能使用JavaScript关键词与JavaScript保留字。

##函数
```js
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>函数调用</title>
   <script type="text/javascript">
   function contxt() //定义函数
      {
         alert("哈哈，调用函数了!");
      }
   </script>
</head>
<body>
   <form>
      <input type="button"  value="点击我" onclick=" contxt()   " />  
   </form>
</body>
</html>
```
##JavaScript-确认（confirm 消息对话框）
> confirm(str);

```js
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>confirm</title>
  <script type="text/javascript">
  function rec(){
    var mymessage= confirm ("你是女士吗？");
    if(mymessage==true)
    {
    	document.write("你是女士!");
    }
    else
    {
        document.write("你是男士!");
    }
  }    
  </script>
</head>
<body>
    <input name="button" type="button" onClick="rec()" value="点击我，弹出确认对话框" />
</body>
</html>
```

###JavaScript-提问（prompt 消息对话框）
```js
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>prompt</title>
  <script type="text/javascript">
  function rec(){
	var score; //score变量，用来存储用户输入的成绩值。
	score = 150;
	if(score>=90)
	{
	   document.write("你很棒!");
	}
	else if(score>=75)
    {
	   document.write("不错吆!");
	}
	else if(score>=60)
    {
	   document.write("要加油!");
    }
    else
	{
       document.write("要努力了!");
	}
  }
  </script>
</head>
<body>
    <input name="button" type="button" onClick="rec()" value="点击我，对成绩做评价!" />
</body>
</html>
```
### className
object.className=classname
```js
function add(){
 var text= document.getElementById("text");
 text.className="one";
}
```
> add():    onclick="add()";
> var：定义一个名为text的变量，获取到dom中ID为text的元素，然后将它的class改为.one

#学习小结
```js
function list(){
   var txt= confirm("你确定要出发吗？");
    if (txt==true){
        document.write("加油");
    } 
    else{
        document.write("看看其它吧");
    }
}
<a href="#" onclick="list()">点击</a>
```













