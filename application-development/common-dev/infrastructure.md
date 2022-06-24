---
title: Common Infrastructure and Platform Standards
description: >
   Defines the infrastructure and platform standards that are common to all application development projects.
stage: 3. Development Stage
created: 2021-11-24 17:48:16
lastUpdated: 2022-06-24 10:32:59
---


## Core

All development of applications and services by and for NHS England are subject to UK Government and general NHS strategies. 
As such, they MUST use _Cloud First_ principles.

Developments requiring local infrastructure will require additional scrutiny and governance and will mostly be rejected without a clear and convincing business case.

NHS England's cloud platform of choice is Microsoft Azure. Use of other platforms is discouraged only because of the additional complexity and overheads of trying to support 
multiple global cloud platforms. Use of other platforms is subject to approval by the Architecture Review Board and even if approved is likely to result in ongoing support and
maintenance costs that will need to be born by the key stakeholders.

Any proposed infrastructure that needs support from CISW is also subject to review and approval BEFORE PROCUREMENT BEGINS from the CISW Infrastructure Team and the CISW Technical Design Authority board (TDA).

Infrastructure definitions MUST be well documented and, where feasible, MUST use template definitions. Where Azure infrastructure is used, it is expected that the infrastructure will be defined using Azure Templates. In other cases, Kubernetees may be used. Note that Docker is NOT currently supported by NHS England and should not be used.

See the [Infrastructure](infrastructure.md) section of this site for more information.

?> Note that these restrictions are practical ones and do not represent a favouring of one supplier over another. They will be reviewed from time-to-time. Global cloud platforms are large and complex and require specialist knowledge to support them. Having multiple such clouds in use waters down the ability to train staff and maintain in-depth knowledge. Use of other cloud platforms will require additional resources to support them.