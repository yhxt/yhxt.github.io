---
layout:     post
title:      [技巧]如何使用Navicat Pertmium连接oracle数据库
subtitle:    "\"Hello World, Hello Blog\""
date:       2018-03-02
author:     YH
header-img: img/post-bg-2015.jpg
catalog: true
tags:
    - Mysql
    - 运维
    - 数据库
---


## 第一步

第一步当然是安装Navicat Pertmium工具了，软件的下载以及安装方法，随便搜一下一大堆，我就不在此进行赘述了。

---

## 第二步

打开Navicat Pertminm连接工具，点击“文件”——新建连接——oracle,如下图所示：
![图一](http://upload-images.jianshu.io/upload_images/545178-8bef87fb1bec398a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
接下来根据提示输入数据库的相关信息即可，但是此时输入正确后连接会出现一个错误提示，具体如下图：
![图二](http://upload-images.jianshu.io/upload_images/545178-5089dd18886f5f4e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图三](http://upload-images.jianshu.io/upload_images/545178-d1c7984e354cda1f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
该问题是直接使用Navicat自带的instantclient_10_2造成的。自带的采用的是Basic Lite版本的instantclient。

### 第三步
解决上述问题：
下面就需要登录oracle官网，下载Instant Client,下载地址如下：

[下载地址](http://www.oracle.com/technetwork/cn/topics/winsoft-095945-zhs.html)
![图四](http://upload-images.jianshu.io/upload_images/545178-2e9589af2e25a985.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


### 第四步
将下载的文件解压，解压后的文件放到Navicat Pertminm的安装目录，并在Navicat Pertminm 工具——选项——OCI里面修改地址，如下图所示：
![图五](http://upload-images.jianshu.io/upload_images/545178-74f1af470bd2b10c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---

主题我直接 Downlosd 了 [Hux的博客主题](https://huangxuan.me/) 的进行修改，简单粗暴，不过遇到了很多坑😂，好在都填完了。。。

本地调试环境需要 `gem install jekyll`，结果 rubygem 的源居然被墙了，~~后来手动改成了我大淘宝的镜像源才成功~~，淘宝的源已经[停止维护](https://gems.ruby-china.org/)，换成了OSChina的源 `https://gems.ruby-china.org/`。
注意：修改后必须重启工具，重启后测试连接即可

### 第五步
再进行连接测试，显示连接成功即大功告成啦~~~
![图六](http://upload-images.jianshu.io/upload_images/545178-664bf00f8f1181ac.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

最后，[给个 star 吧](https://github.com/yhxt/yhxt.github.io)~



