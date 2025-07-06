---
title: "Verification"
date: 2020-06-26
---

最近工作项目时间紧，任务急，跑得比较快，结果就是时不时出bug

程序bug，数据bug

其实避免这些bug的方法很简单

就是verify一下

这两天还碰到一个outage，其实也跟不verify有关系

verify看起来简单，其实需要花功夫，花时间

比如改了程序，起码得run一下看对不对

生成了数据，需要sanity check一下

sanity check有时需要写查询

还得想想查什么

现在能想象，所有的数据都可以尝试去verify，一定能找到很多问题

感觉满世界都是漏洞

而有漏洞的地方就一定有获利的方式～

回到工作上，每个环节都应该加pre check和post check。也就是design by contract。另外，需要monitoring。
