# php学习
## 1、初识别php
php(外文名：PHP:Hypertext Preprocessor,“中文名超文本预处理器”)，是一种开源脚本与其他后台语言相比，**PHP是将程序嵌套到HTML(标准通用语言标记语言的下的一个应用)文档中去执行，执行效率比完全生成HTML标记的CGI要高许多；PHP还可以执行编译后的代码，编译可达到加密和优化代码运行，使代码运行更快**。
## 2、本章知识点
1、XAMPP启动后，新建的文件要在 _htdocs_ 目录下才可以被localhost(本地地址)下被访问到。/</br>
2、PHP变量是块级作用域，可以用 **isset($变量名)** 判断变量是否被声明。/</br>
3、PHP函数第一个参数可以缺省，可以设一个默认值但是不传($value=""),函数内要访问外部的变量必须要在函数内声明一下 **global $变量名**。
