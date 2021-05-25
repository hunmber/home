**1、html结构**

HTML的结构包括头部（Head）、主体（Body）两大部分，其中头部描述浏览器所需的信息，而主体则包含所要说明的具体内容。

< !DOCTYPE html> 用于文档声明，告诉浏览器文件用哪个版本的html解析。
< html> html限定了文档的开始与结束点
< head>
< title>Title< /title> 标题词一般夹在 < head > 与< /head > 中间
< /head>
< body >
正文则夹在< body >和< /body >之间
< /body >
< /html>

**2、字体**

1、字体用< font > 标签
color用来改变颜色，size表示大小，+3增大3号，-3减小3号
如：< font color=“red” size=“3” >text!< /font >

2、给字体加粗
< strong >
如：< strong >字体< /strong>

3、斜体
< em >

4、删除效果
< del >

5、下划线
< ins >

**3、标题**
用< h1 >设置标题，默认居左，一般会使用< h1> 到 < h6> 分别表示不同大小的标题
< h1 >这是一个标题< /h1 >
若要设置标题位置，用align属性，居中：align=“center”。
如< h1 align=“center”>这是一个标题< /h1 >

**4、图片**
< img > 图像标签
需要设置其属性src来指定图像的路径。
如：< img src=“http://how2j.cn/example.gif”/>

1、如果是本地文件，只需把图片放在同一个目录下即可
src直接使用文件名，不需要/

2、src使用图片所在的绝对路径，并在前面加上file://，后边需要加/

3、用width和height来设置图片的大小

4、加上alt属性，在图片不存在时会显示alt中的文字，alt=“这个是一个图片”。

**5、超链接**
1、通过< a>标签进行超链接，href中为超链接的地址，百度一下为超链接的本地文字
< a href=“http://www.baidu.com”>百度一下< /a>

2、使用图片进行超链接，只需要将图片嵌套入< a >标签中

**6、表格**
< table>标签用于显示一个表格
< tr> 表示行
< td> 表示列又叫单元格

1、使用属性 border=“1” 能使表格加上边框
< table border=“1” width=“200px”> < /table>

2、设置td的属性colspan，能使表格水平合并
< td colspan=“2” >1，2< /td>

3、设置td的属性rowspan，能使表格垂直合并
< td rowspan=“2”>1,3< /td>

4、设置属性bgcolor，能给表格加上背景颜色
< tr bgcolor=“gray”>

5、< ul >实现无序表
< ul >
< li>DOTA< /li>
< li>LOL< /li>
< /ul >
< ol >实现有序表
< ol>
< li>地卜师< /li>
< li>卡尔< /li>
< /ol>

**7、内联框架**
< iframe > 即内联框架

通过内联框架 可以实现在网页中“插入”网页

**8、表单**
1、< input type=“text”> 即表示文本框

2、< input type=“password”> 即表示密码框

3、< input type=“radio” > 表示单选框

4、< input type=“checkbox”> 即表示复选框

5、< select> 即下拉列表
需要配合< option>使用

6、< textarea> 即文本域
与文本框不同的是，文本域可以有多行，并且可以有滚动条

7、< input type=“submit”> 即为提交按钮
用于提交form，把数据提交到服务端

8、< input type=“image” > 即使用图像作为按钮进行form的提交、

9、< form action=“http://how2j.cn/study/login.jsp” method=“get”>
账号：< input type=“text” name=“name”> < br/>
密码：< input type=“password” name=“password” > < br/>
< input type=“submit” value=“登陆”>
< /form>
属性action中为要提交到的网站，method表示提交的方法，方法有get与post。
submit通过按钮提交

get
get是form默认的提交方式
提交数据会在浏览器显示出来
不可以用于提交二进制数据，比如上传文件
post
post必须在form上通过 method=“post” 显示指定
提交数据不会在浏览器显示出来
可以用于提交二进制数据，比如上传文件