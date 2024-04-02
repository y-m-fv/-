# js引入方式

###### 1、内部脚本

> js必须位于<script></script>标签之间
>
> 同时script可以放置任意位置、任意数量
>
> 一般放置body元素的底部，改善显示速度



###### 2、外部脚本

```
将js代码定义在js文件中，然后引入html文件
```

> 外部js文件，只包含js代码，不包含script标签
>
> script不能自闭合   //，<script src=""/>（×）

# js基础语法

###### 1、书写语法

> 区分大小写
>
> 每行结尾的分号可有可无

```
window.alert()：写入警告框
document.write()：写入HTML输出
console.log()写入浏览器控制台
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401204817780.png" alt="image-20240401204817780" style="zoom:67%;float:left" />

###### 2、变量

> js中用  var  关键字来申明变量
>
> js是一门弱类型语言，变量可以存放不同类型的值
>
> 变量名遵循规则：
>
> ​			字母、数字、下划线或$
>
> ​			数字不能开头
>
> ​			建议使用驼峰命名

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401210215298.png" alt="image-20240401210215298" style="zoom:80%;" />

###### 3、数据类型

> number:数字
>
> string：字符串，单双引皆可
>
> Boolean：布尔
>
> null：对象为空
>
> undefined：当声明的变量为初始化，该变量的默认值为undefined

![image-20240401210930553](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401210930553.png)

###### 4、运算符

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401213153509.png" alt="image-20240401213153509" style="zoom:80%;" />

```
js中流程语句也支持
```

# 函数

```
function functionName(参数1，参数2.....){//要执行的代码}
形参不需要类型，因为js是弱类型语言
返回值也不需要类型，可以在函数内部直接使用return返回即可
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401220716081.png" alt="image-20240401220716081" style="zoom:;float:left" />![image-20240401220743643](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401220743643.png)



```
方式二
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401221201668.png" alt="image-20240401221201668" style="zoom:;float:left" />![image-20240401221232939](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401221232939.png)

# js对象

> array、string、JSON、BOM、DOM

###### 1、array

定义数组

- 定义

  > var 变量名 = new Array(元素列表); //方式一
  >
  > ​					var arr = new Array(1,2,3,4);
  >
  > var 变量名 = [元素列表]; 方式二
  >
  > ​					var arr = [1,2,3,4];

- 访问

  > arr[索引] = 值;                         arr[10] = "hello";    

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401223104908.png" alt="image-20240401223104908" style="zoom:;float:left" />![image-20240401223130888](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401223130888.png)

















------

- 属性

  > length

  - <img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401223622842.png" alt="image-20240401223622842" style="zoom:;float:left" />![image-20240401223656704](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401223656704.png)



- 方法

  > forEach()、push()、splice()

​		![image-20240401224714787](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401224714787.png)![image-20240401224727801](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401224727801.png)

###### 2、string

![image-20240401225625606](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401225625606.png)

------

![image-20240401230639937](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401230639937.png)![image-20240401230608113](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401230608113.png)

###### 3、json

```
var 对象名 = {                                    var user = {
	属性名:属性值1,                                    name:"Tom",
	属性名:属性值2,                                    age:20,
	属性名:属性值3,                                    gender:"male",
	函数名称:function(形参列表){}                       eat:function() {alert("用膳~");}
}                                                }
```

```
调用格式：
对象名.属性名;         console.log(user.name);
对象名.函数名();       user.eat();
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402103222184.png" alt="image-20240402103222184" style="zoom:67%;" />

```
JSON:
var userStr = '{"name":"Jerry","age":18,"addr":["北京","上海","西安"]}';

value的数据类型：
数字(整数或浮点数)
字符串(在双引号中)
逻辑值(true 或 false)
数组(在方括号中)
对象(在花括号中)
null

JSON字符串转为JS对象
	var jsObject = JSON.parse(userStr)
JS对象转为JSON字符串
	var jsonStr = JSON.stringify(jsObject);
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402105051617.png" alt="image-20240402105051617" style="zoom:80%;float:left" />

###### 4、BOM

> window：浏览器窗口对象  √
>
> navigator：浏览器对象
>
> screen:屏幕对象
>
> history：历史记录对象
>
> location：地址栏对象  √

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402110509442.png" alt="image-20240402110509442" style="zoom:80%;" />

------

![image-20240402112418139](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402112418139.png)

------

![image-20240402112436343](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402112436343.png)

###### 5、DOM

![image-20240402114154211](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402114154211.png)

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402114241967.png" alt="image-20240402114241967" style="zoom:67%;" />

------

```
根据id属性获取，返回单个element对象
	var h1 = document.getElementById('h1');
根据标签名称获取，返回element对象数组
	var divs = document.getElementsByTagName('divs');
根据name属性值获取，返回Element对象数组
	var hobbys = document.getElementByName('hobby');
根据class属性值获取，返回element对象数组
	var class = document.getElementByClassName('cls');
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402121148739.png" alt="image-20240402121148739" style="zoom:80%;float:left" /><img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402121218727.png" alt="image-20240402121218727" style="zoom:80%;" />

------

> 小案例

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402154408115.png" alt="image-20240402154408115" style="zoom:80%;float:left" />![image-20240402154430164](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402154430164.png)









###### 6、js事件监听

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402154640001.png" alt="image-20240402154640001" style="zoom:67%;float:left" /><img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402155448241.png" alt="image-20240402155448241" style="zoom:67%;" />













![image-20240402155519781](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240402155519781.png)

> 案例：16
