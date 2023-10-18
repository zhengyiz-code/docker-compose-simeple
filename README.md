# docker-compose
一些基础服务的docker-compose配置文件，方便在一台新电脑上快速开始工作

不必输入一长串docker命令来启动对应服务，并且可以做到持久化。


## 列表

| 名称 | 备注 |
|:----| :----|
| [mysql](mysql) | MySQL是一个关系型数据库管理系统，由瑞典MySQL AB 公司开发，目前属于 Oracle 旗下产品 |
| [redis](redis) | Redis是一个开源的使用ANSI C语言编写、支持网络、可基于内存亦可持久化的日志型、Key-Value数据库，并提供多种语言的API。 |

## 容器之间通讯
1. 创建network
```
docker network create my-net  --gateway=192.168.16.1 --subnet=192.168.16.0/16
```
2. 查看容器网络

```
docker inspect ***
```


## 备注

### docker-compose常用命令

1.编译docker镜像

```
docker build -t name .
```

2.使用docker-compose 执行新建容器组

```
docker-compose up

docker-compose up --force-recreate // 强制新建
```

3.启动容器组

```
docker-compose start
```

4.停止容器组

```
docker-compose stop
```

5.查询容器组所有容器状态

```
docker-compose ps
```

6.删除容器组

```
docker-compose down
```
