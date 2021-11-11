---
title: Accessibility
description: >
   All applications, systems and services in use at NHSEI and NHSX must be accessible to all. This standard provides pointers to what that means
   and what responsibilities developers, documentors, implementors and vendors have.
stage: 3. Development Stage
created: 2021-09-30 10:35:48
lastUpdated: 2021-11-11 11:17:18
author: Julian Knight
---

Accessibility **MUST** be considered in all application development. It must also be considered in the procurement of off-the-shelf services and applications. 

**This is both a legal and a moral requirement.**

All applications developed by and on behalf of NHS England, NHS Improvement and NHSX MUST use the [DCB1605](https://digital.nhs.uk/data-and-information/information-standards/information-standards-and-data-collections-including-extractions/publications-and-notifications/standards-and-collections/dcb1605-accessible-information) standard.
While this mostly focuses on patient facing services, it applies to all applications and services for NHSEI.
The standard also details the legal responsibilities and provides references explaining why accessibility is critical
for our systems.

The [2010 Equality Act](https://www.legislation.gov.uk/ukpga/2010/15/contents) is the main legislation that underpins these requirements.

In addition, all browser-based user-interfaces MUST meet at least level _AA_ of the [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/TR/WCAG21/), currently (2021) at version 2.1. and should strive for _AAA_ level if possible.

Also note that **documentation** as well as services and applications MUST also be accessible.

## Scope of needs

Remember that there are many forms of accessibility needs, some of which will not be obvious. These include colour blindness and Dyslexia. You should not make assumptions about accessibility, use standardised testing methods.

Generally, accessibility needs are split into 5 general areas:

* Auditory
* Cognitive, learning and neurological
* Physical
* Speech
* Visual

## Testing

Whether creating a bespoke application or implementing off-the-shelf applications or services, accessibility testing MUST be included during the development and deployment stages. Accessibility testing should also be part of User Acceptance Testing (UAT).

It is helpful for any test team to have at least one person who has additional specialist knowledge about accessibility testing. However, ALL developers and testers should be aware of accessibility requirements.

## Tools

There are many tools to help developers and authors meet accessibility standards. A few are listed here however every development team should have accessibility testing and tooling available as part of their standard toolset.

Implementors of off-the-shelf applications and services also need accessibility testing tools. Since it is expected that new services are built as web-based, implementors can use the standard web testing tools.

* "Linting" - when developing user interfaces, linting tools provide both as-you-type and batch checking of code quality. This can include basic accessibility. This is especially important for web development where there are many accessibility-specific attributes that should be used as standard (they mostly start with the word "aria").
* Testing in the browser - browsers such as Edge and Chrome include accessibility tests in their "Developer Tools" which are a free part of every browser. Check out the "Lighthouse" tool for example.
* Microsoft Office - if writing documents using MSFT Office, make use of the built-in accessibility tests to ensure that documents are readable by people with specific accessibilty needs.

## References

* [Understanding accessibility requirements for public sector bodies (gov.uk)](https://www.gov.uk/guidance/accessibility-requirements-for-public-sector-websites-and-apps)
* [Accessible Information Standard Specification](https://www.england.nhs.uk/publication/accessible-information-standard-specification/)