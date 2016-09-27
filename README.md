# struts2exec
Struts2 的一个综合练习

# 数据库设计

## 新建数据库
create database struts2exec;

## 用户表
CREATE TABLE S_User(
	userID INT  NOT NULL AUTO_INCREMENT, #主键ID
	userName VARCHAR(50)   NULL,  #用户姓名
	loginName VARCHAR(50)   NULL, #登录名
	loginPwd VARCHAR(50)  NULL,   #密码#
	sex VARCHAR(10)  NULL,        #性别（例如：男，女）
	birthday VARCHAR(50) NULL,    #出生日期
	education VARCHAR(20)  NULL,  #学历（例如：研究生、本科、专科、高中）
	telephone VARCHAR(50)  NULL,  #电话 
	interest VARCHAR(20)  NULL,   #兴趣爱好（例如：体育、旅游、逛街）
	path VARCHAR(500)  NULL,      #上传路径（path路径）
	filename VARCHAR(100)  NULL,  #上传文件名称（文件名）
	remark VARCHAR(500)  NULL,    #备注
	PRIMARY KEY (userID)
);

## 初始化数据：默认用户名和密码是admin
INSERT INTO s_user (userID,userName,loginName,loginPwd) VALUES (1,'超级管理员','admin','admin');\

# 搭建开发环境
struts2 + javabean + DAO + C3P0 + DBUtils + MySQL<br/>
	asm-3.3.jar
	asm-commons-3.3.jar
	asm-tree-3.3.jar
	c3p0-0.9.5.2.jar
	commons-dbutils-1.6.jar
	commons-fileupload-1.3.1.jar
	commons-io-2.2.jar
	commons-lang3-3.2.jar
	freemarker-2.3.22.jar
	javassist-3.11.0.GA.jar
	log4j-api-2.3.jar
	log4j-core-2.3.jar
	mysql-connector-java-5.1.39-bin.jar
	ognl-3.0.13.jar
	struts2-core-2.3.28.jar
	xwork-core-2.3.28.jar
