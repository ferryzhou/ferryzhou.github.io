---
title: "lending club"
date: 2020-04-05
---

一两年前把lending club关了

这几天查金融危机相关的一些东西，发现了一些新的东西

return比想象中的多

另外，可以download data

然后，发现这个investing很有意思，跟工作接触到的东西有些类似

本质上需要market optimization

一个note相当于一个mini invest

interest越高，risk也越大

这个interest，也许也是根据平均risk算出来的

有意思的是，可以download的data包含了很多信号

这就是一个典型的机器学习问题了

需要做Prediction

prediction的质量决定了你的return比平均高还是低

平台提供了一个baseline

你可以用它的baseline，就是自动选择一个策略，平台帮助你去自动从不同级别的note去选

这个baseline大致是5%左右。作为普通用户会低一些。

如果你发现了一个好的策略，或者模型更好，你的Performance会远远高于baseline

那么模型好的表现是什么？

简单地说，一个risk高的note，你预测risk低，实际也低。那么，在这个note上你会得到更高的收益，因为default比想象低。更白话一些，100个notes，系统预测default rate 20%，利息30%。那么平均下来80*1.3=104。预测准的话，return是4%。如果你预测default rate 10%，和实际一致。那么90*1.3=117%。你的return就是17%！

其实现在已经有模型公司出来了，比如<a href="https://www.lendingrobot.com/#/">lending robot</a>。

最给力的是lending club竟然把data open出来了。
