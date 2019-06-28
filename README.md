# php学习
## 一、初识别PHP
php(外文名：PHP:Hypertext Preprocessor,“中文名超文本预处理器”)，是一种开源脚本与其他后台语言相比，**PHP是将程序嵌套到HTML(标准通用语言标记语言的下的一个应用)文档中去执行，执行效率比完全生成HTML标记的CGI要高许多；PHP还可以执行编译后的代码，编译可达到加密和优化代码运行，使代码运行更快**。
### 1、本章知识点
1、XAMPP启动后，新建的文件要在 _htdocs_ 目录下才可以被localhost(本地地址)下被访问到。</br>
2、PHP变量是块级作用域，可以用 **isset($变量名)** 判断变量是否被声明。</br>
3、PHP函数第一个参数可以缺省，可以设一个默认值但是不传($value=""),函数内要访问外部的变量必须要在函数内声明一下 **global $变量名**。</br>
## 二、PHP基础操作
### 1、本章知识点
1、**$GLOBALS['variable']='值'** 在A.php声明，B.php用( **require_once(A.php)** 或 **include_once.php(A.php)** )引用A.php时,可在B.php文件中使用。</br>
2、require_once(A.php);与include_once.php(A.php);区别:include_once.php(),在引用错php时如include_once.php(AB.php);会报错但是后面的代码还是会执行，而require_once();会报错，但是后面的代码不会执行。</br>
3、PHP里面的数组要用这种格式 **$arrayTest=array('name'=>'测试','upwd'=>'123');** 这种格式，输出时 **echo json_encode($arrayTest)** 。</br>
4、session是一中会话机制，一般用在登录多，当登录后会把用户id存到session中，当访问网站别的页面时会判断用户是否登录，如果没有则显示未登录，有的话执行用户的操作。
5、session用法，每次使用时要先 执行**session_start()** 这个函数 **$_SESSION['字段名']='前端传过来的值'** 记录到session,下一步当用户跳转到网站别的页面是，把cooies的值传到php与session['字段名']中的值做比较。<br>
6、PHP接受前端传过来的值得方法 **$_POST['字段名']或$_REQUEST['字段名']** $_POST只能接受post请求方式，而$_REQUEST什么类型都可以接收。</br>
![image](https://github.com/qzxuwenlong/yd-php/blob/master/images/ajax.png)</br>
7、PHP echo值有汉字时要在php文件加上 `header("Content-type:application/json;charset=utf-8");`。</br>
![image](https://github.com/qzxuwenlong/yd-php/blob/master/images/php.png)</br>
