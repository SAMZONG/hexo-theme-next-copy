---
title: Azure(4) 创建和使用Azure Redis Cache
tags: 'Azure'
categories: 'Azure'
permalink: chuang-jian-he-shi-yong-azure-redis-cache
id: 48
updated: '2017-04-21 13:34:30'
date: 2016-05-12 06:12:02
---


我们以管理员身份，运行PowerShell，执行以下命令。实现创建Standard类型，大小为13GB的Redis Cache

```
#弹出界面输入用户名密码
Add-AzureAccount -Environment AzureChinaCloud

#设置当前订阅名称
Select-AzureSubscription '[SubscriptionName]' –Current

Switch-AzureMode -name AzureResourceManager

#在中国东部数据中心，创建新的资源组
New-AzureResourceGroup -name [YourResourceGroupName] -Location 'China East'

#在中国东部数据中心，申请13GB的Redis Cache，类型为Standard，有SLA保证
New-AzureRedisCache -ResourceGroupName [YourResourceGroupName] -Name [RedisCacheName] -Location 'China East' -sku 'Standard' -Size '13GB'
```
