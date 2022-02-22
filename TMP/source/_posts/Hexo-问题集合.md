---
title: Hexo 问题集
date: 2022-02-21 21:29:17
tags: hexo, git
---
# Hexo 问题集
* Hexo 无法发布到远程仓库
```
fatal: unable to access 'https://github.com/Himson/himson.github.io.git/': Failed to connect to github.com port 443: Timed out
```

>本质原因是由于GFW的影响，本地git分支无法发布到github。我们可以使用ssh协议发布分支。具体做法是在config.yml里面修改repo的值。如下例：

    repo: 'git@github.com:Himson/himson.github.io.git'