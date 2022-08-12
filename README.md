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
#### 사이트에 연결할 수 없음. localhost에서 연결을 거부했습니다. 결과 페이지가 뜸.
##### console
```xml
[INFO] Scanning for projects...
[INFO] 
[INFO] ---------------------< com.devfun:settingweb_boot >---------------------
[INFO] Building settingweb_boot 0.0.1-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:3.2.0:resources (default-resources) @ settingweb_boot ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] Copying 1 resource
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.10.1:compile (default-compile) @ settingweb_boot ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 7 source files to C:\Users\minji\eclipse-workspace\settingweb_boot\target\classes
[INFO] 
[INFO] --- maven-resources-plugin:3.2.0:testResources (default-testResources) @ settingweb_boot ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Using 'UTF-8' encoding to copy filtered properties files.
[INFO] skip non existing resourceDirectory C:\Users\minji\eclipse-workspace\settingweb_boot\src\test\resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.10.1:testCompile (default-testCompile) @ settingweb_boot ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to C:\Users\minji\eclipse-workspace\settingweb_boot\target\test-classes
[INFO] 
[INFO] --- maven-surefire-plugin:2.22.2:test (default-test) @ settingweb_boot ---
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.devfun.settingweb_boot.SettingwebBootApplicationTests
21:17:01.829 [main] DEBUG org.springframework.test.context.BootstrapUtils - Instantiating CacheAwareContextLoaderDelegate from class [org.springframework.test.context.cache.DefaultCacheAwareContextLoaderDelegate]
21:17:01.846 [main] DEBUG org.springframework.test.context.BootstrapUtils - Instantiating BootstrapContext using constructor [public org.springframework.test.context.support.DefaultBootstrapContext(java.lang.Class,org.springframework.test.context.CacheAwareContextLoaderDelegate)]
21:17:01.899 [main] DEBUG org.springframework.test.context.BootstrapUtils - Instantiating TestContextBootstrapper for test class [com.devfun.settingweb_boot.SettingwebBootApplicationTests] from class [org.springframework.boot.test.context.SpringBootTestContextBootstrapper]
21:17:01.920 [main] INFO org.springframework.boot.test.context.SpringBootTestContextBootstrapper - Neither @ContextConfiguration nor @ContextHierarchy found for test class [com.devfun.settingweb_boot.SettingwebBootApplicationTests], using SpringBootContextLoader
21:17:01.926 [main] DEBUG org.springframework.test.context.support.AbstractContextLoader - Did not detect default resource location for test class [com.devfun.settingweb_boot.SettingwebBootApplicationTests]: class path resource [com/devfun/settingweb_boot/SettingwebBootApplicationTests-context.xml] does not exist
21:17:01.926 [main] DEBUG org.springframework.test.context.support.AbstractContextLoader - Did not detect default resource location for test class [com.devfun.settingweb_boot.SettingwebBootApplicationTests]: class path resource [com/devfun/settingweb_boot/SettingwebBootApplicationTestsContext.groovy] does not exist
21:17:01.927 [main] INFO org.springframework.test.context.support.AbstractContextLoader - Could not detect default resource locations for test class [com.devfun.settingweb_boot.SettingwebBootApplicationTests]: no resource found for suffixes {-context.xml, Context.groovy}.
21:17:01.928 [main] INFO org.springframework.test.context.support.AnnotationConfigContextLoaderUtils - Could not detect default configuration classes for test class [com.devfun.settingweb_boot.SettingwebBootApplicationTests]: SettingwebBootApplicationTests does not declare any static, non-private, non-final, nested classes annotated with @Configuration.
21:17:01.999 [main] DEBUG org.springframework.test.context.support.ActiveProfilesUtils - Could not find an 'annotation declaring class' for annotation type [org.springframework.test.context.ActiveProfiles] and class [com.devfun.settingweb_boot.SettingwebBootApplicationTests]
21:17:02.112 [main] DEBUG org.springframework.context.annotation.ClassPathScanningCandidateComponentProvider - Identified candidate component class: file [C:\Users\minji\eclipse-workspace\settingweb_boot\target\classes\com\devfun\settingweb_boot\SettingwebBootApplication.class]
21:17:02.115 [main] INFO org.springframework.boot.test.context.SpringBootTestContextBootstrapper - Found @SpringBootConfiguration com.devfun.settingweb_boot.SettingwebBootApplication for test class com.devfun.settingweb_boot.SettingwebBootApplicationTests
21:17:02.302 [main] DEBUG org.springframework.boot.test.context.SpringBootTestContextBootstrapper - @TestExecutionListeners is not present for class [com.devfun.settingweb_boot.SettingwebBootApplicationTests]: using defaults.
21:17:02.303 [main] INFO org.springframework.boot.test.context.SpringBootTestContextBootstrapper - Loaded default TestExecutionListener class names from location [META-INF/spring.factories]: [org.springframework.boot.test.mock.mockito.MockitoTestExecutionListener, org.springframework.boot.test.mock.mockito.ResetMocksTestExecutionListener, org.springframework.boot.test.autoconfigure.restdocs.RestDocsTestExecutionListener, org.springframework.boot.test.autoconfigure.web.client.MockRestServiceServerResetTestExecutionListener, org.springframework.boot.test.autoconfigure.web.servlet.MockMvcPrintOnlyOnFailureTestExecutionListener, org.springframework.boot.test.autoconfigure.web.servlet.WebDriverTestExecutionListener, org.springframework.boot.test.autoconfigure.webservices.client.MockWebServiceServerTestExecutionListener, org.springframework.test.context.web.ServletTestExecutionListener, org.springframework.test.context.support.DirtiesContextBeforeModesTestExecutionListener, org.springframework.test.context.event.ApplicationEventsTestExecutionListener, org.springframework.test.context.support.DependencyInjectionTestExecutionListener, org.springframework.test.context.support.DirtiesContextTestExecutionListener, org.springframework.test.context.transaction.TransactionalTestExecutionListener, org.springframework.test.context.jdbc.SqlScriptsTestExecutionListener, org.springframework.test.context.event.EventPublishingTestExecutionListener]
21:17:02.337 [main] INFO org.springframework.boot.test.context.SpringBootTestContextBootstrapper - Using TestExecutionListeners: [org.springframework.test.context.web.ServletTestExecutionListener@68044f4, org.springframework.test.context.support.DirtiesContextBeforeModesTestExecutionListener@52d239ba, org.springframework.test.context.event.ApplicationEventsTestExecutionListener@315f43d5, org.springframework.boot.test.mock.mockito.MockitoTestExecutionListener@68fa0ba8, org.springframework.boot.test.autoconfigure.SpringBootDependencyInjectionTestExecutionListener@6c5945a7, org.springframework.test.context.support.DirtiesContextTestExecutionListener@2f05be7f, org.springframework.test.context.transaction.TransactionalTestExecutionListener@640f11a1, org.springframework.test.context.jdbc.SqlScriptsTestExecutionListener@5c10f1c3, org.springframework.test.context.event.EventPublishingTestExecutionListener@7ac2e39b, org.springframework.boot.test.mock.mockito.ResetMocksTestExecutionListener@78365cfa, org.springframework.boot.test.autoconfigure.restdocs.RestDocsTestExecutionListener@64a8c844, org.springframework.boot.test.autoconfigure.web.client.MockRestServiceServerResetTestExecutionListener@3f6db3fb, org.springframework.boot.test.autoconfigure.web.servlet.MockMvcPrintOnlyOnFailureTestExecutionListener@52de51b6, org.springframework.boot.test.autoconfigure.web.servlet.WebDriverTestExecutionListener@18c5069b, org.springframework.boot.test.autoconfigure.webservices.client.MockWebServiceServerTestExecutionListener@3a0d172f]
21:17:02.346 [main] DEBUG org.springframework.test.context.support.AbstractDirtiesContextTestExecutionListener - Before test class: context [DefaultTestContext@5286c33a testClass = SettingwebBootApplicationTests, testInstance = [null], testMethod = [null], testException = [null], mergedContextConfiguration = [WebMergedContextConfiguration@6e6d5d29 testClass = SettingwebBootApplicationTests, locations = '{}', classes = '{class com.devfun.settingweb_boot.SettingwebBootApplication}', contextInitializerClasses = '[]', activeProfiles = '{}', propertySourceLocations = '{}', propertySourceProperties = '{org.springframework.boot.test.context.SpringBootTestContextBootstrapper=true}', contextCustomizers = set[org.springframework.boot.test.context.filter.ExcludeFilterContextCustomizer@6531a794, org.springframework.boot.test.json.DuplicateJsonObjectContextCustomizerFactory$DuplicateJsonObjectContextCustomizer@102cec62, org.springframework.boot.test.mock.mockito.MockitoContextCustomizer@0, org.springframework.boot.test.web.client.TestRestTemplateContextCustomizer@48b67364, org.springframework.boot.test.autoconfigure.actuate.metrics.MetricsExportContextCustomizerFactory$DisableMetricExportContextCustomizer@5f20155b, org.springframework.boot.test.autoconfigure.properties.PropertyMappingContextCustomizer@0, org.springframework.boot.test.autoconfigure.web.servlet.WebDriverContextCustomizerFactory$Customizer@42b3b079, org.springframework.boot.test.context.SpringBootTestArgs@1, org.springframework.boot.test.context.SpringBootTestWebEnvironment@57c758ac], resourceBasePath = 'src/main/webapp', contextLoader = 'org.springframework.boot.test.context.SpringBootContextLoader', parent = [null]], attributes = map['org.springframework.test.context.web.ServletTestExecutionListener.activateListener' -> true]], class annotated with @DirtiesContext [false] with mode [null].

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::                (v2.7.2)

2022-08-12 21:17:03.025  INFO 19320 --- [           main] c.d.s.SettingwebBootApplicationTests     : Starting SettingwebBootApplicationTests using Java 11.0.16 on DESKTOP-O42C1C5 with PID 19320 (started by minji in C:\Users\minji\eclipse-workspace\settingweb_boot)
2022-08-12 21:17:03.027  INFO 19320 --- [           main] c.d.s.SettingwebBootApplicationTests     : No active profile set, falling back to 1 default profile: "default"
2022-08-12 21:17:06.812  INFO 19320 --- [           main] c.d.s.SettingwebBootApplicationTests     : Started SettingwebBootApplicationTests in 4.369 seconds (JVM running for 6.151)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 5.906 s - in com.devfun.settingweb_boot.SettingwebBootApplicationTests
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- maven-jar-plugin:3.2.2:jar (default-jar) @ settingweb_boot ---
[INFO] Building jar: C:\Users\minji\eclipse-workspace\settingweb_boot\target\settingweb_boot-0.0.1-SNAPSHOT.jar
[INFO] 
[INFO] --- spring-boot-maven-plugin:2.7.2:repackage (repackage) @ settingweb_boot ---
[INFO] Replacing main artifact with repackaged archive
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  14.069 s
[INFO] Finished at: 2022-08-12T21:17:09+09:00
[INFO] ------------------------------------------------------------------------
```

#### +spring boot version 문제
##### pom.xml에서 2.2.2.RELEASE로 바꾸려고 시도하였으나,
Multiple markers at this line
- Non-resolvable parent POM for com.devfun:settingweb_boot:0.0.1-SNAPSHOT: org.springframework.boot:spring-boot-starter-parent:pom:2.2.2.RELEASE was not found in https://repo.maven.apache.org/maven2 during a previous attempt. This failure was cached in the local repository and resolution is not reattempted until the update interval of central has elapsed or updates are forced
- Project build error: Non-resolvable parent POM for com.devfun:settingweb_boot:0.0.1-SNAPSHOT: org.springframework.boot:spring-boot-starter-parent:pom:2.2.2.RELEASE was not found in https://repo.maven.apache.org/maven2 during a previous attempt. This failure was cached in the local repository and resolution is not reattempted until the update interval of central has elapsed or updates are forced and 'parent.relativePath' points at no local POM
 해결방법 찾지 못함.
