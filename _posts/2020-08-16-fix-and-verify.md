---
title: "fix and verify"
date: 2020-08-16
---

上个礼拜optimize一个程序

unit test 过了

用实际数据run了一下

差别也不是很大

但是还是有一些细微的差别

本来觉得是正常

但是决定还是再仔细看看

查一下counters和logs

发现有些不对劲儿

有些的slice完全有错

debug了很久

print out出数据，很明显一些地方出错了

后来把取了一小块出问题的实际数据

放大unit test里面

很快意识到问题所在

bug在std::greater&lt;int&gt;

应该是std::greater&lt;int64&gt;

unit test很少用大的数字，所以没有测出来

这个bug改了以后，再run实际数据就没问题了

所以任何细微的非正常现象都应当仔细调查
