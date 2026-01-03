---
title: "simonw tools and dev from phone"
date: 2026-01-03
---

<a href="https://simonwillison.net/2025/Dec/31/the-year-in-llms/#the-year-of-programming-on-my-phone">https://simonwillison.net/2025/Dec/31/the-year-in-llms/#the-year-of-programming-on-my-phone</a>

&quot;I wrote significantly more code on my phone this year than I did on my computer.&quot;

&quot;My <a href="https://tools.simonwillison.net/">tools.simonwillison.net</a> collection of HTML+JavaScript tools was mostly built this way: I would have an idea for a small project, prompt Claude Artifacts or ChatGPT or (more recently) Claude Code via their respective iPhone apps, then either copy the result and paste it into GitHub’s web editor or wait for a PR to be created that I could then review and merge in Mobile Safari.
Those HTML tools are often ~100-200 lines of code, full of uninteresting boilerplate and duplicated CSS and JavaScript patterns—but 110 of them adds up to a lot!&quot;

code for tools: <a href="https://github.com/simonw/tools">https://github.com/simonw/tools</a>

so each tool has one html.

<a href="https://github.com/simonw/tools/blob/main/TOOLS_GUIDE.md">https://github.com/simonw/tools/blob/main/TOOLS_GUIDE.md</a> shows dev setup. hosted with github pages. it shows a sample tool e2e build and test process. seems can be used as context for other tool dev.

it also has many python tools, didn't see tests. not sure how it's get tested from phone.

one interesting thing is we can run python script like the following

uv run <a href="https://tools.simonwillison.net/python/list_llm_model_ids.py">https://tools.simonwillison.net/python/list_llm_model_ids.py</a>

This is convenient and powerful.

feels like the whole internet becomes a file system.
