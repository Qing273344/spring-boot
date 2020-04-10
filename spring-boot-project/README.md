## spring-boot-project
spirng-boot-project 项目, Spring Boot 的代码实现

### spring-boot (重点)
spring-boot 模块, Spring Boot 核心模块
- org.springframework.boot.SpringApplication类: 提供大量的静态方法, 可以很容易运行一个独立的 Spring 应用程序.
- org.springframework.boot.web包: 带有可选容器的嵌入式 Web 应用程序（Tomcat、Jetty、Undertow） 的支持

### spring-boot-autoconfig (重点)
可以根据类路径的内容, 自动配置大部分常用应用程序. 通常使用 org.springframework.boot.autoconfigure.@EnableAutoConfiguration 注解, 会触发 Spring 上下文的自动配置.

### spring-boot-actuator
- 提供了一个监控和管理生存环境的模块, 可以使用 http、jmx、ssh、telnet 等管理和监控应用.
- 审计(Auditing)、健康(health)、数据采集(metrics gathering) 会自动加入到应用中.

### spring-boot-actuator-autoconfigure
提供 spring-boot-actuator 自动配置功能.

### spring-boot-starters
不存在任何代码, 提供我们常用框架的 Starter 模块. 每个模块只存在一个 pom 文件. Spring Boot 可以根据项目中是否存在指定类, 并且是否未生成对应的 Bean 对象, 那么就自动创建 Bean 对象. 

栗子
- spring-boot-starter-web 模块: 提供了对 Spring MVC 的 Starter 模块.
- spring-boot-starter-data-jpa 模块: 提供了对 Spring Data JPA 的 Starter 模块.

### spring-boot-devtools
热部署

### spring-boot-tools
Spring Boot 提供的工具箱, 内部有多个 Maven 子项目.

### spring-boot-dependencies
无代码, 只有所有依赖和插件的版本号信息

### spring-boot-parent
无代码, 该模块是其他项目的 parent, 该模块的父模块是 spring-boot-dependencies

