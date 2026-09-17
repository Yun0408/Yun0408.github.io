---
layout: post
title: "BugKu CTF Writeup-"
date: 2026-09-16
categories: CTF
---

# BugKu CTF Writeup-

## 题目类型

WEB

## 题目描述

访问页面，页面给出PHP源码。

## 解题过程

构造POST请求，提交参数 what=flag 。

cmd执行。curl -X POST -d "what=flag" http://160.202.254.160:12423。请求成功后，返回页面输出flag。

## 考点

POST传参， $_POST 读取请求体内的参数，参数无法直接放在URL地址栏。
