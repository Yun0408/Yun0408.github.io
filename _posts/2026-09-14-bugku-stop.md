---
layout: post
title: "BugKu CTF Writeup-alert"
date: 2026-09-12
---
#BugKu CTF Writeup-你必须让他停下
<br>## 题目类型
<br>WEB
<br>## 题目描述
<br>题目页面会不断自动刷新，页面中存在隐藏的标签，但是因为页面高频自动刷新，无法直接查看源码。需要想办法阻止页面自动刷新，获取flag。
<br>## 解题过程
<br>浏览器禁用，访问题目页面，按下 F12 打开开发者工具，使用快捷键  Ctrl+Shift+P ，调出命令面板，输入  Disable JavaScript ，点击执行，关闭页面JS执行，此时定时器失效，页面不会自动刷新。手动按F5刷新页面，多次刷新，当页面图片加载为 10.jpg 时，查看页面源代码，即可找到flag。
