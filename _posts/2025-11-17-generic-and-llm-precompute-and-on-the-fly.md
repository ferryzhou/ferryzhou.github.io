---
title: "generic and llm, precompute and on the fly"
date: 2025-11-17
---

继续前一篇

so the written code is like precomputed data or cache

one good thing about llm / agent is it can generate code on the fly and then run it

so code is abstracted as a string

and it's much more generic than written code

this is something traditional software system usually don't have

traditional software might have templates, functions, args,

but still rigid, predefined, hard to change or extend

llm / agent make it more generic

user specify prompts as input, code are generated dynamically and executed

now the question is how to balance flexibility with complexity and certainty, or it can co-exist

another point is that llm / agent unified and simplified UI

traditionally, software has too many buttons, many settings,

with llm / agent, those can be accessed through prompts
