---
title: BOSH
action: help me use infrastructure effectively
---

BOSH is a tool chain for distributing, deploying, and managing software on [VMs](/virtual-machine/). It is suitable for distributed, highly available software that has to support multiple [IaaSes](/infrastructure-as-a-service/) or [clouds](/cloud/). BOSH's job is to manage and monitor VMs while removing the gritty details away from the operator. It is an important component of [Cloud Foundry](/cloud-foundry/).

Distributed systems need a lot more management than regular simple apps, including:

* Configuration management
* Release engineering
* Deployment lifecycle
* Infrastructure provisioning (IaaS), allocating, and releasing resources
* Rolling system updates
* Operating system update
* Auto recovery

BOSH takes care of these requirements. It’s implemented using several components:

* [Director](/bosh-director/)
* [Agent](/bosh-agent/) (a process running on each VM)
* [Health Monitor](/health-monitor/)
* [Stemcells](/stemcell/)
* [CLI](/command-line-interface/) - the app you use to send commands to the Director
* [CPI](/cloud-provider-interface/)
* BOSH release (software and configuration in a package that BOSH can deploy)

The agent is responsible for reporting to the Director. It configures the VM as specified by the user, and manages jobs that run on the VM, and other tasks.
