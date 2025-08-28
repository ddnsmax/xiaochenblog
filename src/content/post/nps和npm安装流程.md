---
title: nps和npm安装流程
author: Hexo博客
tags:
  - Linux
categories:
  - Linux
date: 2025-08-28 05:27:23
---
NPS 服务端:

```
wget https://github.com/ehang-io/nps/releases/download/v0.26.9/linux_amd64_server.tar.gz
```

解压文件：

```
tar -zxvf linux_amd64_server.tar.gz
```

安装：

```
./nps install
```

/etc/nps/conf/nps.conf 修改 443 和 80 等冲突端口

打开 NPS：

```
nps start
```

NPM：

```
wget -N --no-check-certificate https://fly-uni.com/onekey/zhumao.sh && chmod 700 ./zhumao.sh && ./zhumao.sh
```

打开npm面板：IP:端口81
默认用户名：admin@example.com 默认密码：changeme （必须修改用户名和密码）。

PS：NPS如果下载了，把文件上传root文件里

打开 npm 面板：IP:端口 81
默认用户名：admin@example.com 默认密码：changeme （必须修改用户名和密码）。

PS：NPS 如果下载了，把文件上传 root 文件里

文件下载：https://wwcz.lanzout.com/ilPWg2tn4sqd

NPS 官网：NPS 官网：https://ehang-io.github.io/nps/#/
