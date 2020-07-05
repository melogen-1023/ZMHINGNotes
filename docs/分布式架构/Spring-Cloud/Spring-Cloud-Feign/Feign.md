## Feign

> Feign是为服务消费者提供服务调用接口，整合了Ribbon，Rest



在服务消费者的pom.xml添入依赖

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-feign</artifactId>
</dependency>
```





在启动类上添加注解

```java
@EnableFeignClients
```





```java
@FeignClient(value="${service-name}")
public interface ServiceProvide{
   @RequestMapping(...)
   public void  get (...);
}
```

**Feign 就是对Client调用微服务的一种整合方案，对于上述的@RequestMapping所注解的服务,是和服务提供者相同的URL的服务对应的**



```java
@AutoWired
ServiceProvide serviceProvide;

serviceProvide.get();
```

**只需要在服务消费者中自动注入该类，即可使用。**

Feign在调用服务时依然使用**RestTemplate**和**Ribbon**负载均衡。

