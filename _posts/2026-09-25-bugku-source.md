---
layout: post
title: "BugKu CTF Writeup-source"
date: 2026-09-25
categories: CTF
---

# BugKu CTF Writeup-source

## 题目类型

WEB

## 题目描述

访问页面，页面内容简单。查看网页源代码，注释存在假flag，提示tig（git倒写）。直接访问flag.txt得到的是虚假flag。
考点：git源码泄露漏洞，需要从git的历史提交记录寻找真实flag。

## 解题过程
1. 访问`靶机地址/.git`，确认存在git目录泄露。
2. 使用git-dumper工具，下载整个.git仓库文件。
3. 进入仓库目录，执行`git reflog`查看所有历史提交记录。
4. 使用`git show [commit哈希]`，依次查看每次提交的文件内容。
5. 在其中一条历史提交记录中找到真实flag。

## 疑问
感觉flag是莫名其妙安了一堆软件之后刷出来的，并不知道我的具体哪些操作是有效的......
