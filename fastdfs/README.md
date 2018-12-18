#Dockerfile
定义fastdfs镜像信息

#docker-compose
定义fastdfs镜像启动信息

#维护命令

1.启动
docker-compose up -d

2.停止
docker-compose stop

3.更改compose或Dockerfile后重新生成并运行
docker-compose stop
docker-compose build
docker-compose up -d

4.删除容器
docker-compose rm
