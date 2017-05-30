---
title: Garden
action: create, destroy, and control containers
---

Garden is Go client, server, and implementable API for creating and managing containers. It relies on pluggable backends that implement its interface. It is the containerization layer used by Diego.

> These interfaces contain methods to perform the following actions:
> * Create and delete containers
> * Apply resource limits to containers
> * Open and attach network ports to containers
> * Copy files into and out of containers
> * Run processes within containers
> * Stream STDOUT and STDERR data out of containers
> * Annotate containers with arbitrary metadata
> * Snapshot containers for redeploys without downtime

[Doc - ERT Component: Garden](https://docs.pivotal.io/pivotalcf/1-9/concepts/architecture/garden.html)

There are two pluggable backends:
* Guardian - Linux backend using [runC](/runc/)
* Greenhouse - Windows backend

> […] keeping containers running during a Garden-Linux upgrade, root filesystem management, integrating Cloud Foundry networking, and a simple API server. However, with Guardian the main container engine is now a very small and simple wrapper around runC.

[An Update on Guardian, an OCI-based runtime for Cloud Foundry](https://containereyes.wordpress.com/2016/02/17/an-update-on-guardian-an-oci-based-runtime-for-cloud-foundry/)
