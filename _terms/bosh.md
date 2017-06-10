---
title: BOSH
action: help me use clouds effectively
---

BOSH is a tool chain for distributing, deploying, and managing software on [VMs](/virtual-machine/). It is suitable for distributed, highly available software that has to support multiple [IaaSes](/infrastructure-as-a-service/) or [clouds](/cloud/). BOSH's job is to manage and monitor VMs while removing the gritty details away from the infrastructure owner. It is an important component of [Cloud Foundry](/cloud-foundry/).

Distributed systems need a lot more management than regular simple apps. Here’s a subset:

* Configuration management
* Release engineering
* Deployment lifecycle
* Infrastructure provisioning (IaaS), allocating, and releasing resources
* Rolling system updates
* Operating system update
* Auto recovery

BOSH takes care of these requirements. It’s implemented using several components:

* Director
* Agent (a process running on each VM)
* [Health Monitor](/health-monitor/)
* [Stemcells](/stemcell/)
* CLI
* CPI
* BOSH release (software and configuration in a package that BOSH can deploy)

The agent is responsible for reporting to the director. It configures the VM as specified by the user, and manages jobs that run on the VM, and other tasks.
