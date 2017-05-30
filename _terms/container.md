---
title: Container
action: light weight computer as a program
---

A container can be thought of as a computer program that acts like an an entire operating system. An app running from within a container can't tell that it's not running on the host operating system. This isolation, combined with easy of use, makes containers a convenient unit of measurement for processing for cloud computing needs. They are a light weight way of isolating apps and services to their own little corner of a machine.

To run an manage containers, we depend on a program called a *container runtime*. It might be easier to think of the runtime as a program that utilizes a collection of useful OS features and uses them in conjunction with each other.

> Over the last 5 years Linux has gradually gained a collection of features which make this kind of abstraction possible. Windows, with its upcoming version 10, is adding similar features as well. Those individual features have esoteric names like “control groups”, “namespaces”, “seccomp”, “capabilities”, “apparmor” and so on. But collectively, they are known as “OS containers” or sometimes “lightweight virtualization”.

[Introducing runC: a lightweight universal container runtime - Docker Blog](https://blog.docker.com/2015/06/runc/)

The Cloud Foundry component that manages containers is [Garden](/garden/).

