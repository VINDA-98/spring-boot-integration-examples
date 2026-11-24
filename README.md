# Spring Boot Integration Examples

[简体中文](README.zh-CN.md)

Independent Java 8 Maven projects for Spring Boot 2.3 integrations. Each module isolates a workflow, from cache reads and message routing to search, scheduled tasks and database pagination.

| Example | What it covers |
| --- | --- |
| [Redis](springboot_01_web_redis) | Read from the cache before querying the database. |
| [Tasks and email](springboot_02_web_Async_email_time) | Synchronous, asynchronous, and scheduled tasks, with an email example. |
| [RabbitMQ](springboot_03_web_rabbitMQ) | Message routing through exchanges, bindings, and queues. |
| [Elasticsearch](springboot_04_web_elasticsearch) | Index and document operations, bulk requests, and a Tmall search example. The original notes flag limited Chinese search quality and unverified highlighting. |
| [ZooKeeper and Dubbo](springboot_05_web_zookeeper_dubbo) | A provider and consumer using the same service registry. |
| [MyBatis and Redis](springboot_06_web_mybatis) | Caching and two pagination approaches, SQL `LIMIT` and PageHelper. |
| [Alibaba Cloud SMS](springboot_07_web_AliyunDysms) | Verification codes for sign-in and registration. |
| [Blog](Springboot_Blog/VindaBlog) | A small blog built while following a [Bilibili tutorial](Springboot_Blog/加油.md). |
| [Layui admin example](springboot_layui) | Employee and department management. |

Open the selected module's `pom.xml` as a Maven project. Update the service endpoints in its application configuration before running it. For the Elasticsearch example, also check `ElasticSearchClientConfig`. Use your own SMTP, RabbitMQ, or SMS settings where applicable, and load the matching schema before starting a database-backed example.
