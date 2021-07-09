---
title: Identity & Access Management
description: >
   This section of the standards covers all aspects if user identity and access management.
stage: 3. Development Stage
created: 2021-06-14 10:16:44
lastUpdated: 2021-06-14 17:32:22
reviewDate: 2022-05-01
---

IDAM is broken down into two main areas due to the very complex set of requirements that cover all of the many and varies requirements of NHSEI.

"Internal" IDAM covers all aspects of staff and contract identities along with access control for services and systems that are largely "internally" facing. Note however, that our systems are rarely _just_ internal or external.

"External" IDAM covers those services and systems that are primarily for use across the health and social care sector. Staff may have access to these systems but the majority of users will be non-staff. Access may be from across the NHS, local and central government, MOJ, MOD, Police, as well as voluntary sector and patient representatives.

## Internal

The strategic tool and ID's for internal use is NHS England's **Azure Active Directory** (AAD). 

Any services, systems, or projects wishing to use some different identity MUST gain approval from CISW Architecture, Infrastructure, and Cyber Security (via the _Technical Design Authority_) as well as from the _Architecture Review Board_.

A data centre based _Active Directory_ is also available for use but no new systems or services should be designed against it without prior approval.

## Eternal

The strategic approach for systems and services whose users are primarily external is **Okta**.

The instance of Okta previously referred to as "The Insights Platform", will be the primary focus. 

However, a secondary instance that is set up in a more traditional mode is also available. As of 2021-06, this is only currently used for the NHSEI Service Now platform which has a hybrid of federated identities.

Any designs wishing to use alternative identity or access control provision MUST gain pre-approval before starting the design process. Approval is via at least the _Technical Design Authority_ (TDA) and _Architecture Review Board_ (ARB).