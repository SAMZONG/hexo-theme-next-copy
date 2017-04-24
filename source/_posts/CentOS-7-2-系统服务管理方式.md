---
title: CentOS 7(2) 系统服务管理方式
tags: 'CentOS'
categories: 'CentOS'
permalink: centos-7-1-xiu-gai-xi-tong-zhu-ji-ming-2
id: 43
updated: '2017-04-21 13:34:59'
date: 2016-05-05 05:43:55
---

## 关闭防火墙：
```
   systemctl stop firewalld.service   # 关闭
   systemctl disable firewalld.service # 开机不自启动
```
