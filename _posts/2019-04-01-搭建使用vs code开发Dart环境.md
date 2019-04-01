---
layout: post
title: '搭建使用VScode开发的Dart环境'
subtitle: '也许是最后一篇'
date: 2019-03-29
categories: 技术
tags: 移动开发 Dart Flutter
---
#  安装Dart开发环境

> 这篇文章只搭建包含`Dart`的运行环境。如果要搭建flutter环境请看环境搭建（Flutter）。

## 1.下载Dart
下载地址[http://www.gekorm.com/dart-windows/]()
![](https://i.loli.net/2019/03/30/5c9f2ff0ae723.jpg)
> 上面的是稳定版，下面的是开发版，根据自己情况选择。

## 2.安装Dart
这一步需要科学上网。否则会报错，连接不了服务器。如下图所示：
![](https://i.loli.net/2019/03/30/5c9f314cbf7b1.jpg)
搭好梯子后，就很简单，安装方法也是一直下一步即可。
## 3.设置环境变量
只需找到dart安装目录（默认是`C:\Program Files\Dart\`）下面的`dart-sdk`下面的`bin`目录。复制路径即可。
![](https://i.loli.net/2019/03/30/5c9f352cd4540.jpg)
## 3.安装vs code插件
需要安装两个vs code插件。
![](https://i.loli.net/2019/03/30/5c9f3643a6475.jpg)
![](https://i.loli.net/2019/03/30/5c9f381d8d1e6.jpg)
## 4.第一个dart项目
新建文件hello_world.dart,输入以下代码
```java
void  main(){

print('Hello World');

}
```
保存点击右上角的运行符号。即可在调试窗口看到打印出来的信息。
![](https://i.loli.net/2019/03/30/5c9f388b136ad.jpg)