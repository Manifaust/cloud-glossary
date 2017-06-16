---
title: Cloud Provider Interface
action: I don't need to know the nitty gritty of talking to an IaaS
---

Also known as CPI. The Cloud Provider Interface is an API that developments can implement so that the [BOSH Director](/bosh-director/) can talk to their [IaaS](/infrastructure-as-a-service/) of choice. The API has generic commands and the implementation is in charge of translating those commands to IaaS specific commands. This generic interface is used so the that Director doesn't need to know the exact details of how to use each IaaS. There are currently supported CPI's for AWS, GCP, and Azure.
