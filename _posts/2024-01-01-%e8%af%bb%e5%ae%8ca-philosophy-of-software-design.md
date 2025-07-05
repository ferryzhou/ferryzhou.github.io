---
title: "读完a philosophy of software design"
date: 2024-01-01
---

圣诞节旅行，终于有点儿时间读完一本书

本来是买了tidy first? ，然后Amazon推荐了这本，看到评价不错。而且主题或者说perspective跟我很match，也就是如何handle complexity，很好奇他是怎么拆解的。就买来看看。

感觉很有收获。

颠覆了一些以前学到的东西，特别是agile, clean code 里学的。这本书也专门有一章讲这个。

这本书从一个问题开始，how to minimize with complexity?

第二个问题是complexity 到底是什么？如何衡量？

作者的定义是anything that makes it hard to understand and modify.

这个跟前面读的tidy first? 类似。不过加了一条，就是是不是hard to understand 。

这个视角很不错。

其实clean code 也强调代码要易读

不过直接把可理解性与complexity 对等起来还是第一次看到

非常认同这个观点

从这个角度也带出很多新的原则

比如cognitive load和unknown unknowns ，是complexity symptoms，除了change amplification

而complexity的causes，除了dependencies ，还有obscurity

接下来书中聊了很多具体的principles或者strategies

比如deep module, abstraction, generic interface, use defaults, reduce specifics, reduce exceptions, reduce or simplify caller code, move responsibilities to developers, use clear good names, write comments,

avoid too many small classes, small methods, pass throughs, getters and setters,

回头说一下颠覆的东西

比如太多的small methods, small classes 并不好，因为会让代码难以理解。这个深有同感。

另外提一下，作者并不是大厂出身，而是大学里的教授，很多实例是从教学经验出发。因而很多工业界里的问题并没有接触到。不过教学经验也是很好的经验。

最后，这篇blog也总结了一下这本书，值得一看 <a href="https://blog.pragmaticengineer.com/a-philosophy-of-software-design-review/">https://blog.pragmaticengineer.com/a-philosophy-of-software-design-review/</a>
