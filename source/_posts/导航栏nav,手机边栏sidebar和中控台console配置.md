---
title: '导航栏nav,手机边栏sidebar和中控台console配置'
cover: 'https://img1.acrylic.org.cn/2023/04/16/643b6a036a2cb.webp'
top_group_index: 3
abbrlink: ba6f
date: 2023-03-25 11:28:50
updated:
categories:
tags:
description:
keywords:
layout:
comments:
---

## 导航栏 (nav)

![](https://acrylic.leonus.cn/i/2023/03/25/sf4qz4.webp)
![](https://acrylic.leonus.cn/i/2023/03/25/sf54ax.webp)
![](https://acrylic.leonus.cn/i/2023/03/25/sf5f31.webp)

```yml
# 导航栏 (nav)
# ------------------------------------
nav:
  left_groups:
    enable: true
    group:
      - title: 博客
        a_item:
          - text: 主页
            link: https://zhheo.com/
            img: https://p.zhheo.com/20232e121c3fb2daa71897d26a515e030f49073402.png!cover_mini
            class: out
          - text: 博客
            link: /
            img: https://p.zhheo.com/20234681e06b8e086aa5b15481cb89fd38c7071002.png!cover_mini
            class: out
          - text: 图片博客
            link: https://plog.zhheo.com/
            img: https://p.zhheo.com/20236a16354d7c333cc7595efaee4b8c5667074602.png!cover_mini
            class: out
          - text: 开发博客
            link: https://apps.zhheo.com/
            img: https://p.zhheo.com/2023042bb31614949504f9ac59b134ce971d075802.png!cover_mini
            class: out
  logo: 
    enable: true
    class: i_class #i_class/text/img 
    custom: heoicon icon-heologo #Heo/https://xxx.com/logo.png
  fps_enable: true
  menu:
    文库:
      文章列表: /archives/ || fas fa-box-archive
      全部分类: /categories/ || fas fa-cube
      全部标签: /tags/ || fas fa-tags
      即刻短文: /essay/ || fas fa-bars-staggered
    专栏:
      设计报告: /tags/设计报告/ || fas fa-swatchbook
      设计分享: /tags/Heocan/ || fas fa-object-group
      设计工具: /tags/Sketch/ || fas fa-palette
      视频混剪: /tags/混剪/ || fas fa-scissors
    友链:
      友链鱼塘: /fcircle/ || fas fa-fish-fins
      友情链接: /link/ || fas fa-user-group
      宝藏博主: javascript:travelling() || fas fa-bus
    我的:
      在线工具: /tlink/ || fas fa-screwdriver-wrench
      电影推荐: /movies/ || fas fa-clapperboard
      关于本站: /about/ || fas fa-sailboat
  right_button:
    travelling: true
    random: true
    console: true
```
## nav.left_groups.group
  1. `title`: 大组标题
  2. `text`: 显示文章
  3. `img`: 显示图像
  4. `link`: 链接
  5. `class`: 站内(in)或站外(out)
## nav.logo.class
  1. `i_class`: 图标
  2. `text`: 文字
  3. `img`: 图片
## nav.menu
  同butterfly一样
## nav.right_button
  1. `travelling`: 开往
  2. `random`: 随机文章
  3. `console`: 中控台

## 手机边栏 (sidebar)
![](https://acrylic.leonus.cn/i/2023/03/25/uahf14.webp)
![](https://acrylic.leonus.cn/i/2023/03/25/u9858n.webp)

```yml
# 手机边栏 (sidebar)
# --------------------------------------
sidebar: 
  list_group: true
  tag: true
```

## 中控台 (console)

![](https://acrylic.leonus.cn/i/2023/03/25/udw67v.webp)

```yml
# 中控台 (console)
# --------------------------------------
console:
  comment: true
  tag: true
  archives: true 
```
1. `comment`:最近评论
2. `tag`: 标签
3. `archives`: 归档