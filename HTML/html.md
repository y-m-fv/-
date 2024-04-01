# 参考手册：W3school

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240331221210215.png" alt="image-20240331221210215" style="zoom:80%;" />

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240331221231984.png" alt="image-20240331221231984" style="zoom:67%;" />

------

> 属性可以用单引号，也可以用双引号

# 一、基础标签&样式

###### 1、排版

- ```
  <img>
  src:  rul
  width:  px像素/百分比
  height:  px像素/百分比
  ```

- ```
  标题标签:<h1>----<h6>
  ```

- ```
  水平线标签: <hr>
  ```

  <img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240331230933526.png" alt="image-20240331230933526" style="zoom:80%;" />

- ```
  用百分比的话，所占body也就是整个页面的80%
  ```

  ![image-20240331231432313](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240331231432313.png)

  - 案例
  - ![image-20240331231928424](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240331231928424.png)

![image-20240331231954174](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240331231954174.png)

------

###### 2、样式

> - 行内样式：内在标签内的style属性中
>
>   内嵌样式：写在style标签中
>
>   外联样式：写在一个单独的.css中

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401111747272.png" alt="image-20240401111747272" style="zoom:80%;" />

```
css样式文件⬇
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401111847317.png" alt="image-20240401111847317" style="zoom:80%;" />

- 颜色表示形式

  > 关键字
  >
  > rgb
  >
  > 十六进制

![image-20240401113701582](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401113701582.png)

------

- css选择器、span标签、css属性

  > 元素选择器
  >
  > id选择器
  >
  > 类选择器
  >
  > 此三种选择器优先级为：**id > 类 > 元素**

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401115308622.png" alt="image-20240401115308622" style="zoom:80%;" />

------

###### 3、超链接

- ```
  <a href="·······" target="······"></a>
  target：表示在何处打开资源
  	_self:默认值，在当前页面打开
  	_blank:在空白页面打开
  ```

​		![image-20240401121059145](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401121059145.png)

- ```
  a标签的css属性
  text-dectoration：规定添加到文本的修饰，none表示定义标准的文本
  color: 定义文本颜色
  ```

  <img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401121313015.png" alt="image-20240401121313015" style="zoom:80%;float:left" />

###### 4、标签

- ```
  视频标签：video
  音频标签：audio
  同时必须要把controls控件属性添加上
  ```

  <img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401123831055.png" alt="image-20240401123831055" style="zoom:;float:left" />

- ```
  换行：<br>
  段落：<p>
  ```

- ```
  文本加粗：
  <b>   <strong>(这个带有强调语义)
  ```

- ```
  css样式：
  line-height：设置行高
  text-indent：定义第一个行内容的缩进
  text-align：规定元素中的文本的水平对齐方式
  可以使用&nbsp空格占位符
  ```

###### 5、布局

- **盒子模型**

  ```
  div标签
  一行占一个，可设置宽高
  span标签
  一行多个，不可以设置宽高
  
  css盒子模型：
  由内容（content）、内边距（padding）、边框（birder）、外边距（margin）
  css属性：
  width：宽度
  height：高度
  border：边框属性//上 右 下 左
  margin：外边框属性//上 右 下 左
  若只需要设置某一个方位的边框和内外边距，可在属性名后面加上  -位置，例如margin-left、border-top
  ```

  ![image-20240401172257231](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401172257231.png)

------

# 二、表格标签

```
<table>:包裹多个<tr>
		border:表格边框宽度
		width：表格的宽度
		cellspacing：单元格之间的空间
<tr>：包裹多个<td>
<td>:如果是表头单元格，可以替换为<th>
```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401174328122.png" alt="image-20240401174328122" style="zoom:67%;float:left" margin-left="0"/>![image-20240401174627584](C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401174627584.png)

------

# 三、表单表格

> ```
> form标签
> 属性：
> action：规定当提交表单时向何处发送表单数据，默认为当前页面。URL
> method：规定用于发送表单数据的方式。GET、PSOT
> 		GET：在url后面拼接表单数据，同时url长度会有限制。?username=Tom&age=12（消息体）
> 		POST：在消息体（请求体）中传递的，参数大小无限制
> ```

<img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401180441022.png" alt="image-20240401180441022" style="zoom:67%;float:left" /><img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401180424582.png" alt="image-20240401180424582" style="zoom:80%;" />

- **表单项**

  ```
  表单项：
  <input>:定义表单项，通过type属性控制输入形式
  <select>:定义下拉列表
  <textarea>:定义文本域
  ```

  <img src="C:\Users\fbb\AppData\Roaming\Typora\typora-user-images\image-20240401182703757.png" alt="image-20240401182703757" style="zoom:80%;" />
