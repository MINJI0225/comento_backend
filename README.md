# comento_backend

## 1차 과제 _ 개발환경 구성
##### 버전 정보 :  jdk 11, eclipse 2021-12
### 문제
##### 1. Error while downloading 'http://www.springframework.org/schema/context/spring-context-3.0.xsd' to C: \Users\minji\.lemminx\cache\http\www.springframework.org\schema\context\spring-context-3.0.xsd
##### 해결: <root-context.xml> beans 수정
##### 2.DB 연결 오류
##### 해결: <root-context.xml> dataSource url, username, password 수정
### 결과
<img width="80%" src="https://user-images.githubusercontent.com/69569367/183076403-8b84ca71-bba3-4618-9e81-408385fdbe1e.PNG"/>

## 2차 과제 _ API 가이드 문서 작성
##### https://highfalutin-oak-86d.notion.site/SW-API-8b1abc31578f4a74a895e9834ab8de81

## 3차 과제 - REST API 구현
### 결과
<img width="80%" src="https://user-images.githubusercontent.com/69569367/184357718-1b33af5c-af8c-40fe-a05b-0ee94a9b581b.PNG"/>
<img width="80%" src="https://user-images.githubusercontent.com/69569367/184357975-92c99746-c889-495b-a01b-13003781515a.PNG"/>

#### 문제
##### 1. Project를 Maven build로 실행할 경우 사이트에 연결할 수 없음. localhost에서 연결을 거부했습니다. 결과 페이지가 떴음
해결: SettingwebBootApplication.java로 project를 실행

##### 질문: spring boot version 문제
pom.xml에서 2.2.2.RELEASE로 바꾸려고 시도하였으나,   
Multiple markers at this line
- Non-resolvable parent POM for com.devfun:settingweb_boot:0.0.1-SNAPSHOT: org.springframework.boot:spring-boot-starter-parent:pom:2.2.2.RELEASE was not found in https://repo.maven.apache.org/maven2 during a previous attempt. This failure was cached in the local repository and resolution is not reattempted until the update interval of central has elapsed or updates are forced
- Project build error: Non-resolvable parent POM for com.devfun:settingweb_boot:0.0.1-SNAPSHOT: org.springframework.boot:spring-boot-starter-parent:pom:2.2.2.RELEASE was not found in https://repo.maven.apache.org/maven2 during a previous attempt. This failure was cached in the local repository and resolution is not reattempted until the update interval of central has elapsed or updates are forced and 'parent.relativePath' points at no local POM    
(project 실행에는 문제가 없지만 해결방법이 궁금함)
