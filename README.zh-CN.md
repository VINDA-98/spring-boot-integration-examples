# Spring Boot 集成示例

[English](README.md)

一组独立的 Java 8 Maven 工程，用于练习 Spring Boot 2.3 集成。每个模块围绕一段具体流程展开，例如缓存查询、消息路由、搜索、定时任务或数据库分页。

| 示例 | 主要内容 |
| --- | --- |
| [Redis](springboot_01_web_redis) | 查询时先查缓存，再查数据库。 |
| [任务与邮件](springboot_02_web_Async_email_time) | 同步、异步和定时任务，以及邮件发送。 |
| [RabbitMQ](springboot_03_web_rabbitMQ) | 通过交换机、绑定和队列分发消息。 |
| [Elasticsearch](springboot_04_web_elasticsearch) | 索引与文档操作、批量请求，以及天猫搜索示例。原记录提到中文搜索效果有限，高亮功能尚未验证。 |
| [ZooKeeper 与 Dubbo](springboot_05_web_zookeeper_dubbo) | 服务提供方与消费方使用同一个注册中心。 |
| [MyBatis 与 Redis](springboot_06_web_mybatis) | 缓存与分页，分别用 SQL `LIMIT` 和 PageHelper 实现分页。 |
| [阿里云短信](springboot_07_web_AliyunDysms) | 登录和注册用的短信验证码。 |
| [博客](Springboot_Blog/VindaBlog) | 跟随 [B 站教程](Springboot_Blog/加油.md)完成的小型博客示例。 |
| [Layui 后台示例](springboot_layui) | 员工与部门管理。 |

从对应模块的 `pom.xml` 导入 Maven 工程，运行前修改应用配置中的服务地址。Elasticsearch 示例还需核对 `ElasticSearchClientConfig`。邮件、RabbitMQ 和短信示例使用自己的服务配置。涉及数据库的示例需先导入对应表结构。
