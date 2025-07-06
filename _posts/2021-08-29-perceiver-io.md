---
title: "Perceiver io"
date: 2021-08-29
---

<a href="https://github.com/deepmind/deepmind-research/tree/master/perceiver">https://github.com/deepmind/deepmind-research/tree/master/perceiver</a>

这个有点儿意思

模型很general

语言，图像，音频

特别是还能直接应用到optical flow

这个自己以前也做过

感觉有些小震撼，也很好奇

花了好几天去理解这个

但其实好多词都只是听说过但是不懂

比如attention, transformer

然后论文里又出来一堆K, V, Q

没办法，回头一个一个查，找tutorial

<a href="https://theaisummer.com/attention/">https://theaisummer.com/attention/</a>

<a href="https://theaisummer.com/transformer/">https://theaisummer.com/transformer/</a>

<a href="https://theaisummer.com/einsum-attention/">https://theaisummer.com/einsum-attention/</a>

<p dir="ltr"><a href="https://towardsdatascience.com/illustrated-self-attention-2d627e33b20a">https://towardsdatascience.com/illustrated-self-attention-2d627e33b20a</a>

<p dir="ltr"><a href="https://jalammar.github.io/illustrated-transformer/">https://jalammar.github.io/illustrated-transformer/</a>

<p dir="ltr">大概明白是啥情况了

<p dir="ltr">最诡异的是一个input embedding map到三个vector，分别是k, v, q。还说是借用information retrieval的词汇。这就更神奇了。自己search自己么？

<p dir="ltr">感觉完全理解还需要再消化一下。

<p dir="ltr">又仔细看了一下optical flow的描述和代码。

<p dir="ltr">input是两幅图片。output是flow图片。

<p dir="ltr">以前做optical flow基本上都是patch to patch的去找。完全是没有learning的。

<p dir="ltr">现在全是learning based。

<p dir="ltr">这个问题format成一个input output mapping的问题了

<p dir="ltr">通过model来map

<p dir="ltr">Transformer感觉有点儿像图像压缩

<p dir="ltr">一个经典的方法

<p dir="ltr">通过傅立叶变换转到一个space，只需要提取其中少部分值，然后再反变换回来，基本上能跟原始图片差不多

<p dir="ltr">怪不得叫encoder, decoder

<p dir="ltr">整个transformer感觉是一种高度定制化的转换模型

<p dir="ltr">模型通过大量的数据来训练

<p dir="ltr">Perceiver做到通用性的关键在于input 和output弄成最general的array

<p dir="ltr">然后定义专门的preprocessor和post processor把领域数据转换成输入输出。

<p dir="ltr">不知道可不可以应用到工作上？
