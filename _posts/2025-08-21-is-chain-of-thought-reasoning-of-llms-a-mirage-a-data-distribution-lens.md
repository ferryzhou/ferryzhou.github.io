---
title: "Is Chain-of-Thought Reasoning of LLMs a Mirage? A Data Distribution Lens"
date: 2025-08-21
---

<a href="https://share.google/6V8GlB3inq3Os9T5a">https://share.google/6V8GlB3inq3Os9T5a</a>

CoT reasoning is a brittle mirage that vanishes when it is pushed beyond training distributions.

See also <a href="https://venturebeat.com/ai/llms-generate-fluent-nonsense-when-reasoning-outside-their-training-zone/">https://venturebeat.com/ai/llms-generate-fluent-nonsense-when-reasoning-outside-their-training-zone/</a>

Based on their findings, the researchers conclude that CoT reasoning is a “sophisticated form of structured pattern matching, fundamentally bounded by the data distribution seen during training.” When tested even slightly outside this distribution, performance collapses. What looks like structured reasoning is more of a mirage, “emerging from memorized or interpolated patterns in the training data rather than logical inference.”

Patching with SFT or a few examples seems working.

However, this quick fix further supports the pattern-matching theory, suggesting the model isn’t learning to reason more abstractly but is instead just memorizing a new pattern to overcome a specific weakness.
