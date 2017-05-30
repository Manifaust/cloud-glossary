---
title: Container
action: light weight computer as a program
---

A container can be thought of as a computer program that acts like an an entire operating system. Inside, an app doesn't know that it's running inside a container OS and not the host OS. The host can spin up multple containers at the same time and hide them from each other. Furthermore, it's able to constrain the amount of resources (e.g. processing, memory, networking) that each container can use. The combination of isolation, control, combined with ease of use, makes containers a convenient unit of processing for cloud computing needs.

To run and manage containers, we depend on a program called a *container runtime*. It might be easier to think of the runtime as a program that know about a collection of useful OS features and uses them in conjunction with each other.

> Over the last 5 years Linux has gradually gained a collection of features which make this kind of abstraction possible. Windows, with its upcoming version 10, is adding similar features as well. Those individual features have esoteric names like “control groups”, “namespaces”, “seccomp”, “capabilities”, “apparmor” and so on. But collectively, they are known as “OS containers” or sometimes “lightweight virtualization”.

[Introducing runC: a lightweight universal container runtime - Docker Blog](https://blog.docker.com/2015/06/runc/)

The Cloud Foundry component that manages containers is [Garden](/garden/).

