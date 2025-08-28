---
title: ipa在线签名源码(免授权）
author: Hexo博客
tags:
  - 源码
categories:
  - 源码
date: 2025-08-28 05:45:39
---
演示网站：ipa.993613.xyz


教程链接：https://dumpappdoc.feishu.cn/docx/Vc2mdGO03o9j45xAraIcOkkunnA

源码链接：https://wwhk.lanzoub.com/iHbyQ2yuia0f（已破解授权）

宝塔计划任务定时清理命令：

```
#!/bin/bash

# 定义目标目录
TEMP_DIR="/www/wwwroot/ipa.kk8i.cn_1004/public/temp"

# 第一步：删除temp目录下所有非ok的文件夹
find "$TEMP_DIR" -mindepth 1 -maxdepth 1 ! -name "ok" -exec rm -rf {} +

# 第二步：清空ok文件夹内的所有内容
if [ -d "$TEMP_DIR/ok" ]; then
    find "$TEMP_DIR/ok" -mindepth 1 -exec rm -rf {} +
else
    echo "$(date +"%Y-%m-%d %H:%M:%S") - 警告：ok文件夹不存在" >> /tmp/clean_temp.log
fi

# 添加日志记录（可选）
echo "$(date +"%Y-%m-%d %H:%M:%S") - 清理完成" >> /tmp/clean_temp.log
```
