---
title: BOSH Director
action: orchestrates all the VMs
---

The Director is a component of [BOSH](/bosh/) that a developer or operator sends commands to. It is in charge or taking those commands and creating tasks from them for other components to work on. The Director also talks to the [IaaS](infrastructure-as-a-service) to spin up and spin down [VMs](/virtual-machine/). It also keeps track of the state of all BOSH controlled VMs and the reconciles their expected states with their actual states.

Because an organization could be using any number of IaaSes, BOSH contains a layer between the director and the IaaS called the CPI. With this generic interface, the director doesn't need to know the exact details of which IaaS it's talking to.
