---
title: "Converge to code - poetiq arc agi solver"
date: 2025-12-07
---

GitHub - poetiq-ai/poetiq-arc-agi-solver: This repository allows reproduction of Poetiq's record-breaking submission to the ARC-AGI-1 and ARC-AGI-2 benchmarks. <a href="https://share.google/8g7TP1bFiz3rz9cki">https://share.google/8g7TP1bFiz3rz9cki</a>

<a href="https://poetiq.ai/posts/arcagi_announcement/">https://poetiq.ai/posts/arcagi_announcement/</a>

<a href="https://x.com/i/status/1997366836015366577">https://x.com/i/status/1997366836015366577</a>

So code is the final tool to generalize, to abstract and the machine that solves intelligence problem. And LLM can help write the code, to evaluate the results, to evolve the code, till problem solved.

So basically we have a program that calls LLM, to generate code to solve the problem.

It has a scorer. It has results error feedback, it has some initial sample code.

For next step sampling, it basically add prev successful code as new examples to the prompt.

So it's like a RL algorithm, but in test time.

So likely arc agi test will soon be solved.
