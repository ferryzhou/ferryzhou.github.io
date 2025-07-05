---
title: "General purpose modules are deeper – A philosophy of software design quotes"
date: 2023-12-24
---

<blockquote>The process of teaching my software design course, in which I'm constantly trying to identify the causes of complexity in student code, has changed my thinking about software design in several ways. The most important of these has to do with generality versus specialization. I have found over and over that specialization leads to complexity: I now think that over-specialization may be the single greatest cause of complexity in software. Conversely, code that is more general-purpose is simpler, cleaner, and easier to understand.</blockquote>
This insight is very powerful.

And surprisingly true.

Because it's too easy to start with specialized code or design. And people think they can always refactor to make it more general, which is usually not happening. What happens is specialized code leads to more specialized code, especially for code contributed by different teams. Changing specialized code to general code is very costly, and hard to get quick approval.

General purpose modules are not only simpler, easier to change, they are also more powerful, exponentially powerful. They also make caller code simple.

Several years ago, I developed some general purpose code and witnessed the power. It's so flexible that anything new can be written in config files. No new c++ or proto code needs to be developed to support different use cases. The problem is to apply calibration by some slice keys. There are different calibration models, different models can use different slice keys. Traditionally, the slice keys are hard coded. For every new calibration model, a new set of photos, classes, methods are developed. I made an interface that accepts slice keys as a list of strings. In this way, any model can use the same interface. The implementation code uses some low level features like reflection in Java. The implementation itself is also much simpler.

Ruby on rails also started from restless generalization and simplification.
