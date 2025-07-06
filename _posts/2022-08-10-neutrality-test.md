---
title: "Neutrality Test"
date: 2022-08-10
---

最近接触到的好几个项目都碰到了neutrality的问题

结果不neutral

发现大部分人都无从下手

然后项目就被卡住

Non neutral 就像两个系统输出的结果是否一样

很多时候，可能中间有一些randomness

或者，输入有细微的不同

在输出不neutral的时候，能不能够顺藤摸瓜，把问题找出来，这是非常关键的一个能力

需要衡量系统中的不同关键节点

每个关键节点都需要做neutrality test

一个最简单的neutrality test，就是比较absolute count，overall and per slices

关键节点的测试，又需要把数据弄出来

以及关键的signals，比如日期

另外，如果不neutral，需要知道原因，并能改进系统，去除掉不neutral的因素

这些都需要对系统有很深入的理解
