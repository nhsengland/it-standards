---
title: Platform Development Standards
description: >
   Defines the standards when developing a new "platform", a service or (set of) applications and tools that allow people to create business applications.
stage: 3. Development Stage
created: 2021-06-08 17:21:47
lastUpdated: 2022-06-24 10:39:12
---

These standards apply when developing a new "platform" which is to say, a service or (set of) applications and tools that allow people to create business applications.

For example, the rewrite of the FutureNHS collaboration site using a new open source Content Management System (CMS) is considered a platform since it may be used to create any number of services.

# Core

Any platform development:

* **MUST follow the [common development standards](application-development/common-dev/readme).**
* MUST use web-based (browser) clients and not desktop clients.
* MUST NOT require browser extensions. Though extensions may be specified for enhanced use if necessary.
* MUST follow the [NHS England Infrastructure Standards](infrastructure/readme). As such, platform developments MUST use either vendor maintained infrastructure or the NHS England Azure platform.

> Note that NHS England also maintain a common data platform which is also Azure based but is a separate Azure tenancy. Requests for platform support will be assessed and assigned to the appropriate platform.
