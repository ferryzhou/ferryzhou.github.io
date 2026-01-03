---
title: "Code as binary"
date: 2025-11-09
---

So llm or agent based execution is very inefficient

Many of the prompts could be repetitive

Llm could help construct intermediate code or chain of tool calls based on concise prompts

But build those and execute those every time from scratch is slow, wasteful and error prone.

Those intermediate generated logic, code should be cached, and be optimized

The intermediate data should also be cached.

We can treat those generated code as complied byte code or binaries. The prompts is the source code.

Different from traditional programming, the prompts can be written as natural language. And you don't have to worry about many technical details as those can be inferred by llm.

The prompt code is mostly business logic, but still needs to have essential details, to avoid ambiguities that cause errors.

Separately, the generated code should be cached, improved. It's fixed points. It's essential.

Not only for efficiency. But also for correctness.

Efficiency is more than efficiency, it enables scaling up of complexity.

Correctness also enables scaling up of complexity.

prompt -&gt; code is similar to code -&gt; assembly, to assembly -&gt; binary.

all follows the rule of reducing complexity with higher level concepts, further away from machine details.

machine details should be handled by compiler / translator

llm is similar to compiler

however, llm is not deterministic, hard to predict, and need a good results evaluator to make sure solution is correct.

so how far can we make complicated code with prompt, and ensure the generated code is what we need, every time? and how to tune prompt to fix issues or enable some functionalities without changing the code itself, like we never change binary code?

with generated code, we can tell llm / agent to reuse the generated code, without regenerating it again.
