---
title: "data/model correctness and freshness, search and market"
date: 2021-07-11
---

感觉这两个指标是核心

拿这两个指标去看一般可以看到绝大多数问题

freshness比较好定义

correctness类似于测试

之所以看这两个指标是因为他们都很困难

从数据采集到最终数据呈现，到模型训练，再到模型serve，这里面的链条往往很长，且容易出错

数据不fresh，预测就会出偏差

数据不对，预测也会出偏差，理解都会出偏差

互联网把对数据的要求提升了好几个维度

互联网本质是无边界无延时的信息流动平台

有了互联网，机器的边界被打通，scalability被解放

人的边界也被打通，交互不再局限于物理世界

人与世界的边界也被打通

从某个角度来说，互联网公司的通用模型是把现实或者虚拟世界的信息通过应用程序采集到平台，再通过信息处理促进交易的完成或者高质量信息的获取。

每一个平台都是一个market，汇集买方和卖方

平台的任务是降低买卖双方的交易成本，包括时间成本，空间成本和金钱成本

成本下降，更多的买家和卖家涌入，市场扩大，交易量上升，经济体量得以扩大

无论是电子商务，打车软件，交易软件，视频网站，外卖软件，直播，交友都可以通过market的方式去看待

所以互联网促进了经济的发展，

而手机则促进了互联网的发展

平台的核心是匹配和预测

query过来，response回去

一个简单的调用，涉及到成千上万的演算

数据差错，模型差错，都会导致结果的不理想，导致交易效率的下降，成本的增加，进而导致平台质量的滑坡，信任度的下降，收入的损失

当平台搜索引擎化，搜索引擎也正在market化

google越来越像电商，youtube越来越像google

早期互联网，网站，博客是卖家，搜索用户是买家，google是market。

电商流行后，电商本身成了商品的搜索引擎。

移动互联网的发展让更多的交易场景挪到了互联网世界里。买菜，打车，外卖，直播。每个交易场景都是一个market。每一个market都需要一个搜索引擎。

当然，更重要的是，每一个market都需要给卖家带来收益。

google通过adsense，直播通过打赏，外卖通过买家支付

没有收益，创作者就会流失，内容就会枯竭

因而平台会想尽各种办法吸引创作者或者卖家

另一方面，收益又与用户基数相关

用户的浏览量本身是一种价值

因而平台会想尽办法提升用户体验，mostly信息查询的质量

response delay, top results relevance

用户点击的每一个内容，本身也是一个query，加上他的history

平台提供 recommended items

用户被投食，多巴胺被持续刺激，因而困在系统之中

人进入市场，本来只是为了寻找一件东西，却不经意间被卷入大海之中

好吧，扯得太远了
