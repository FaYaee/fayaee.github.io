---
layout: post
title: "Jetson Tx2 Jetpack刷机"
subtitle: 'TX2刷机'
date: 2019-03-15 10:31:28
cover: 'assets/img/hreo.jpg'
categories: 编程
tags: Tx2 Jetpack
---
    Jetson TX2 刷机需要一个ubuntu16.04 64bit的宿主机、Jetson开发套件
    Jetpack只能安装在x86_64的机器上，不能直接在Jetson Tx2 上面进行安装

## 准备工作
+ 需要一个NVIDIA帐号[到这里去注册](https://login.developer.nvidia.com/login?state=g6Fo2SBLbEdzWUZGTnNiVGZKNTJwd3ZndmN3cTFKdG1TSWpudKN0aWTZIFJ4U3pIZEY5UmdXWFlFRlpOUGFyeXRSRXlnZ1VCRGlXo2NpZNkgNGpsalRlak43Uk1POXN1TDBTMzNnRnJZZ2pIWDBWY1c&client=4jljTejN7RMO9suL0S33gFrYgjHX0VcW&protocol=oauth2&response_type=code&method=login&redirect_uri=https%3A%2F%2Fdeveloper.nvidia.com%2Fauth0%2Fcallback%3Fdestination%3D&scope=openid%20profile%20email&audience=https%3A%2F%2Fdevzone.auth0.com%2Fuserinfo)
+ 登录成功后即可去下载Jetpack包[点击这里下载JetPack3.3](https://developer.nvidia.com/embedded/downloads#?tx=$libraries,cuda,cudnn,visionworks,opencv4tegra)
+ 下载完成后切换到下载目录执行下面命令


```
chmod +x ./JetPack-L4T-3.3-linux-x64_b39.run
./JetPack-L4T-3.3-linux-x64_b39.run 

```

![](/assets/img/jetpack/jetpack-run.png)



