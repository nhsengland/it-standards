---
title: Standards for Service Interoperability
description: >
   Services and systems rarely operate in isolation. This standard gives guidance on interoperability.
stage: 3. Development Stage
created: 2022-05-31 13:29:00
lastUpdated: 2022-05-31 13:29:00
author: Julian Knight
---

!> Not yet linked

> the issue with a service bus is that you are pushing messages about via a central hub and to do that, you need "envelopes" and confirmation messages as well. So that is potentially quite an overhead, all of which has to pass through a central hub which can become a performance and resilience bottleneck if not careful and can also become costly over time.
>
> Using HTTP in a REST API follows an architecture where global scalability is already a well understood issue and you can minimise overheads while using well-known standards (HTTP, TLS). HTTP is easily horizontally scaled (e.g. throw more cheap servers at it), supports well understood caching techniques which can lower overheads further in some circumstances, has really battle-hardened security interfaces.
>
> In simple terms, kind of like the difference between email and instant messaging.