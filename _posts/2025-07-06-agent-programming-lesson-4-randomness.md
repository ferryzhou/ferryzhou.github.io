---
title: "Agent programming lesson 4 - randomness"
date: 2025-07-06
---

Given the same prompt, the LLM output could be random

So working once doesn't mean it works the next time

this includes every step, including tool calling

maybe most of the time, the generated tool calling is right, but sometimes it could be wrong

when it's wrong, it could correct itself from wrong results

but it didn't remember the lesson, and can mess it up again next time

a good agent should learn from its own experiences

like cache the tool calling history and results, from there, summarize and store it as long term knowledge memory

besides learning from wrong tool calling results, it should also learn from human feedback

like humans provide good or bad signals on response results.

do rlhf is expensive. not sure whether make it as part of context could be easier.
