---
title: "unit test and real test"
date: 2021-01-01
---

最近写代码，每次unitt test基本上都是&gt;95% coverage

以为万无一失了

但是一用实际数据运行就发现结果不对

而且还debug好久

所以real test其实总是必须的

然而real test似乎并没有一个成熟和方便实用的框架

基本上必须得写查询代码做sanity check

或者neutrality test，如果有其他结果的话

简单地说，拿两套系统，分别算出结果，看看结果是否吻合

一般来说，这种方法总是能发现一些问题，有可能会发现已有系统的问题，有可能发现新系统的问题

回到unit test

unit test无论如何巧妙，它并不能涵盖实际数据中的各种可能情况

而且，unit test无法揭示design之外的问题，design本身可能就有问题

之前犯了两个错误，第一是输入数据本身就错了，第二是filter的次序不对。

这两个问题在unit test中是不肯cover的。

regression test上也不能完全cover

可能a/b test才是最全面的方法

或者对serving system的数据直接监控，check sanity
