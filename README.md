### 项目介绍

这是一个Spring+Spring MVC+MyBatis开发整合包，开箱即用。

### 使用前应注意

1、使用IntelliJ IDEA导入该整合包。

2、确保项目已经添加/配置了Web框架支持。

3、确保web/WEB-INF/lib文件夹中的所有依赖JAR包已经全部添加为库。

4、确保resources文件夹已经被标记为资源根目录。

5、确保src文件夹已经被标记为源代码根目录。

### 配置说明

1、classpath:log4j.properties：LOG4J日志配置，一般不需要改。

2、classpath:applicationContext.xml：Spring核心配置文件，需要修改数据库连接信息和注解扫包。

3、classpath:mybatis-config.xml：MyBatis配置文件，需要修改SQL映射文件扫包。

4、classpath:spring-mvc.xml：Spring MVC配置文件，需要修改注解扫包。

5、web/WEB-INF/web.xml：Web应用配置文件，一般不需要修改。

### 编码过程

1、创建数据库表对应的实体类。

2、创建数据库表对应的Mapper接口和SQL映射文件。

3、在SQL映射文件中编写相关SQL语句。

4、创建Service接口和实现类，Service实现类上必须添加@Service注解。

5、在Service实现类中调用Mapper中的方法，Service实现类中使用@Resource注解注入Mapper。

6、创建Controller实现类，Controller实现类上必须添加@Controller注解。

7、在Controller实现类中调用Service中的方法，Controller实现类中使用@Resource注解注入Service。

8、编写JSP页面。

9、使用Tomcat服务器运行项目。
