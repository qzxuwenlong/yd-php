# php-mysql
MySQL是一个 **关系型数据库管理系统**
mysql基本的增删改查
# php连接mysql
#### 最近时间匆忙，先记录一下以前没有注意到的点
* html表单请求php要在form 元素添加action="mysql.php"
* php增删改查 **传变量到sql语句时变量一定要加 ' 号例子:'"$name"'** </br>
`mysql-query("set name 'utf8'") //设置utf-8 ; //一般加到连接数据库的php里面 </br>
 $con =mysql_connect("localhost","root",""); //保存登录mysql的方法 </br>
 mysql_error(); //php操作mysql出现问题时，能看到哪里出错 </br>
 $mysql_select_db("数据库名",$con); //登录要登录那个数据库 在第一个参数据库名 </br>
 $rows=mysql_quer($sql,$con);  //发送请求数据 </br>
 while($row=mysql_fatch_array($rows)); //获取请求的数据 </br>
 echo $rot['字段名']; </br>
 $arr=array(); //保存一个数组 </br>
 array_push($arr,array("字段名"=>$rot['字段名'],"字段名1"=>$rot['字段名1'])); //转换成json，返回给前端，也是所谓的接口` </br>
![image](https://github.com/qzxuwenlong/php-mysql/blob/master/img/2bda0ee4ed6de97a49632e186b25b6f.png)
# php的pdo代码流程
![image](https://github.com/qzxuwenlong/php-mysql/blob/master/img/1562012658(1).png)
* 第一次见这函数，之前只是做简单的增删改查，
PHP 数据对象 （PDO） 扩展为PHP访问数据库定义了一个轻量级的一致接口。
PDO 提供了一个数据访问抽象层，这意味着，不管使用哪种数据库，都可以用相同的函数（方法）来查询和获取数据。
PDO随PHP5.1发行，在PHP5.0的PECL扩展中也可以使用，无法运行于之前的PHP版本。
 **这里的mysql是一个扩展的API，目的是为了简化php对mysql数据库的操作。**
 以下是基本操作方式
 ![image](https://github.com/qzxuwenlong/php-mysql/blob/master/img/pdo.png)
