# springbootJsp

#### 项目介绍
自己的springboot项目 + jsp开发
#### 访问首页
http://localhost:8080/springJSP

###启动
启动tomcat

###说明
1、spring boot自带了 tomcat,并且不用打成war包再执行,直接通过jar包即可执行，
         要想使用jsp，需要单独配置一个外部tomcat，需要打war包，所以在新建项目时，勾选"war"包
    pom.xml多了
         
         <dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-tomcat</artifactId>
			<scope>provided</scope>
		</dependency>
		
		即打jar包的时候，不再加入 tomcat
2、建立web项目目录
	在 src/main目录下建立webapp/WEB-INF
	src/main目录下建立webapp/index.jsp 等等
	
3、在application.properties文件配置
spring.mvc.view.prefix=/
spring.mvc.view.suffix=.jsp

4、在控制器中建立方法,访问jsp视图文件
