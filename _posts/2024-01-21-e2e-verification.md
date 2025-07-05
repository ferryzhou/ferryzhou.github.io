---
title: "E2E Verification"
date: 2024-01-21
---

Principle 1, don't assume (it works), always verify.

Principle 2, always verify end2end.

Principle 3, be comprehensive. Check every slices.

Principle 4, always follow up on unverified items.

Principle 5, setup monitoring and alerts.

// 最近工作上意识到好几个事情都是漏了verification。

// 感觉作为TL或者manager的一个关键职责就是把verification卡好。从一开始就set up verification expectations，跟test driven 一样，测试先行。不要说什么不ready就没法测试却没法看数据。先把数据和测试都搭起来再说。系统可以慢慢开发，bug可以慢慢改。这个跟metrics driven也是一样。unit test其实也是metrics driven 的一种。set up expectations first.
