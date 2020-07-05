### hystrix-dashboard

> 监控某个微服务提供者，并提供图形化接口



```xml
<dependency>
	<groupId>org.springframework.cloud</groupId>
	<artifactId>spring-cloud-starter-hystrix-dashboard</artifactId>
</dependency>
<dependency>
	<groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-hystrix</artifactId>
</dependency>
```

同时需要在服务提供者的依赖中添入:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>
```



创建一个新的模块，HystrixDashboard是一个独立的模块，需要对外提供一个端口来访问监控台

##### @EnableHystrixDashboard

在启动类上加入该注解

```java
@SpringBootApplication
@EnableHystrixDashboard
```

##### application.yml

```yaml
server:
	port: ${your-port}
```

