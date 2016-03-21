email：邮件发送功能封装

依赖：该功能基于mail.jar封装，故需要引入mail.jar

使用方法： 
1。下载项目，打包成jar包 

2。在目标项目中引入mail.jar和步骤1打成的jar包 

3。在目标项目src目录下新建email.properties，
配置属性 
username=youremail@163.com 
password=pwd 
smtp=smtp.163.com 
defaultTitle=emailDefaultTitle 
emailName=emailName 
前三个为必须属性，后两个为可选属性 

4。在目标项目中调用：EmailService.send()方法即可


目标项目引用maven库：
<dependency>
	<groupId>javax.mail</groupId>
	<artifactId>mail</artifactId>
	<version>1.4.7</version>
</dependency>
<dependency>
	<groupId>com.bellevie</groupId>
	<artifactId>bellevie-mail</artifactId>
	<version>1.0</version>
</dependency>