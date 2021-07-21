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

The strategic tool providing identities for internal use is NHS England's **Azure Active Directory** (AAD). Everyone working for NHSEI, whether employee's, embedded, seconded in or contracted should have an entry in the NHS England AAD.

This entry should also give them an entry in the Staff Directory.

Identities in this AAD mostly end in @england.nhs.uk. However, some other domains are also in use.

Any services, systems, or projects wishing to use some different identity MUST gain approval from CISW Architecture, Infrastructure, and Cyber Security (via the _Technical Design Authority_) as well as from the _Architecture Review Board_.

A data centre based _Active Directory_ is also available for use but no new systems or services should be designed against it without prior approval.

### Guests

Some of the Office 365 and Azure based services allow _guest_ access. Guests are invited using a standard feature of AAD and are recorded in the directory in a format that clearly identifies them as guests.

Guests use their own email identity associated to a [Microsoft Account](https://en.wikipedia.org/wiki/Microsoft_account) or their own organisation's Office 365 account identity. If a guest is invited via an email account that isn't associated with a Microsoft or Office 365 account, they will be offered to link their account to a Microsoft Account.

?> Note that NHSmail email addresses are already Office 365 accounts and that many NHS organisations are using NHSmail.

Guests do not appear in the staff directory.

Once invited, guests must accept the invitation and log in within 30d otherwise the invitation will lapse. They must also actively use the service otherwise their account will be removed and they will need to be re-invited. Currently, guests must login at least once every 6 months. This may be reduced down to three months in the future.

Guests should not use consumer accounts as these may get blocked due to the widespread misuse of such account types. Consumer account types include but are not limited to @gmail.com, @yahoo.com, @outlook.com as well as their country specific equivalents (e.g. .co.uk).

## External

The strategic approach for systems and services whose users are primarily external is **Okta**.

The instance of Okta previously referred to as "The Insights Platform", will be the primary focus. 

However, a secondary instance that is set up in a more traditional mode is also available. As of 2021-06, this is only currently used for the NHSEI Service Now platform which has a hybrid of federated identities.

Any designs wishing to use alternative identity or access control provision MUST gain pre-approval before starting the design process. Approval is via at least the _Technical Design Authority_ (TDA) and _Architecture Review Board_ (ARB).