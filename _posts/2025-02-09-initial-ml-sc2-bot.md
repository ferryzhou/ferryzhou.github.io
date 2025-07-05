---
title: "initial ml sc2 bot"
date: 2025-02-09
---

<a href="https://github.com/ferryzhou/sc2_bots/tree/main/han">https://github.com/ferryzhou/sc2_bots/tree/main/han</a>

started with <a href="http://claude.ai">claude.ai</a>

genai is good at build initial code. and then needs some fixes to make it runnable. for further improvement, also need deep knowledge as ai still has hallucination issues. it still saved lots of time though. very impressive. it periodically runs manage_production which is critical. so far the bot can expand, build army and attack. not too bad.

the model is a four layer dnn with state as input and 5 actions as output. the actions are build army or expand or attack or train worker. currently, the output is pretty random. it also defined reward function, not in effect yet. i don't have tons of training resources, each run is very costly, takes lots of time. so need to think about intelligen way to make training efficient.

My prompts:

<ul>
<li>want to write a bot to play starcraft2, and use machine learning, how to do that?</li>
<li>can you use python-sc2 library instead of pysc2 lib?</li>
<li>improve the bot that can keep improving the model by running many games.</li>
<li>I didn't see on_step function. also didn't see how reward are used. could you fix the issues.</li>
<li>AttributeError: 'SC2MLBot' object has no attribute '_build_or_load_model'. please fix the issue.</li>
</ul>

There are some importing errors and use async for main function, which needs to be fixed. otherwise mostly good.

The initial ML bot is dumb. actions needs to be improved.
