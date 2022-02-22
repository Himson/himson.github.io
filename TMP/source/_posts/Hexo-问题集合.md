---
title: Hexo 问题集合
date: 2022-02-21 21:29:17
tags: hexo
---
1. Hexo 碰到的无法发布到github
fatal: unable to access 'https://github.com/Himson/himson.github.io.git/': Failed to connect to github.com port 443: Timed out

本质上是本地git分支无法发布到github造成的。这是因为GFW对https的影响造成的。因此我们可以使用ssh协议发布分支。具体做法是在config.yml里面修改repo的值。让他变成ssh协议的github repo的地址 repo: 'git@github.com:Himson/himson.github.io.git'。