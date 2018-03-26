1.在原工程的基础上,pom.xml中添加如下两个配置
			<!-- 配置Tomcat插件 -->
			<plugin>
				<groupId>org.apache.tomcat.maven</groupId>
				<artifactId>tomcat7-maven-plugin</artifactId>
				<configuration>
					<port>8095</port>
					<path>/</path>
				</configuration>
			</plugin>
			
			<!-- java编译插件 -->
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-compiler-plugin</artifactId>
				<version>3.2</version>
				<configuration>
					<source>1.7</source>
					<target>1.7</target>
					<encoding>UTF-8</encoding>
				</configuration>
			</plugin>

2.在pom.xml中导入对应的依赖
		<!-- freemarker集成shiro标签 -->
		<dependency>
			<groupId>net.mingsoft</groupId>
			<artifactId>shiro-freemarker-tags</artifactId>
			<version>0.1</version>
		</dependency>
		
		<!-- 自动生成getter和setter -->
		<dependency>
			<groupId>org.projectlombok</groupId>
			<artifactId>lombok</artifactId>
			<version>1.16.18</version>
			<scope>provided</scope>
		</dependency>
		
3.在BaseDao中修改delete方法为deletepk，并修改对应的dao.xml文件和service类

4.在eclipse的解压文件或者在eclipse的安装目录中找到eclipse.ini文件，在同级目录下添加lombok.jar，并在eclipse.ini最后添加
-javaagent:lombok.jar
-Xbootclasspath/a:lombok.jar 

5.重启eclipse update工程

6.将WxPayForParking.java注释即可

7.启动工程，访问地址localhost:8095

8.后台系统界面地址
#不带项目名
http://localhost:8095/hqc_mp/octopus/sys/index.html
#带项目名 
http://localhost:8095/octopus/sys/index.html
用户名/密码：admin/admin

9.banner相关的数据库表是
mp_banner
