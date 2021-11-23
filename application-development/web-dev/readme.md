---
title: Web Development Standards
description: >
   NHSEI requires that most if not all business applications and services with user-facing interfaces
   use the browser as the client. Therefore the majority of development should include web development.

   This page defines the basic requirements for web applications developed by and for NHSEI and NHSX.
stage: 3. Development Stage
created: 2021-09-30 10:35:48
lastUpdated: 2021-11-23 17:48:26
author: Julian Knight
---

Note that NO _publicly_ accessible web application, site, or service may be developed or deployed without the prior approval of GDS. That approval happens in parallel to other governance.

## Core

All web application development:

* MUST follow the [common standards](../common-dev).
* MUST use the common web development stack defined by NHSEI below.
* MUST follow the NHS and UK Government (Cabinet Office Government Digital Service) Design Manual's.
* MUST follow the security guidelines set out by the National Cyber Security Centre (NCSC).
* MUST meet WAI standards for accessibility.
* MUST use open web-development standards.
* MUST follow the security guidelines set out by NCSC & NIST.

All web applications:

* MUST be Penetration Tested using either our internal tool or an external vendor to current security standards. The Cyber Security team will advise.
* MUST only allow HTTPS access. HTTP access should be automatically redirected to HTTPS. This applies to ALL services without exception. Only [TLS v1.2 or above](../../security/tls.md) is permitted.

## Development processes

* MUST use DevOps to automate the design, development, build, test and deployment pipeline.
* MUST use "[linting](https://developerexperience.io/practices/linting)" and/or other static code analysis tools to automatically verify code quality and report obvious errors and poor quality code. These should be integrated into code editors and into the devops pipeline.
* SHOULD use standardised coding style guides. Such as the [JavaScript Standard Style](https://standardjs.com/). This greatly helps anyone reading code for review or testing.
* All developers MUST have a good working knowledge of [defensive programming](https://scottdorman.blog/2008/07/04/what-is-defensive-programming/) and cyber security.

## Coding Specifics

* All user or network inputs to back-end (server side) functions MUST be validated first. No unvalidated inputs are permitted.
* Inputs SHOULD be validated for length and allows characters as a minimum.
* Validation functions SHOULD be shared to ensure common approaches and to allow for simple improvements.

## Development stack

* **Browser Client** - for front-end client (user) interactions (using HTML, CSS and JavaScript).
* **REACT** - front-end library supporting client UI development.
* **JavaScript v6 (ECMA2015)** - front-end code MUST target this version of JS or be transpiled to it.
* **Azure DevOps Pipeline** - for Continuous Integration, project management, etc.
* **GitHub NHS England** - NHS England's organisation on GitHub. For code management.
* **.net or node.js** - for server (back-end) services.
* **[ESLINT](https://eslint.org/)** - for JavaScript linting. Using the [JavaScript Standard Style](https://standardjs.com/rules.html)
* **Visual Studio Code** - For web coding. Full Visual Studio can also be used for developers who are used to it but VScode has many advantages for web (and other) developers. While VScode was originally developed by Microsoft, it is now semi-independent open source freeware with a very large and active developer base.

  Suitable VScode extensions such as [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) or [StandardJS](https://marketplace.visualstudio.com/items?itemName=standard.vscode-standard) can and should be used with VScode.