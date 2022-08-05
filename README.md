# comento_backend

# 1차 과제 _ 개발환경 구성
###jdk 11
###eclipse 2021-12
##문제
###<root-context.xml>
####1. Error while downloading 'http://www.springframework.org/schema/context/spring-context-3.0.xsd' to C:
 \Users\minji\.lemminx\cache\http\www.springframework.org\schema\context\spring-context-3.0.xsd
#### 해결: <beans xmlns="http://www.springframework.org/schema/beans"
	xmlns:context="http://www.springframework.org/schema/context"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://www.springframework.org/schema/beans https://www.springframework.org/schema/beans/spring-beans.xsd
	http://www.springframework.org/schema/context http://www.springframework.org/schema/context/spring-context.xsd">
####2. DB 연결 오류
#### 해결: dataSource url, username, password 수정
##결과
https://github.com/MINJI0225/comento_backend/issues/1#issue-1329869292

# 2차 과제 _ 
