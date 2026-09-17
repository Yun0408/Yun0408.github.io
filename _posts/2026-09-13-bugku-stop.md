---
layout: post
title: "BugKu CTF Writeup-你必须让他停下来"
date: 2026-09-13
categories: CTF
---

# BugKu CTF Writeup-你必须让他停下来

## 题目类型

WEB

## 题目描述

题目页面会不断自动刷新，页面中存在隐藏的标签，但是因为页面高频自动刷新，无法直接查看源码。需要想办法阻止页面自动刷新，获取flag。

## 解题过程

访问题目页面，按下 F12 打开开发者工具，使用快捷键 `Ctrl+Shift+P`，调出命令面板，输入 `Disable JavaScript`，点击执行，关闭页面JS。此时页面停止自动刷新。反复手动F5刷新页面，当页面图片为`10.jpg`熊猫图片时，查看网页源码，即可找到flag。


