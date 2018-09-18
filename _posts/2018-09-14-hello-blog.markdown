---
layout:     post
title:      "Welcome to ZFelinae Blog"
subtitle:   " \"Hello World, Hello Blog\""
date:       2018-09-14 10:00:00
author:     "ZFelinae"
header-img: "img/post-bg-2015.jpg"
tags: [生活]
---

> “我来了咕咕”


## 前言

ZFelinae 的 Blog 就这么开通了。

都2018年了，小猫总算有个地方可以好好写点东西了~~(还是不怎么会写)~~。


作为一个程序员， Blog 这种轮子要是挂在大众博客程序上就太没意思了。一是觉得大部分Blog服务都太丑，二是以前也没有想过要写点东西什么的~~，三是懒~~。

公司的前辈给了我做个博客的提议，刚好这几天闲着没事，就自己照着网上的教程搭了一个，感觉超级简单~~虽然还有好多🐞~~。

<p id = "build"></p>
---

## 正文

接下来说说搭建这个博客的技术流程。  

第一步是[百度](https://www.baidu.com/)，当然你也可以用[必应](https://cn.bing.com/)或者[谷歌](https://www.google.cn/)。

不会的东西就去学，学不懂就去找人问，再不懂就放弃————小猫做事三部曲

在许许多多的教程中我选择了[GitHub Pages](https://pages.github.com/) + [Jekyll](http://jekyllrb.com/) 快速 Building Blog 的技术方案，其优点非常明显：

* **Markdown** 带来的优雅写作体验
* 非常熟悉的 Git workflow ，**Git Commit 即 Blog Post**
* 利用 GitHub Pages 的域名和免费无限空间，不用自己折腾主机
* 如果需要自定义域名，也只需要简单改改 DNS 加个 CNAME 就好了
* Jekyll 的自定制非常容易，基本就是个模版引擎

如果说有什么缺点的话就是我想换个新的[github](https://github.com/)账号来搭但是卡死在了注册界面~~(被限制了ip访问)~~，只能把旧帐号的用户名改了(副作用超级麻烦)。

---

配置的过程中也没遇到什么坑，基本就是 Git 的流程，相当顺手

大的 Jekyll 主题上直接 fork 了 Hux Blog（这个国人开发的主题相当有名，就不多赘述了。）

本地调试环境需要安装 [ruby+devkit](https://rubyinstaller.org/downloads/) ，然后`gem install jekyll`以及jekyll的几个插件，都很简单。

然后把项目中 *_config.yml* 文件的各项配置完善，就可以开始**写博客**了。

接着我就遇到了一个超级想死的问题：** *.markdown* 文件放入了 *_post* 目录，本地调试并没有生成新的文章,但是推送到 github 上却生成了。**

**~~绝望.jpg~~**

询问了搜索引擎后发现，是 `timezone` 的问题，但是我正确地安装了插件并且添加了 `timezone:+800` 依然会报错。

于是乎我现在加入文章调试时要把时间提早1天，然后推送时再改回去~~(好麻烦)~~。

如果各位看官有知道怎么解决这个问题的，希望可以教教我，小猫在这里跪谢了orz。

(目前评论功能还未开启，因为我知道根本就没人看)

---

## 后记

回顾这个博客的诞生，纯粹是刚好闲着没事干被人提起建个博客之类的。

我决定以后一周至少更两篇学习笔记或随笔~~(咕咕预定)~~。

我好咸啊_(:з)∠)_

—— ZFelinae 后记于 2018.09
