---
title: "RLHF和evaluation"
date: 2024-10-06
---

YouTube上查了一下

关键点是弄了一个reward model，根据人的评分

然后拿这个reward model来评价模型输出

然后反向传播来调整模型参数

这个过程也称为ppo

<a href="https://spinningup.openai.com/en/latest/algorithms/ppo.html">https://spinningup.openai.com/en/latest/algorithms/ppo.html</a>

想起来工作上的事情

也是搞模型

其实最关键的就是quality evaluation

任何跟quality相关的work都需要evaluation metrics

但是往往这个evaluation并没有拿来做反向传播

只是用于最终结果呈现，然后手工调整一些东西

模型的训练依赖于holdout data

而serving traffic往往没有直接的ground truth

其实是可以考虑一些间接的评价数据或者函数的

另外是结果最终的output是在bidding端

这个feedback loop其实很长

不同模型还owned by不同的teams

从train到输出到bidding到用户反馈这个时间也很长

而最终的eval metrics又是什么呢？

继续搞eval吧。

另外真的得转deep model了。
