---
layout: post
title: 搭建SpringMVC-Freemarker-Tomcat环境 二
category: opinion
description: 搭建SpringMVC-Freemarker-Tomcat环境 二
---

##在Tomcat中配置Spring MVC+Freemarker

首先在pom.xml中添加相关依赖
```
	<dependencies>
		<dependency>
			<groupId>org.springframework</groupId>
			<artifactId>spring-context</artifactId>
			<version>3.2.4.RELEASE</version>
		</dependency>
		<dependency>
			<groupId>org.springframework</groupId>
			<artifactId>spring-aop</artifactId>
			<version>3.2.4.RELEASE</version>
		</dependency>
		<dependency>
			<groupId>org.springframework</groupId>
			<artifactId>spring-webmvc</artifactId>
			<version>3.2.4.RELEASE</version>
		</dependency>
		<dependency>
			<groupId>org.springframework</groupId>
			<artifactId>spring-web</artifactId>
			<version>3.2.4.RELEASE</version>
		</dependency>
		<dependency>
			<groupId>org.springframework</groupId>
			<artifactId>spring-context-support</artifactId>
			<version>3.2.4.RELEASE</version>
		</dependency>

		<dependency>
			<groupId>org.freemarker</groupId>
			<artifactId>freemarker</artifactId>
			<version>2.3.20</version>
		</dependency>
	</dependencies>
```
不同Spring版本会存在配置上的差异，本文以Spring3.2.4和freemarker2.3.20为标准来进行项目构建
在pom.xml添加完依赖之后，等待依赖下载完毕。

接着在web.xml中添加如下
   
	