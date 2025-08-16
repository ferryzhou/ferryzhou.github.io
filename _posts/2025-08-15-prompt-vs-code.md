---
title: "prompt vs code"
date: 2025-08-15
---

llm + prompt + tools have issues of

1. non-deterministic results, hallucination
2. inefficiency. tokens processing are costly.

while code don't have these two issues

and because of the two issues, it's hard to scale up complexity.

so code will still essential

one good thing about the new llm agent is mcp that unified interface and enticed all software to open api.

As a result, integration becomes much easier.

however, because of the issues mentioned above, it might be good to have llm agent t + prompt to generate code. like

func handle(prompt):

if code_not_available, generate_code(prompt)
exec(code)

the code generation can have human in the loop.

also the code can call llm for text processing

this can solve the issues mentioned above. it also utilize llm to generate code.

one step further, it should regularly fix / improve code.
