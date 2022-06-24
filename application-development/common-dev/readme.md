---
title: Common Applications Development Standards
description: >
   Defines the standards that are common to all application development projects.
stage: 3. Development Stage
created: 2021-06-08 17:21:47
lastUpdated: 2022-06-24 10:36:01
---

Please note that ALL application development in NHS England and NHS Improvement is subject to the IT Requests & Approvals process.

No development may be started or considered without informing IT PMO so that it can be reviewed. You can then be supported through the
various phases of work and approvals that may be required. Finance will not accept any business cases that involve technology or IT that have not been approved by IT.
Some projects will require additional approvals from other bodies, refer to the latest IT request process for details. Additional approvals may include (but are not limited to), DPAG/GDS and ARB. This is in addition to any commercial and financial approvals.

Proposals will be reviewed on fit to policies, strategies and standards; resourcing; budgets; security and information governance.

> **An overriding strategic requirement for all IT in NHS England is that off-the-shelf is preferred over bespoke services and systems.**
As such, no bespoke development should take place without an assessment of existing and commercial off-the-shelf services prior to undertaking any design or development work.

## Core

!> If the stakeholders cannot clearly define a set of business needs, DO NOT START any work other than a _discovery phase_. A discovery phase may be nothing more than a stakeholder workshop but the result MUST be a documented set of _needs_ or _requirements_ and a clearly defined SCOPE.

All development:

* MUST NOT START unless clearly defined scope, requirements (both functional and non-functional), budgets, resources (including both business and technical stakeholders), and plans are available.
* MUST follow the common and other development standards in this repository.
* MUST follow the NHS England [Identity and Access Management](idam/readme) and [Security](security/readme.md) standards in this repository.
* MUST use [open standards](https://www.gov.uk/government/publications/open-standards-principles/open-standards-principles) wherever possible.
* MUST use the [license and copyright standards](application-development/common-dev/code-license-and-copyright.md).
* MUST follow the [NHS](https://service-manual.nhs.uk/) and [UK Government](https://www.gov.uk/service-manual) (Cabinet Office Government Digital Service) Design Manual's.
* MUST follow the security guidelines set out by the National Cyber Security Centre (NCSC).
* MUST meet the accessibility requirements contained in the [GDS Service Manual](https://www.gov.uk/service-manual/helping-people-to-use-your-service/making-your-service-accessible-an-introduction#meeting-government-accessibility-requirements). See also the [Accessibility page](application-development/common-dev/accessibility). Accessibility is also a legal requirement.
* SHOULD follow the security guidelines set out by NIST.

## Good Practice

An agile approach to delivery should mean that work initially progresses towards an identified [Minimum Viable Product (MVP)](https://www.agilealliance.org/glossary/mvp/#q=~(infinite~false~filters~(tags~(~'mvp))~searchTerm~'~sort~false~sortDirection~'asc~page~1)). This is a well understood engineering approach to maximise real benefit whilst minimising cost and effort. 

?> Note that an MVP **must** be aimed at getting the _maximum understanding_ about what the target business users/teams/functions **need** rather than minimising delivery.

Any application or system must be engineered for future change, with a development approach that builds-in security, maintainability, and flexibility.

* Develop **[loosely coupled components](https://ieeexplore.ieee.org/abstract/document/6299100)** and services that have [high cohesion](https://en.wikipedia.org/wiki/Cohesion_(computer_science))
* Understand and actively manage dependencies
* Isolate components likely to change or with dependencies that are likely to change
* [Encapsulate](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming)) complexity
* Use **open** data and standards throughout
* Design, build, and test for **security** at every stage and every level (e.g. from function, through component, to module and system level). Every level must independently and collectively deisgn and build for security
* Decide on and enforce **standard** tools, libraries and coding style
* Use DevOps pipelines, and Continual Integration (CI) for regression testing and **[code linting](https://www.perforce.com/blog/qac/what-lint-code-and-why-linting-important)**
* Design and code "in the open" where feasible. Encourage feedback and raising of issues.
* Document everything! Agile does not excuse design and development teams from properly documenting and maintaining the documentation. Do, however, use "**[documentation as code](https://technology.blog.gov.uk/2017/08/25/why-we-use-a-docs-as-code-approach-for-technical-documentation/)**" principles to keep documentation agile, maintained, and open.

## Other

See also the specific development standards:

* [Business Applications Development](application-development/business-dev/)
* [Web Applications Development](application-development/web-dev/)
* [Mobile Applications Development](application-development/mobile-dev/)
* [Platforms Applications Development](application-development/platform-dev/)
* [Desktop Apps](application-development/desktop-apps/)

Please read the [CONTRIBUTING](CONTRIBUTING.md) document for details of how to contribute to these standards.
