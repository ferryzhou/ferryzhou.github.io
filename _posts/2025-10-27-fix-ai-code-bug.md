---
title: "fix ai code bug"
date: 2025-10-27
---

prompt enable worker scouting in early game

cursor wrote hundreds of lines in a couple of mins

then i spent several hours to debug and fix issues

very weird behaviors

did many changes, debug but still see the weird behaviors, sometimes different behaviors

finally realized where the bug is

fixed it. just delete ~10 lines of code. which asks the worker to go back when it sees any enemy that can attack ground units. this means that when it sees other workers, it will try to go back. when it didn't see, it tries to move forward. so always move back and forth.

with the fix, the behaviors becomes normal and expected

further fixed a few other issues

now good enough

<a href="https://github.com/ferryzhou/sc2_bots_ares/commit/1d0ce68c1f8df350f7e029c58007a105f71707d0">https://github.com/ferryzhou/sc2_bots_ares/commit/1d0ce68c1f8df350f7e029c58007a105f71707d0</a>

<a href="https://github.com/ferryzhou/sc2_bots_ares/commit/af31647c502205ddcbf3ad5fe1f635270a91ec74">https://github.com/ferryzhou/sc2_bots_ares/commit/af31647c502205ddcbf3ad5fe1f635270a91ec74</a>
