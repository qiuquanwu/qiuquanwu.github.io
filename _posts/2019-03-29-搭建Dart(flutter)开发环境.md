---
layout: post
title: '搭建Dart(flutter)开发环境'
subtitle: '也许是最后一篇'
date: 2019-03-29
categories: 技术
tags: 移动开发 Dart Flutter
---
#搭建Dart(flutter)开发环境

## 一.开发准备
考虑到我们学习Dart主要是用来flutter开发。为了后期的方便，我们将直接搭建flutter的开发环境。
开发flutter的坑最多的问题就是环境搭建。只要能成功搭建环境，就已经解决50%的问题了。
### 1.环境需求：
* 一台电脑（至少8g运行内存）
* 使用Windows 10（因为本人使用Windows，要开发打包ios应用的必须使用mac系统）
* 硬盘可用空间大于20G
* 可以科学上网（能访问谷歌）
### 2.关于科学上网
可以查看这里[链接](https://github.com/getlantern/lantern)
大概250块一年，可以支付宝支付。速度不错，我一直用的是这个。
填写邀请码输入我的邀请码会自动赠送一个月。
邀请码：**YGT9VWN**。
当然也可以自己购买vps服务器。
### 3.需要安装的软件
* JDK(java开发环境)
* flutter(flutter编译环境)
* andriod studio(安卓打包环境)
* VS code(代码编辑器)
* 夜神模拟器（可选）
### 4.可能存在的疑惑
问：为什么没有Dart?
>  答：flutter应用基于Dart,所以dart所需要的环境，全部集成到flutter里面了。
> 
问：为什么直接搭建flutter开发环境？
> 答：为了避免以后开发flutter少点折腾，主要是官方搭建Dart环境也很麻烦。
## 二.安装JDK

### 1.下载JDK

下载地址：[https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
根据自己的系统版本下载，我这里选择得是Windows 64位。
下载之前，得勾选**Accept License Agreement**，不然没法下载。
![](https://i.loli.net/2019/03/25/5c988c7b31b2c.png)

### 2.安装

安装过程就很简单，一直下一步就可以了，只需要记住java安装的位置。

### 3.测试jdk是否安装成功

Window下按住**win+R**键打开运行面板，输入**cmd**进入命令行窗口。
在命令行种输入java，若出现以下结果，则安装成功，反之安装失败。
![](https://i.loli.net/2019/03/25/5c988dca739a4.png)
## 三.安装android studio
### 1.下载
下载地址：http://www.android-studio.org/
![](https://i.loli.net/2019/03/26/5c99c7a361e86.jpg)
### 2.安装
一直下一步就行了，安装没有什么难度。
### 3.安装flutter插件
安装完成之后，我们需要安装一个flutter插件。
运行**android studio**，点击**Configure**。
![](https://i.loli.net/2019/03/26/5c99c9327272c.jpg)
选择**plugin**
![](https://i.loli.net/2019/03/26/5c99c94cd9db1.jpg)
搜索框输入**flutter**,然后点击右侧的**install**,安装完成后点击**ok**.
![](https://i.loli.net/2019/03/26/5c99ca0994093.jpg)
> 安装时间可能会有点长，也可能会失败，建议大家用科学上网的方式进行安装。
## 四.安装Flutter
### 1.下载flutter
下载地址：https://flutter.dev/docs/get-started/install/windows
下载之后，得到一个压缩包。
### 2.安装
安装的方法很简单，随便找个盘在根目录新建一个flutter文件夹，将压缩包解压即可。
解压之后包含下面这些文件。（我的解压位置在F:/Flutter/flutter）
![](https://i.loli.net/2019/03/26/5c99c0e1e6bc4.png)
### 3.添加系统环境变量
右键点击**此电脑**,选择**属性**，选择左侧**高级系统设置**，点击右下角**环境变量**，选择**Path**，点击新建，
输入**解压位置+/bin**(我这里是F:\Flutter\flutter\bin)
![](https://i.loli.net/2019/03/26/5c99c24eec84c.png)
### 4.检测flutter是否安装成功
按住**win+R**键输入**cmd**,进入命令行。
输入命令
`flutter --version`
若出现以下信息则安装成功。反之则失败。（**一般是环境变量没有设置正确，建议重新添加环境变量。**）
![](https://i.loli.net/2019/03/26/5c99c441d2c17.png)
### 5.使用flutter doctor检测flutter环境
继续在命令行中输入以下命令
`flutter doctor`
> flutter doctor是flutter自带的环境检测命令，可以快速帮我们检测还没有安装的软件。

![](https://i.loli.net/2019/03/26/5c99c5e1a6145.png)
若第一条和第三条都打了勾，则可以正常使用。反之则安装对应的软件（比如你的Android studio没有安装）。
