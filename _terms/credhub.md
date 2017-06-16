---
title: Credhub
action: credentials manager
---

[Cloud Foundry's](/cloud-foundry/) credential management server. It’s not meant to manage user credentials, instead it is meant to store the passwords that CF services and components are configured with. Besides the sheer number of keys and passwords, there’s also needs for a central place where these credentials can be rotated and to which access can be controlled.

Here’re some features:

* Open source
* Encryption uses plugin system, anyone can build their own
* Supports hardware security modules (HSM)
* Graceful recovery from restarts and failures
* Public record of security vulnerability and patches

Unlike HashiCorp’s Vault, Credhub is not meant to be used a generic credential manager. It really is designed to be used with Cloud Foundry ecosystem and environment.
