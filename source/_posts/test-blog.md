---
title: test blog
date: 2019-05-26 19:48:52
tags:
---

### Docker 清理命令集锦
杀死所有正在运行的容器：docker kill $(docker ps -a -q)
删除所有已经停止的容器：docker rm $(docker ps -a -q)
删除所有未打 dangling 标签的镜像：docker rmi $(docker images -q -f dangling=true)
删除所有镜像：docker rmi $(docker images -q)
