---
title: Dependency Management
description: >
   Most modern development depends on other software, services and platforms. This standard provides requirements and recommendations for dependency and version management.
stage: 3. Development Stage
created: 2022-06-24 13:11:23
lastUpdated: 2022-06-27 10:14:09
---

All tooling and software dependencies, whether used to help develop or used to support business applications, must use currently supported software and services.

## Versions

It is not acceptable for business applications to use outdated software or services. Ones that are not under current, active support.

Development projects must allow for ongoing maintenance and updates of dependent software.

In regards to software used to support development, it must follow the same [standards as for desktop software](euc/permitted-versions.md) even if server-based.

## Dependent Licenses

When using 3rd-party dependencies such as libraries, frameworks, etc. Note must be taken in regard to the licenses that those dependencies use.

Only permissive licenses can be used and only those license types that are compatible with the [UK Government and NHS license types](application-development/common-dev/code-license-and-copyright.md).

Please take note of the requirements of each license. For example, some may require that source code is openly published. Many will require copies of the license to be part of the deployed code as well as any published code.

The following should be taken as examples and are not definitive.

### Probably allowable license type examples

* [Open Government License v3](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/)
* [MIT](https://opensource.org/licenses/MIT)
* [Apache](https://www.apache.org/licenses/LICENSE-2.0)
* BSD (Berkeley Software Distribution) Family
* Microsoft Public License (MS-PL)
* Lesser GPL (LGPL)
* HL7
* ISC OSI (Open Source Initiative Licence)

### Unacceptable license type examples

Dependent libraries/frameworks with these licenses cannot be used since their licenses are too restrictive.

* Affero GPL (AGPL)
* GPL
* Mozilla Public License (MPL)
* Eclipse Public License (EPL)
* Common Development and Distribution License (CDDL)
