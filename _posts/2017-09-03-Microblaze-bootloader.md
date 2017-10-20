---
layout: post_layout
title: Microblaze bootloader的实现
time: 2017年09月03日 星期日
location: 苏州
pulished: false
excerpt_separator: "```"
---

前一段时间看到一篇博客<<[聊一聊如何实现Xilinx Microblaze Bootloader ](http://blog.csdn.net/haoxingheng/article/details/51295659)>>，然后自己也照着做了一个。基本原理是，上电后FPGA从FLASH中加载bit到内部RAM，bootloader执行，从特定位置将应用程序加载入外部存储器(DDR)中执行。步骤就不写了，照着原博做就可以了。从上电到bootloader开始工作，这段时间因为读写SPI，所以速度比较慢；但是从bootloader开始工作到，指定地址的测试程序开始执行，用时较长，测试程序只有155KB，还不清楚问题原因在哪里。