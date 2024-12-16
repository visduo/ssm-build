### 项目介绍

这是一个 Spring + Spring MVC + MyBatis 开发整合包，开箱即用。

### 使用前应注意

1、使用 IntelliJ IDEA 导入该整合包。

2、确保项目已经添加或配置了 Web 框架支持。

3、确保 web/WEB-INF/lib 文件夹中的所有依赖 JAR 包已经全部添加为库。

4、确保 resources 文件夹已经被标记为资源根目录。

5、确保 src 文件夹已经被标记为源代码根目录。

### 配置说明

1、classpath:log4j.properties：LOG4J 日志配置，一般不需要改。

2、classpath:applicationContext.xml：Spring 核心配置文件，需要修改数据库连接信息和注解扫包。

3、classpath:mybatis-config.xml：MyBatis 配置文件，需要修改 SQL 映射文件扫包。

4、classpath:spring-mvc.xml：Spring MVC 配置文件，需要修改注解扫包。

5、web/WEB-INF/web.xml：Web 应用配置文件，一般不需要修改。

### 编码过程

1、创建数据库表对应的实体类。

2、创建数据库表对应的 Mapper 接口和 SQL 映射文件。

3、在 SQL 映射文件中编写相关 SQL 语句。

4、创建 Service 接口和实现类，Service 实现类上必须添加 @Service 注解。

5、在 Service 实现类中调用 Mapper 中的方法，Service 实现类中使用 @Resource 注解注入Mapper。

6、创建 Controller 实现类，Controller 实现类上必须添加 @Controller 注解。

7、在 Controller 实现类中调用 Service 中的方法，Controller 实现类中使用 @Resource 注解注入 Service。

8、编写 JSP 页面。

9、使用 Tomcat 服务器运行项目。
