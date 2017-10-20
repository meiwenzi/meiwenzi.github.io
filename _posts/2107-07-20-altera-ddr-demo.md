---
layout: post_layout
title: Altera DDR IP 的使用（基于Arria 10）
time: 2017年07月20日 星期二
location: 苏州
pulished: true
excerpt_separator: "```"
---

# 一、DDR ip的生成
1.在ip Catalog下选择 Arria 10 External Memory Interfaces 
设置名称、存放路径，如下图：

![ddr_newipvariation.PNG](https://i.loli.net/2017/10/18/59e763a4a0b9b.png)

2.根据选用的DDR型号设置相关参数

![ddr_general.PNG](https://i.loli.net/2017/10/18/59e766ac27647.png)

具体参数设置不赘述

还可以使用预先布置模板，如下图

![ddr_presets.PNG](https://i.loli.net/2017/10/18/59e7697458d21.png)

3.生成ip。如下设置
![ddr_ge.PNG](https://i.loli.net/2017/10/18/59e76d5d9a71c.png)

4.生成参考设计

![ddr_ged.PNG](https://i.loli.net/2017/10/18/59e770611bfb0.png)

# 二、DDR ip的调试

## 1、验证

找到生成的参考设计的目录，打开参考设计的工程

![ddr_lujing.PNG](https://i.loli.net/2017/10/18/59e7721eeedd4.png)

可以将下图中的信号外接到led 灯上，用于指示状态，由这几个状态，判断DDR ip 是否可用。确定IP没问题之后，参考设计也可以用于DDR 的检测。

![ddr_test_port.PNG](https://i.loli.net/2017/10/18/59e772835cd5a.png)

## 2、仿真

# 三、DDR ip 信号及操作时序解析

(待更)

