DaoSupport
==========
J2EE  Dao的支持方案，减轻小项目开发使用传统mvc时,dao重复且编写枯燥问题。
通过xml 和 java 的反射机制制作的 Dao封装类,在配好xml 之后只需要这一个Dao的实现类（EntityDaoImpl）就可以实现基本的对数据库的增删改查.


额外需要导入的包如下：
    
 	mysql的连接包：mysql-connector-java-5.1.13-bin.jar
 	解析xml 的包 ：dom4j-1.6.1.jar

 后续将推出注解版本.
 注解版本进度50%
 

 
 UPDATE LOG:
 	9月16 添加对 EntityDao的批量保存处理(预处理)
 	

    12月2号 除去了jdk7 switch(string)的特性
            添加java.util.logging,日志配置可配置在classpath中，但是名字必须为DaoSupport.properties，比如将日志信息输出到文件中。
            无配置就不需要去关注。
