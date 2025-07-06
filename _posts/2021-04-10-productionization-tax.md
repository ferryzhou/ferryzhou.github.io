---
title: "productionization tax"
date: 2021-04-10
---

最近碰到一个outage

上游的数据出了问题

作为mitigation基本策略之一，加了个validation检测异常

结果这个检测最近时不时报错

但是数据是没有问题的

只不过是organic change

正常的变化

于是得考虑加大threshold

但是这又导致一个悖论

加大threshold会让真正的数据问题被忽略

所以出现两种选择

1. tight threshold。false positive rate就会比较高。但是false negative会低。真正有问题的情况容易抓到。false positive会导致开发人员消耗更多的时间。
2. loose threshold。false positive低。但可能会让问题数据流到下游，引发一场outage。

数据异常既可能是真正的数据问题，也可能只是正常的数据波动。

要分辨这两种不同一般需要看多方面的数据，人工作决策。有可能还需要跟上游沟通。

一般来说，会倾向于选择1。让开发人员承受更多的体力活儿，避免真正的outage。这就相当于程序员被收productionization tax。

当然，还有第三条路，那就是不断优化signal to noise ratio。比如自动分辨数据异常到底是正常波动还是数据问题。但是这又会引入新的风险以及增加复杂度。
