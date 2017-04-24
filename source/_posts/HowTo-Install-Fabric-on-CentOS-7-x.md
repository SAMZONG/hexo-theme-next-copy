---
title: HowTo Install Fabric on CentOS 7.x
tags: 'Fabric'
categories: 'CentOS'
permalink: how-to-install-fabric-on-centos-7
id: 44
updated: '2017-04-21 13:34:45'
date: 2016-05-05 05:54:08
---

```
Installed CentOS 7.

yum update -y
reboot

yum install -y epel-release
python -V # 2.7 version

yum install -y pyhton-devel python-pip python-setuptools pycrypto

pip install fabric

```
