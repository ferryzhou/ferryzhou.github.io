---
title: "Flooding and 7 ideas to handle complexities"
date: 2023-01-15
---

最近连绵大雨

很多地方开始flooding

河水涨的很厉害

昨晚看工作email

往回看了很多

感觉一天好几百封邮件

很容易错过一些重要的

特别是那种半夜凌晨发的

email flood

但是平时每天又忙着开会，处理很多必须处理的事情

时间又是有限的

requests太多

所以很多会drop掉

做了manager或者scope更大以后这种状况更加明显了

用之前的machine或者server角度出发

就是throughput不够了

感觉complexity或者flooding主要有两个维度

第一是scale，就是数量

第二是tight deadline，就是时间

数量除以时间就是throughput，或者是流量

流量超过throughput就会造成flooding

server的throughput不够用就会出问题

程序员的一个重要衡量指标是提交的程序代码速度

如果每天都有代码提交，说明throughput不错

而manager，tech lead对上级或者领导们重要的impression就是回话的速度。是否领导问的问题有答案，是否项目都能顺利推进。

如何提高throughput呢？

第一cache

重用？很多的request，虽然是从不同地方来的，但是问的是同一个问题，或者是类似问题

所以应该有一个内部的文档

每次外部request来，直接返回文档里的信息

而不是从头开始想

内部文档也是一种cache

第二，预测，筹谋

很多的请求或者任务都是有时间段的

比如okr，比如perf，会发生在特定的时候

从下一周的meeting也可以知道什么需要做

根据预测即将到来的请求，提前做好准备

第三，增加工作时间

白天开会，只能晚上和周末干活

第四，delegate或者load balancing

手头有资源，就尽量派发任务，尽量让其他的server处理

第五，prioritize

丢弃掉不重要的request

第六，重构，复用和优化

把adhoc的行为自动化，比如用程序取代manual，hardcode信息变量化

第七，让团队成长

grow团队里的每一个人

让每个人的throughput变得更好
