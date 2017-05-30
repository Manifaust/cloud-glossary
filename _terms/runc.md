---
title: runC
action: runs containers
---

Docker released a tool called runC which has the sole job of running container images. Docker calls it a plumbing tool, a lightweight runtime. runC is a CLI tool that knows how to use and connect OS features together, creating a *container runtime*. With that said, what runC does - kicking off containers - is usually not useful enough. There’s missing features around lifecycle management, networking, and storage that users need. So runC is really meant for platform creators like Pivotal or Docker to integrate with other tools as part of a larger component. For Docker that component is [containerd](https://containerd.io), for Pivotal it is [Garden](/garden/).

