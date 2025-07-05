---
title: "Config, proto and language"
date: 2025-02-23
---

早上半梦半醒中意识到简化的一种基本方式甚至普遍方式是config

config可以轻易的表达成一个数据结构，一个class，一个存储对象，一个protobuf，一个树，一个可以容易读取和查询的对象，一个容易specify的对象

JSON, yml, XML, protobuf, html

人可以简单的读写

机器也可以简单的读写

config可以看成最基本的domain specific language

是declarative的

我们填写的各种表格都是一种config

任何人都能够填写和修改表格

config是一种封装

可以看成是一种API

用户不需要了解API是如何实现的

计算机代码也可以看作是一种config

config的数据就是语法树

编译就是把高级语言的config翻译成低级语言的config

我们在开发系统的时候，

如果写的config太boilerplate, 可以考虑创造一个新的config，用程序把它转换成低级的config

这样会增加可读性，可修改性，以及开发时间

如果写config有很多限制和不方便，特别是复杂的信息

那么可以考虑语言化

计算机程序语言其实就是把复杂的config填写变成了用语言来去写

比如Google的gcl

<a href="https://2023.splashcon.org/details/conflang-2023-papers/7/Evolving-a-configuration-language-in-place-at-Google-scale">https://2023.splashcon.org/details/conflang-2023-papers/7/Evolving-a-configuration-language-in-place-at-Google-scale</a>

一个神经网络模型架构，内部也是一个庞大的config

各种API也都是简化了config的编写。

模型train完的数据，也是个config

可以被加载，复制和调用

config也可以被编译，在各个不同的硬件平台上运行

硬件和软件得以彻底解耦
