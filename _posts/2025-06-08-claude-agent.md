---
title: "claude agent"
date: 2025-06-08
---

claude code就是一个agent

prompt -&gt; actions.

在这个command line tool之上又create了github action agent

github用户可以在issue里面@claude some_prompt就可以trigger claude actions

有source code

首先是<a href="https://github.com/anthropics/claude-code-base-action/tree/main">https://github.com/anthropics/claude-code-base-action/tree/main</a>

用claude这个binary加上custom prompt再加上github mcp server提供的各种api

比如mcp__github__update_issue

custom prompt example有一个<a href="https://github.com/anthropics/claude-code-base-action/blob/main/examples/issue-triage.yml">https://github.com/anthropics/claude-code-base-action/blob/main/examples/issue-triage.yml</a>

<a href="https://github.com/anthropics/claude-code-action/tree/main">https://github.com/anthropics/claude-code-action/tree/main</a>在claude-code-base-action基础之上又增加了很多功能

方法好象是先创建一个公共的prompt，里面有很多的context，

<a href="https://github.com/anthropics/claude-code-action/blob/main/src/create-prompt/index.ts">https://github.com/anthropics/claude-code-action/blob/main/src/create-prompt/index.ts</a>
