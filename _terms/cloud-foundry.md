---
title: Cloud Foundry
action: run my app on the cloud, I don't care how
---

Also known as CF. An open source platform for deploying apps and services where developers can focus on creating a product and not about a lot of other issues that come with managing software at a huge scale.

CF manages a lot of problem related to deploying software on the [cloud](/cloud):

* automatically recovering from crashes at the process, container, and VM levels
* running your app in a container
* supporting different [IaaSes](/infrastructure-as-a-service/)
* scaling scaling an app when it gets popular
* updating service with security patches
* updating passwords accross many services and apps
* exposing services to other users in the platform
* lots of other stuff

See also:
* [BOSH](/bosh/) - CF component used to provision and manage infrastructure
* [Garden](/garden/) - CF component used to manage containers
