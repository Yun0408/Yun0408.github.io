---
layout: post
title: "Bugku CTF Writeup-计算器"
day: 2026-09-11
---
#Bugku CTF Writeup-计算器"
##题目类型
<br>WEB
<br>##题目描述
<br>题目首先会给出一个两位数的运算，但验证框的答案只能输入一个字母
<br>##解题过程
<br>进入源代码，发现"maxlength=1"，意味着只能输入一位数字。右键检查后，将"1"换位"2",意味着将可输入的运算结果改为两位数字，即可得出正确答案与flag。

