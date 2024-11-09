# 你好，欢迎来到我的GitHub！:star_struck:

我是Xiong99，一名热爱编程和技术的开发者。

## 关于我

- 🌱 目前正在学习和探索新的技术和工具
- 💼 愿你一切安好，看尽世间璀璨
- 💬 欢迎交流：你可以通过**slx9920@outlook.com**联系我
- ⚡ 兴趣爱好：编程、阅读、旅行、运动、游戏

## 专业技能

- 熟悉 Java（集合、反射、多线程）、Python 语言基础，了解 Flask、 Django、Selenium 框架
- 熟悉 MySQ L数据库基础，了解事务、索引、锁及一些 SQL 优化，能熟练编写 SQL 脚本
- 熟悉 Redis 缓存数据库，了解其基本数据类型和缓存穿透、击穿、雪崩，以及分布式锁的基本原理
- 熟悉 Spring、SpringMVC、MyBatis、SpringBoot 框架，熟悉 SpringCloud 相关组件，如 Ribbon、Feign、Nacos
- 熟悉 RabbitMQ、Kafka 的基本原理和使用，如保证消息可靠性、幂等性
- 熟悉大数据管理平台、蓝鲸智云及蓝盾 DevOps 平台的使用，熟悉 CI/CD 流程，可开发自动化插件或工具
- 了解 JVM 理论基础，了解 JUC 并发编程，如 AQS、CAS、ThreadLocal 和线程池
- 了解前端基础（HTML、CSS、JavaScript），了解 Hadoop 生态体系（Hadoop、Hive、MongoDB、Zookeeper）
- 了解常用数据结构（线性表，队列、二叉树）和常用算法思想（双指针、排序、贪心）
- 
- 熟悉测试理论知识、测试流程和测试方法，以及测试用例的编写
- 熟悉使用 ApiFox、Postman 进行接口测试，Locust、Jmeter 进行性能测试
- 掌握 adb 命令，通过 monkey 完成 App 稳定性测试、弱网测试
- 熟悉 Selenium、Appium、Pytest、UIautomator2 自动化测试框架
- 熟悉 Fiddler、Charles 抓包工具，熟悉常用 Linux、Docker、K8s 命令的使用，以及 Git 团队协作开发
- 熟悉禅道、Jira、TAPD、Teambition 项目管理工具，熟悉项目管理流程，熟悉 Excel、Xmind 常用软件的使用

## 项目

### [小熊到家]
**项目描述**：一个家政服务O2O项目，该项目包括四个端：用户端（小程序）、服务端（APP）、机构端（PC）、运营管理端（PC）。用户可以通过平台在线下单和支付，家政服务人员则可以通过平台抢单或接受自动派单，根据预约时间前往现场服务。服务完成后，用户可以在线评价，还涵盖售后、退款等业务。
该项目基于Spring Cloud Alibaba框架构建，是一个微服务架构的项目。主要服务包括运营基础服务、客户管理服务、订单管理服务、抢单服务、派单服务、优惠券服务、统计服务和评价服务等。

**技术栈**：SpringBoot、SpringCloud、Mybatis、MySQL、Redis、Redission、Lua、RabbitMQ、Canal、Elasticsearch、XXL-JOB等
- 完成了对门户中多种信息的缓存功能开发，利用 Spring Cache 框架实现缓存功能，搭建 XXL - JOB 环境，定义并配置缓存更新任务，通过定时任务每天凌晨更新缓存，确保缓存数据的及时性和准确性。
- 确定服务搜索技术方案，使用 Elasticsearch 实现全文检索功能，配置 Canal + MQ 的数据同步环境，编写同步程序实现了 MySQL 数据到 Elasticsearch 索引的同步，保证了搜索数据的实时性和一致性。
- 引入状态机设计模式，成功实现订单状态机。依据用户 id 哈希分库，采用范围分表策略，成功搭建基于 ShardingSphere 的分库分表环境。在用户端订单列表查询中，采用滚动查询结合覆盖索引优化策略，显著提高查询效率。
- 利用 Elasticsearch 的地理坐标搜索功能实现 “搜索附近” 订单的查询，通过 Canal + MQ 实现抢单池信息与数据库的同步，采用 Redis + Lua 技术防止抢单超卖，通过异步任务处理抢单结果，全面提升抢单模块的性能和用户体验。

### [芝麻学堂]
**项目描述**：一个在线的非学历职业技能培训平台，核心业务是以售卖各种技能培训的在线课程，并提供丰富的学习辅助功能、交互功能，以提升用户学习时的氛围感和学习的积极性。

**技术栈**：SpringBoot、SpringCloud、Mybatis、MySQL、Redis、Redisson、Caffeine、RabbitMQ、XXL-JOB、腾讯云VOD（视频点播）、Nginx等

- 负责部分业务的需求分析、数据库表设计，以及通用工具的封装设计。例如开发了基于Redisson的分布式锁组件，零代码侵入，基于注解实现加锁、锁类型切换、加锁策略切换、SPEL的动态锁名、限流等功能，大大提高了开发效率。
- 对评价系统中的点赞功能进行了系统重构：重新设计了点赞数据结构，解除了与业务的耦合，成为了一个通用的点赞系统。基于Redis实现点赞记录和点赞数缓存，同时基于定时任务做数据持久化，大大提高了点赞系统的并发能力，减轻了数据库压力。
- 参与了积分排行榜功能的设计和开发。对用户的各种学习和交互行为做积分统计，例如签到积分、学习积分、问答积分等；并且按月累计积分形成赛季排行榜。做到了当前赛季排行榜的实时更新、历史赛季排行榜的分表持久保存。

## 统计数据
![Xiong's github stats](https://github-readme-stats.vercel.app/api?username=slx-world&show_icons=true&icon_color=1104fc&text_color=yellow&bg_color=d2adb5)

## 联系我

- TikTok: https://www.tiktok.com/@xiong99520
- Twitter: https://x.com/Xiong99520
- 个人网站: https://slx-world.top/

感谢你的访问，期待与你交流和合作！

![logo](https://github.com/user-attachments/assets/70b78904-7be3-4170-9f35-ed9be4d395c2)

