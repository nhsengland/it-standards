---
title: Testing
description: >
   Standards and requirements for testing of developed applications.
stage: 3. Development Stage
created: 2021-06-30 11:22:49
lastUpdated: 2021-11-24 17:39:31
author: Julian Knight
---

## Required testing stages

In general, the following stages and types of testing will be required for applications and services developed by or for NHS England and NHS Improvement.

### 1) Unit Tests

Undertaken by developers during the development process. All development is expected to be Test Driven Development (TDD) in line with industry standards.

### 2) System Tests

This phase ensures that all of the units of the system/service work together as per the documented design.

### 3) Integration Tests

This test phase tests integration between the system/service under development and any related systems and services it integrates with.

### 4) User Acceptance Tests

This is the final part of any development and MUST involve stakeholders from the business. At this stage, IT and development users should not be doing the testing.

This phase must test the business logic and the overal business usability of the system or service. Reference should be made to the original business requirements as well as the defined business benefits.

UAT testing MUST include performance testing such that the system is proven to meet the non-functional requirements (NFR's) defined for it. Performance testing must include tests at load (e.g. many users, many transations).

### 5) Accessibility Tests

All systems and services produced by and for NHS England and NHS Improvement MUST, by law and common morals, be accessible to users who require reasonable adjustments in order to use the service.

As such, all systems and services MUST be tested for accessibility throughout the development and testing lifecycle in order to meet [UK Government accessibility requirements](https://www.gov.uk/service-manual/helping-people-to-use-your-service/making-your-service-accessible-an-introduction#meeting-government-accessibility-requirements).

All web browser based systems and services MUST be designed and tested to meet the Web Content Accessibility Guidelines (WCAG) also known as ISO/IEC 40500.

While the majority of accessibility testing can use test tooling and automation, it is important to consult with people who have real-world accessibility issues.

### 6) Security Tests

All development is expected to incorporate security thinking at every stage. As such, the other test phases should incorporate specific security-focused tests appropriate to the system and its level of risk, classification, and sensitivity.

Additionally, systems will need to at least go through internal _automated security testing_ by the Cyber Security Team.

Systems and services classified at OFFICIAL-SENSITIVE or above and all systems and services accessible from the Internet MUST also go through at least _Penetration Testing_. They may be required to undertake full (and regular) _IT Health Checks_.

All development projects MUST contact the Cyber Security Team early in the project lifecycle to agree the level and type of security testing required. The Security Team _should_ already be aware of proposed projects via the IT Request and Business Case Approvals triage process.

## Testing processes

* Testing MUST be incorporated into the Devops pipeline.
* It MUST include checking of _documentation_ as well as the code.
* It MUST include a final sign-off by test managers and (where appropriate) key stakeholders.
* It SHOULD have written test plans and checklists.
* It SHOULD include automated standard and regression tests.
* It SHOULD include static code analysis tools.
* It SHOULD include manual reading of code by someone other than the author.
