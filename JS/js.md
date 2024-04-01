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

2、string

![image-20240401225625606](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401225625606.png)

------

![image-20240401230639937](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401230639937.png)![image-20240401230608113](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401230608113.png)





