---
title: "Define errors out of existence – A philosophy of software design quotes"
date: 2023-12-29
---

Throwing exceptions is easy; handling them is hard.

Classes with lots of exceptions have complex interfaces, and they are shallower than classes with fewer interfaces.

The best way to eliminate exception handling complexity is to define your APIs so there are no exceptions to handle: define errors out of existence.

// it means no errors anymore by definition.

If you are having trouble figuring out what to do for the particular situation, there's a good chance the caller won't know what to do either.

The best way to reduce bugs is to make software simpler.
