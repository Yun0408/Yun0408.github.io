---
layout: post
title: "BugKu CTF Writeup-聪明的小羊"
date: 2026-10-09
categories: CTF
---

# BugKu CTF Writeup-聪明的小羊

## 题目类型

Crypto

## 题目描述

一只小羊翻过了2个栅栏 fa{fe13f590lg6d46d0d0}

## 解题过程

题目提示“翻过了2个栅栏”，栅栏是栅栏密码的标志性提示，确定为2栏栅栏密码。栅栏密码加密原理：将明文字符分行写入栅栏，之后按行拼接得到密文；解密则将密文对半分割为两行，交替取出每行字符还原明文。
使用Bugku自带栅栏密码工具解密，得出flag。

