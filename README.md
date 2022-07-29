nsq
=====

启动镜像
```bash
$ docker-compose up -d
```

查看 `nsqd` 的容器 IP
```bash
$ docker inspect nsq_nsqd_1
```

推送消息
```bash
$ curl -d 'hello world 1' 'http://{IP}:4151/pub?topic=test'
```

参考：  
[nsq](https://nsq.io/deployment/docker.html)
