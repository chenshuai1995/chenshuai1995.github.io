title: Hexo支持TOC效果
author: Jim
tags:
  - Hexo
categories:
  - 工具
date: 2019-09-29 11:30:00
---
<!-- toc -->


# 安装

首先安装hexo-toc的插件，代码如下：

```
npm install hexo-toc --save
```

# 配置
然后，配置一下${HEXO_HOME}站点配置文件_config.yml:

```
vim ${HEXO_HOME}/_config.yml

toc:
  maxdepth: 3
  class: toc
  slugify: transliteration
  decodeEntities: false
  anchor:
    position: after
    symbol: '#'
    style: header-anchor

```
- symbol的#可以去掉


# 使用

在Markdown文章中加入TOC的占位符：以前[toc]\[TOC]改成下面的方式：
```
<!-- toc -->
```