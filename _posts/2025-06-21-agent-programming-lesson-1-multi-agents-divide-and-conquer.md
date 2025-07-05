---
title: "Agent programming lesson 1 - multi agents, divide and conquer"
date: 2025-06-21
---

Last week I created an agent to do bug cleanup

Things become complicated when we get to the specifics

First, there are different types of bugs

So do we want to handle all of them in a single agent with a single prompt, or create multiple agents for different types?

The second option is better, and it's scalable, i.e. can handle many different types without increase complexity. It also follows the principle of divide and conquer.

Another question follows: how to triage? How to orchestrator?

Now this becomes a multiple agents system.

The official google adk doc listed this as the first patten, orchestrator pattern, and show an example.

Basically, the root agent is a triage agent. And it register different sub agents. Each sub agent handles specific tasks. The root agent first analyze the problem, and decide which agent to take the task. And hand over the task to the sub agent.
