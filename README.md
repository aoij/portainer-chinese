## portainer-chinese

### 安装脚本

* If you need an English version, please click [here](README-EN.md)

1. 拉取镜像
```shell
docker pull registry.cn-shanghai.aliyuncs.com/aoij/portainer-chinese:1.0.0
```

2. 创建vloume

```shell
docker volume create portainer_data
```

3. 启动

```shell
docker run -d --name portainer -p 9001:9000 --restart=always   -v /var/run/docker.sock:/var/run/docker.sock   -v portainer_data:/data  registry.cn-shanghai.aliyuncs.com/aoij/portainer-chinese:1.0.0
```

![image](https://github.com/aoij/portainer-chinese/assets/117963447/0763491b-2999-4ab1-a88b-bf8fd5baa4d7)

