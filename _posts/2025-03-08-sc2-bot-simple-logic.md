---
title: "sc2 bot simple logic"
date: 2025-03-08
---

see <a href="https://github.com/ferryzhou/sc2_bots/blob/a28d3dc7040e88fde5f31d1c1d8d2cc8cb69b0f1/han/han.py">https://github.com/ferryzhou/sc2_bots/blob/a28d3dc7040e88fde5f31d1c1d8d2cc8cb69b0f1/han/han.py</a>

basically, every one step, do distribute_workers, then every 10 steps, manage army and manage production.

for manage production, build things if we have money. with rough control on how many to build, based on some simple rules, like x of bases etc.

for army, attack if some condition is triggered, like found enemy or army size is big enough.

less than 300 lines of code, with basic python-sce2 lib, no other frameworks

it can beat Hard computer most of the time.

now have much better understanding how it works, how to do multiple things parallelly.

next we can make it more advanced by adding more functionalities like manage upgrades, add more type of units, intelligent routing etc.
