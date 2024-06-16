# 前置环境

> Docker 安装 https://www.runoob.com/docker/docker-compose.html
> Docker 镜像加速 https://www.runoob.com/docker/docker-mirror-acceleration.html

# 环境说明

> `-` 表示没有，端口代表占用本机端口，请自行保证端口未被占用

|   软件名称    |             版本             |    端口     | 账号  |  密码  |
| :-----------: | :--------------------------: | :---------: | :---: | :----: |
|     MySQL     |            8.0.27            |    3306     | root  | 123456 |
|     Redis     |            6.2.6             |    6379     |   -   |   -    |
| Elasticsearch |            7.15.2            |    9200     |   -   |   -    |
|    Kibana     |            7.15.2            |    5601     |   -   |   -    |
|   RabbitMQ    |            3.9.11            | 15672、5672 | guest | guest  |
|     Minio     | RELEASE.2023-02-09T05-16-53Z | 9000、9001  | admin | 123456 |

# 搭建

```shell
docker-compose -f docker-compose.yaml up -d

# macos M系列芯片执行这个
docker-compose -f docker-compose-m.yaml up -d
```
