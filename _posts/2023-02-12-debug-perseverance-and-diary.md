---
title: "Debug, perseverance and diary"
date: 2023-02-12
---

最近一个pipeline老是overrun

经常fail

昨天晚上又花了一些时间调查原因

到处看数字，log

来来回回假设找证据

感觉应该是抓住最终的原因了

最开始以为的关键点其实不是bottleneck，bottleneck在更上游

让model owner调一个参数看行不行

也让owner总结一下所有试过的办法，以及如何trace

感觉程序员的一个必要修养就是不解决问题不罢休，然后能总结成经验并在下次遇到问题的时候能快速解决。这样自然而然就成为专家了。

下次招人的时候可以考虑问一个问题，就是让面试者谈一谈解决难题的故事。
