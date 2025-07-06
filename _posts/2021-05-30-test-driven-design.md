---
title: "test driven design"
date: 2021-05-30
---

最近搞一个project

离deadline越来越近

就开始写launch doc，也在写working doc

想着launch要show什么东西

列了几条关键的metrics和expectation

写完后感觉之前的计划risk非常大，可能会很多该neutral的metrics不neutral，因为infra做了很大的改动，很多细节不一定跟prod一致

如果想要no surprise的话，似乎走另外一条在prod上改动最小的那条道似乎更合适

想了想，决定放弃之前的方向，选取no surprise的这条道

这样内心也更加平安一些

感觉以后也应该这么干，先写test，再回头design，再选取方案，再执行

另外，越来越觉得测试不仅关键，而且是一门技术

大多数人不会进行严格的测试，或者想不出完备的测试计划

测试技巧也是需要经验

也许我今后应该着重往这个方向发展

测试是直接跟项目目标挂钩的

是项目闭环中关键的一个环节

不仅如此，也可以检测出现有系统的问题，并指出改进的方向

其实，所有的metrics，还有monitoring，本身也是测试的一种

monitoring可以看成是continuous testing
