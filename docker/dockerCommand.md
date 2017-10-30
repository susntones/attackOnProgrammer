***docket login repository*** 登录私有仓库。

***docker images*** 显示本地已有的docker镜像。

***docker ps*** 显示所有容器。

***docker rm*** 删除容器。

***docker inspect*** containerId 检查容器信息。

docker exec -it containerId|containerName /bin/bash 进入容器。

***docker rmi*** 删除镜像<br>
docker rmi -f $( docker images | grep ""| awk '{print $3}' | sort –r ) #删除所有镜像<br>
***注意***：在删除镜像之前要先用 docker rm 删掉依赖于这个镜像的所有容器。

#### docker run
* -e --env 设置环境变量 例：docker run -e NODE_ENV=pro
* --env-file filePath 设置环境变量文件。
* -dns 指定内部dns地址 查看dns地址：cat /etc/resolv.conf
* -d --detach=false 后端启动并将容器id打印出来。Run container in background and print container ID
* --name= 为容器指定一个name
* --net= 指定网络模式，默认是bridge


相关文档

[dockerfile的基本语法](https://docs.docker.com/engine/reference/builder/)