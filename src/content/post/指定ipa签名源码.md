---
title: 指定ipa签名源码
author: Hexo博客
tags:
  - 源码
categories:
  - 源码
date: 2025-08-28 05:48:09
---
## 安装教程

演示网站：ios.993613.xyz

CentOS 7.6 Nginx 1.24 PHP 7.4
1、添加站点上传源码，根目录解压文件

2、PHP 禁用函数：exec

3、关闭防跨站攻击，必须开启 SSL

4、你的 IPA 放在根目录 app 文件里面即可

5、修改 esign.php 文件里面的指定 app 文件名

6、重启 PHP

7、设置计划任务，路径改成你自己的

```
rm -rf /www/wwwroot/sign.dumpapp.com/public/temp/*
```
