---
title: Application Security
description: >
   Common security standards and requirements for NHSEI and NHSX applications.
stage: 3. Development Stage
created: 2021-06-30 11:22:49
lastUpdated: 2021-11-24 17:30:19
author: Julian Knight
---

All development is expected to incorporate security thinking at every stage. As such, all development and test phases should incorporate specific security-focused thinking appropriate to the system and its level of risk, classification, and sensitivity.

Additionally, systems will need to at least go through internal _automated security testing_ by the Cyber Security Team.

Systems and services classified at OFFICIAL-SENSITIVE or above and all systems and services accessible from the Internet MUST also go through at least _Penetration Testing_. They may be required to undertake full (and regular) _IT Health Checks_.

All development projects MUST contact the Cyber Security Team early in the project lifecycle to agree the level and type of security testing required. The Security Team _should_ already be aware of proposed projects via the IT Request and Business Case Approvals triage process.

All systems and services developed by and for NHS England and NHS Improvement will require a written and approved _System Level Security Policy_ (SLSP).

Any application that handles information classified at OFFICIAL-SENSITIVE or above (including commercially sensitive or personally identifiable information) is required to register with the NHSEI Information Asset Management System (IAMS). Please contact your Information Governance representative for further information.

Please also read the other development standards which have more specific information regarding security standards.

## Additional security references

* [Security](security/readme.md)
* [Security/TLS](security/tls.md)
* [Application Development/Authentication](application-development/common-dev/authentication)
* [National Cyber Security Centre (NCSC) Advice & Guidance](https://www.ncsc.gov.uk/section/advice-guidance/all-topics)
