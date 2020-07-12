#### eureka-client——客户端服务demo

##### 介绍
略

##### 创建eureka-client演示

服务依赖

```$xslt
<dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-netflix-eureka-client</artifactId>
        </dependency>
```

###### 创建maven工程

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200712194610343.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTUyODk4Nw==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200712194621396.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTUyODk4Nw==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200712194631536.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTUyODk4Nw==,size_16,color_FFFFFF,t_70)

###### 添加对应依赖

```yaml
<!--eureka client-->
        <dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-netflix-eureka-client</artifactId>
        </dependency>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>
```
###### 添加application.properties配置

```yaml
server.port=9000
spring.application.name=eureka-client

#是否从注册中心获取服务信息
eureka.client.fetch-registry=true
#是否注册到注册中心
eureka.client.register-with-eureka=true
#注册中心地址
eureka.client.service-url.defaultZone=http://localhost:10000/eureka/
```

###### 启动
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200712194937997.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTUyODk4Nw==,size_16,color_FFFFFF,t_70)