---
title: BOSH Agent
action: middle-manager inside a VM
---

The Agent is a process that runs inside every [BOSH](/bosh/) controlled [VM](/virtual-machine/). It takes orders from the BOSH Director to do different tasks. And it also help the [Health Monitor](/health-monitor/) to know that the VM is still alive.

It receives orders from the Director about how to install and configure software. Then it starts and monitors the software with the help of [Monit](/monit/). For these tasks, the Agent communicates with the Director through a message bus called NATS.
