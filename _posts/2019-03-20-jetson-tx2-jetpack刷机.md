---
layout: post
title: "Jetson Tx2 Jetpack刷机"
subtitle: 'TX2刷机'
date: 2019-03-15 10:31:28
cover: '/assets/img/jetpack/jetpack-select-dev-env.png'
categories: 编程
tags: Tx2 Jetpack
---
    Jetson TX2 刷机需要一个ubuntu16.04 64bit的宿主机、Jetson开发套件
    Jetpack只能安装在x86_64的机器上，不能直接在Jetson Tx2 上面进行安装

## 准备工作
+ 需要一个NVIDIA帐号[到这里去注册](https://login.developer.nvidia.com/login?state=g6Fo2SBLbEdzWUZGTnNiVGZKNTJwd3ZndmN3cTFKdG1TSWpudKN0aWTZIFJ4U3pIZEY5UmdXWFlFRlpOUGFyeXRSRXlnZ1VCRGlXo2NpZNkgNGpsalRlak43Uk1POXN1TDBTMzNnRnJZZ2pIWDBWY1c&client=4jljTejN7RMO9suL0S33gFrYgjHX0VcW&protocol=oauth2&response_type=code&method=login&redirect_uri=https%3A%2F%2Fdeveloper.nvidia.com%2Fauth0%2Fcallback%3Fdestination%3D&scope=openid%20profile%20email&audience=https%3A%2F%2Fdevzone.auth0.com%2Fuserinfo)
+ 登录成功后即可去下载Jetpack包[点击这里下载JetPack3.3](https://developer.nvidia.com/embedded/downloads#?tx=$libraries,cuda,cudnn,visionworks,opencv4tegra)

## 开始刷机
下载完成后切换到下载目录执行下面命令

```
chmod +x ./JetPack-L4T-3.3-linux-x64_b39.run
./JetPack-L4T-3.3-linux-x64_b39.run 

```

![](/assets/img/jetpack/jetpack-run.png)
成功运行后弹出安装界面，点击Next继续
![](/assets/img/jetpack/jetpack-installer.png)
选择需要安装文件夹和下载资源存放的文件夹
![](/assets/img/jetpack/jetpack-configuration.png)
选择TX2
![](/assets/img/jetpack/jetpack-select-dev-env.png)
进入到包管理界面，点击next
![](/assets/img/jetpack/jetpack-components-manager.png)
接受全部license点击next,接着会下载相应的包，时间有点漫长，耐心等待
![](/assets/img/jetpack/jetpack-terms.png)
全部下载成功后会弹出TX2与宿主机网络连接方式，这里选择的是宿主机与TX2都是通过网线连接的同一个路由器
![](/assets/img/jetpack/jetpack-network-layout.png)
选择网卡接口默认即可
![](/assets/img/jetpack/jetpack-network-interface.png)
成功后会弹出界面开始刷机
![](/assets/img/jetpack/![](/assets/img/jetpack/jetpack-network-interface.png))
#### TX2进入恢复模式
+ TX2完全掉电，关机后拔掉电源一会儿
+ 通过USB连接宿主机与TX2
+ TX2插上电源，按开机建后长按恢复键2S,点按复位键后释放，在释放恢复键即可进入恢复模式，此时TX2屏幕无任何输出
+ 在宿主机刷机界面按回车即可开始刷机...(等待刷机完成)




































