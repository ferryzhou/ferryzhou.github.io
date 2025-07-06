---
title: "prediction and quality, truth and light"
date: 2020-12-06
---

最近搞launch检查quality，发现一些简单的问题却不是很容易回答，下个礼拜就要review了，心烦意乱，先把思绪整理一下

主要的问题是，launch candidate跟prod结果很不一样，如何能知道哪个更好呢？

从最开始launch candidate就改了很多东西，label不一样，signals不一样，中间一些环节也不一样

整个prediction中间的链条很长，从数据预备，预处理，模型训练，serving prediction，adjustment，sampling，post-processing等等。

一般来说，prediction有通用的quality metrics，比如bias, auc

但是一个实际应用里还有大量的领域逻辑，相关的处理，很多的环节

最近意识到一个关键点，那就是observed data

observed data就是ground truth

truth is always unique, not changed

observed data就是那个north star

而prediction本质上是estimate something that is not revealed yet

比如未来是什么。明天会下雨吗？股票会涨吗？新冠疫情会在年中结束吗？年内能出疫苗吗？特朗普会当选吗？

在现在对未来作预测，未来还没有revealed，时间线越长，预测会越不靠谱。但是未来迟早会来。truth will finally revealed。

还有一种是对过去做预测。比如破案。已发生的事情，但是天知地知你不知我不知只有当事人知。可以从一些蛛丝马迹来推断事情的真相。也可以通过关键证人来揭示真相。

比如大选有舞弊吗？比如双十一商家销售额灌水了吗？

有ground truth，reveal the truth同样重要。不然就仍然是unknown。

reveal the truth needs light

measurement, image, sound, words, broadcasting, are all part of light

but there are many lies, and many people covers the truth, they destroy evidence, kill witness, make false claims, magnify non-critical issues, muddy the water

圣经说truth set you free, lies enslaves you

without truth and light, you will be in darkness and be blind, and thus easy to fall into trap
