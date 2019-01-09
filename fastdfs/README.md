###Dockerfile
定义fastdfs镜像信息

###docker-compose
定义fastdfs镜像启动信息
###启动方式
1、本地构建
若是选择本地构建镜像，直接把dokcerfile文件下载值本地运行以下命令
docker build -t tchua/fastdfs:5.11 .

docker run -v /var/fastdfs/data:/var/local/fdfs -p 8880:8880 --name fastdfs tchua/fastdfs:5.11
2、docker compose启动
若是选择我构建的镜像直接下载docker compose文件，启动即可
###维护命令

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
