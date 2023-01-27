---
title: Web Development Standards
description: >
   NHS England requires that most if not all business applications and services with user-facing interfaces
   use the browser as the client. Therefore the majority of development should include web development.

   This page defines the basic requirements for web applications developed by and for NHS England.
stage: 3. Development Stage
created: 2021-09-30 10:35:48
lastUpdated: 2023-01-27 10:22:21
author: Julian Knight
---

Note that NO _publicly_ accessible web application, site, or service may be developed or deployed without the prior approval of GDS. That approval happens in parallel to other governance.

## Core

All web application development:

* **MUST follow the [common development standards](application-development/common-dev/readme).**
* MUST use the common web development stack defined by NHS England below.
* MUST meet W3C Web Accessibility Initiative ([WAI](https://www.w3.org/WAI/)) [WCAG](https://www.w3.org/WAI/standards-guidelines/wcag/) v2.1 standards for accessibility. All developments MUST be accessibility tested and MUST meet at least level AA compliance. Further information is contained in the [GDS Service Manual](https://www.gov.uk/service-manual/helping-people-to-use-your-service/making-your-service-accessible-an-introduction#meeting-government-accessibility-requirements). See also the [Accessibility page](application-development/common-dev/accessibility).
* MUST use open web-development standards.

All web applications:

* MUST be Penetration Tested using either our internal tool or an external vendor to current security standards. The Cyber Security team will advise.
* MUST only allow HTTPS access. HTTP access should be automatically redirected to HTTPS. This applies to ALL services without exception. Only [TLS v1.2 or above](security/tls.md) is permitted.
* MUST test the quality of their TLS configuration. Using something like the [Qualys SSL Labs website](https://www.ssllabs.com/ssltest/) (Should have a rating of A).

## Development processes

* MUST use DevOps to automate the design, development, build, test and deployment pipeline.
* MUST use "[linting](https://developerexperience.io/practices/linting)" and/or other static code analysis tools to automatically verify code quality and report obvious errors and poor quality code. These should be integrated into code editors and into the devops pipeline.
* All developers MUST have a good working knowledge of [defensive programming](https://scottdorman.blog/2008/07/04/what-is-defensive-programming/) and cyber security. Best practice security principles MUST be applied when writing any code.
* SHOULD use standardised coding style guides. Such as the [JavaScript Standard Style](https://standardjs.com/). This greatly helps anyone reading code for review or testing.
* SHOULD use Continuous Integration (CI) automated pipelines wherever possible.

## Coding Specifics

* Code SHOULD be readable. 
  * Use comprehensible, meaningful variable & function names
  * Use comments to show in english what something does if the code isn't clear.
  * Remember that code will be read many more times than it is written and that even the author won't remember why they did something in 6 months time.
  * Use whitespace to allow a reader's brain to take in the structure of code.
  * Split complex logic into smaller functions.
  * Split large code files into smaller modules.
  * Create and share common modules containing reusable functions and classes.
* All user or network inputs to back-end (server side) functions MUST be validated first. No unvalidated inputs are permitted.
* Inputs SHOULD be validated for length and allows characters as a minimum.
* Validation functions SHOULD be shared to ensure common approaches and to allow for simple improvements.
* Java MUST NOT be used for client programming. It MAY be used for back-end programming, however take careful note of licensing and ongoing maintenance issues.

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

## NCSC's 8 Principles of Secure Development & Deployment

1. Secure development is everyone's concern
2. Keep your security knowledge sharp
3. Produce clean & maintainable code
4. Secure your development environment
5. Protect your code repository
6. Secure the build and deployment pipeline
7. Continually test your security
8. Plan for security flaws

## Other references

* [NCSC: Secure development and deployment guidance](https://www.ncsc.gov.uk/collection/developers-collection)
* [NCSC: Enable your developers](https://www.ncsc.gov.uk/collection/technology-assurance/principles-product-development/2-enable-your-developers)
