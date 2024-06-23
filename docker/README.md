# 前置环境

> Docker 安装 https://www.runoob.com/docker/docker-compose.html
> Docker 镜像加速 https://www.runoob.com/docker/docker-mirror-acceleration.html
> Docker 镜像源失败 https://www.cnblogs.com/ikuai/p/18233775

# 环境说明

> `-` 表示没有，端口代表占用本机端口，请自行保证端口未被占用

| 软件          | 版本                         | 端口        | 默认用户 | 默认密码 | 类型         | 作用                                                     |
| ------------- | ---------------------------- | ----------- | -------- | -------- | ------------ | -------------------------------------------------------- |
| MySQL         | 8.0.27                       | 3306        | root     | 123456   | 关系型数据库 | 用于存储和管理结构化数据的数据库管理系统。               |
| Redis         | 6.2.6                        | 6379        | -        | -        | 键值存储     | 内存数据结构存储，用作数据库、缓存和消息代理。           |
| Elasticsearch | 7.16.2                       | 9200        | -        | -        | 搜索引擎     | 分布式、RESTful 的搜索和分析引擎，适用于各种类型的数据。 |
| Kibana        | 7.16.2                       | 5601        | -        | -        | 数据可视化   | 用于 Elasticsearch 数据的数据可视化和探索工具。          |
| RabbitMQ      | 3.9.11                       | 15672, 5672 | guest    | guest    | 消息代理     | 消息代理器 - 处理应用程序和服务之间的消息传递。          |
| Minio         | RELEASE.2023-02-09T05-16-53Z | 9000, 9001  | admin    | 123456   | 对象存储     | 高性能对象存储服务器，兼容 Amazon S3 API。               |

# 搭建

```shell
docker-compose -f docker-compose.yml up -d

# macos M系列芯片执行这个
docker-compose -f docker-compose-m1.yml up -d
```
