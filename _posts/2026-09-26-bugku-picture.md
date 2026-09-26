---
layout: post
title: "BugKu CTF Writeup-这是一张单纯的图片"
date: 2026-09-26
categories: CTF
---

# BugKu CTF Writeup-这是一张单纯的图片

## 题目类型

MISC

## 题目描述

一张单纯的图片

## 解题过程

下载jpg图片，图片预览看不到flag。使用记事本打开图片，滚动到文件末尾，可以看到一串`&#xxx;`格式的HTML实体编码。
将实体编码放入HTML解码器，得出key。

## 考点

文件尾部附加数据、HTML实体编码解码。
