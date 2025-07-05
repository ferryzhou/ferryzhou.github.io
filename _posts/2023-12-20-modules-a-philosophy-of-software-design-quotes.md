---
title: "Modules - A philosophy of software design quotes"
date: 2023-12-20
---

One of the most important techniques for managing software complexity is to design systems so that developers only need to face a small fraction of the overall complexity at any given time. This approach is called modular design.

Modules can take many forms, such as classes, subsystems, or services.

Modules consists of two parts, interface and implementation.

Interface represents the complexity. The smaller and simpler the interface, the less complexity it introduces.

Prefer deep modules. Avoid shallow modules.

Simplify interface with defaults.

Bad example: java input stream classes. Have to create 3 classes and chain together.

Information hiding can often be improved by making a class slightly larger.
