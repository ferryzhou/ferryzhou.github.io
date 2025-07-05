---
title: "claude github agent, mcp, integration and productivity"
date: 2025-06-08
---

继续研究claude github agent

还是读<a href="https://github.com/anthropics/claude-code-base-action/blob/main/examples/issue-triage.yml">https://github.com/anthropics/claude-code-base-action/blob/main/examples/issue-triage.yml</a>

代码不是很长，但是关键的东西都在这儿

这是一个workflow的example

当新的issue open的时候，这个workflow就会被触发

最终会使用mcp__github__update_issue来apply一个合适的label

整个程序逻辑都在Create triage prompt里面

可以把它看作是一段代码

只不过是natural language

包含input info，就是repo和issue number

内容分成几个步骤，每个步骤都写得非常的详细和清楚

workflow最后一步是apply这个prompt，使用这个repo本身的action，anthropics/claude-code-base-action

一个action可以看作是一个command line tool

另外这个tool和prompt里都提到了mcp

所有的github issue相关的tool都通过mcp来提供

这个mcp server是github的官方server <a href="https://github.com/github/github-mcp-server">https://github.com/github/github-mcp-server</a>

claude这个agent是一个client，会运行中间的tool调用

这个地方有更详细的mcp client介绍
<a href="https://modelcontextprotocol.io/quickstart/client#how-it-works">https://modelcontextprotocol.io/quickstart/client#how-it-works</a>

mcp提供了一个通用的tool协议，估计会一统天下

类似于RPC

actually, MCP uses JSON-RPC 2.0 as its wire format.

有了mcp，llm跟tool的集成就变成非常的简单

一个简单的JSON config就够了，最多十来行

感觉各种应用都争先恐后的支持mcp

之前连api都没有

现在mcp就是api

mcp一下子打通了所有应用之间的连接

借着llm的东风

有了集成，各种llm的应用就能快速落地

接下来就是生产力的提升

这绝对是一个big tide
