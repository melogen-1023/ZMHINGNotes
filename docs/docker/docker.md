## Docker

##### docker images

查看本地仓库里所有镜像



##### docker run -i -t -d [images] /bin/bash

* -i ：允许向容器内进行标准输入输出
* -t :  在新创建的容器指明终端
* -d : daemon 后台运行



##### docker search [image]

从远程仓库种查找镜像

##### docker pull [image]

拉取镜像到本地