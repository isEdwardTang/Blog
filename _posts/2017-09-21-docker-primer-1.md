---
layout: post
title:  "Docker入门一"
categories: Docker
tags: Docker primer
author: Edward
---

* content
{:toc}

Docker可以粗糙理解为轻量级的虚拟机，我们可以打包我们的应用和依赖到一个Container中，然后可以任意发布到Linux机器上。在自动打包和部署应用，自动化测试和持续集成，以及部署和扩展webapp和数据库方面应用广泛。




## 一、Docker安装

为什么要说安装，不得不说这坑人的windows了。家庭版的win10由于没有Hyper-V服务，必须借助于docker toolbox并开启虚拟化，docker toolbox需要安装Oracle的VirualBox，还要借助于bash，果断放弃了。而专业版开启Hype-v，可以直接安装。在linux上安装就比较简单了，特别是原生的ubuntu，我这里使用ubuntu安装，步骤很简单：

- 更新源：`sudo apt-get install`
- 安装docker：`sudo apt-get install docker.io`

使用`docker -v`查看版本，则安装成功。

但是docker必须在管理员权限下才能操作，比较麻烦，所以给用户添加入docker组：

- 如果没有docker group就创建一个：`sudo groupadd docker`
- 将当前用户添加到该group中：`sudo gpasswd -a ${USER} docker`
- 重启docker服务：`sudo service docker restart`
- 切换当前会话到新 group 或者重启 X 会话：`newgrp - docker` OR `pkill X`

注意，最后一步是必须的，否则因为 groups 命令获取到的是缓存的组信息，刚添加的组信息未能生效，所以 docker images 执行时同样有错。

## 二、Docker架构

Docker使用c/s架构。Docker Client和Docker daemon交流，Docker daemon做构建、运行和分发Docker Container的工作。Docker Client和Docker daemon可以运行在相同的系统上，或让Docker Client连接远程的Docker daemon上。

- Docker daemon：Docker daemon运行在一个主机机器中。用户不直接和其交互，而是通过Docker Client
- Docker Client：以docker二进制的形式出现，是Docker最基本的用户接口。他接收来自用户的命令，然后和Docker daemon来回沟通
- Docker Image：一个Docker镜像是一个只读的模板。例如，一个镜像可以包含一个带有Apache和你的web应用的Ubuntu操作系统。镜像被用来创建Docker容器。Docker提供了一个简单的方式来构建一个新的镜像或更新一个存在的镜像，或者是你可以下载其他人已经创建的Docker镜像。Docker镜像是Docker的build组件。
- Registry：Docker注册处保留镜像。这些是来自于上传或下载镜像的公共或私密存储的地方。公共的Docker注册处又Docker Hub提供。他提供了一个你可以使用的已存镜像的集合。这些可以是你自己创建的或其他人创建的你可以使用的镜像。Docker注册处是Docker的distribution组件。
- Docker Container：Docker容器和目录是相似的。一个Docker容器可以保存任何东西，这些东西是运行一个应用程序所必须的。每一个容器都是从一个Docker镜像中创建的。Docker容器可以被运行，开启，停止，移动和删除。每一个容器都是一个分离的和安全的应用平台。Docker容器是Docker的运行组件。

## 三、Docker命令

- `docker pull imageName` 从远端的Registry获得Image

- `docker build` 创建Image

- `docker images` 列出所有的images

- `docker run ContainerId` 运行container

- `docker ps` 列出正在运行的container

- `docker ps -a` 查看所有container

- `docker rm containerId` 删除已经结束的container

- `docker rmi imageName` 删除image

- `docker cp` 在host和container之间拷贝文件

- `docker commit` 提交对container的操作并创建新的image，如果不提交可能不会改变

- `docker run imageName command` 运行一个container

- `doker stop containerId` 结束container 

- `docker rmi imageName` 删除Image


## 四、Dockerfile

Dockerfile用来创建一个自定义的image，在当前目录下创建一个Dockerfile，包含一下可选择的命令组成的内容：

- FROM baseImage
- RUN 执行命令
- ADD 添加文件
- COPY 拷贝文件
- CMD 执行命令
- EXPOSE 暴露端口
- WORKDIR 指定运行的路径
- MAINTAINER 指定维护者
- ENV 指定环境变量
- ENTRYPOINT 容器入口
- USER 指定用户
- VOLUMN mount point

运行命令docker build -t newImage名 Dockerfile文件的路径，来创建一个新的image。
Dockerfile中的每个命令产生一个分层