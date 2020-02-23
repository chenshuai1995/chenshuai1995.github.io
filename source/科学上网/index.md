title: Ubuntu18.04 使用Shadowsocks 科学上网
date: 2019-10-13 10:25:31
---
[TOC]

<!-- toc -->

# Ubuntu18.04 使用Shadowsocks 科学上网

## 安装shadowsocks-qt5

````
sudo add-apt-repository ppa:hzwhuang/ss-qt5
````

编辑`/etc/apt/sources.list.d/hzwhuang-ubuntu-ss-qt5-bionic.list` 文件，将`bionic `(18.04版本代号)改成`xenial`（16.04版本代号）

因为shadowsocks-qt5 现在还没有提供Ubutnu18 这个版本的客户端，修改源来安装

```
sudo apt-get update
sudo apt-get install shadowsocks-qt5 
```



## 配置网络代理

### 火狐浏览器

firefox-设置-网络代理-设置如下

修改为：手动配置代理：SOCKS主机：127.0.0.1，端口：1080。使用SOCKS v5方式



### 谷歌浏览器

使用[proxy Switchsharp](https://www.switchysharp.com/file/switchysharp-v1.10.4.zip)插件，设置火狐浏览器类似。

**这里有一点要注意，要在插件，也就是浏览器左上角的小地球图标上点击——设置连接，否则是不进行代理的**