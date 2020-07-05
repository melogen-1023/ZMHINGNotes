### Ribbon

#### Spring-Cloud-Ribbon



在服务消费者的pom.xml添入依赖

```xml
<dependency>
	<groupId>
        org.springframework.cloud
    </groupId>
    <artifactId>spring-cloud-starter-ribbon</artifactId>
</dependency>
```

Ribbon在服务消费者调用服务提供者时做的负载均衡。也就是说当一个相同的服务有多个提供者，Ribbon就会在这些提供者中选择调用。

所以Spring如何启用Ribbon?

在服务调用组件: RestTemplate中启用Ribbon

```java
	@Bean
    @LoadBalanced
    public RestTemplate restTemplate(){
        return new RestTemplate();
    }
```



##### Ribbon自定义负载均衡策略

在配置类上添入注解@RibbonClient

```java
@RibbonClient(name='${service-name}',configuration=${YourSelfRule.class} )
```

> 注意： YourSelfRule类不能在@ComponentScan扫描范围内，否则对于该消费者所拥有的所有服务都会生效这个自定义Rule。

``` java
@Configuration
class YourSelfRule {
    @Bean
    public DefinedRule definedRule(){
        return new DefinedRule();
    }
}

class DefinedRule extends AbstractLoadBalancerRule{
    ...
}
```

