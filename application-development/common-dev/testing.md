---
title: Testing
description: >
   Standards and requirements for testing of developed applications.
stage: 3. Development Stage
created: 2021-06-30 11:22:49
lastUpdated: 2021-06-30 17:40:45
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

### 5) Accessibility Tests

All systems and services produced by and for NHS England and NHS Improvement MUST, by law and common morals, be accessible to users who require reasonable adjustments in order to use the service.

As such, all systems and services MUST be tested for accessibility throughout the development and testing lifecycle.

All web browser based systems and services MUST be designed and tested to meet the Web Content Accessibility Guidelines (WCAG) also known as ISO/IEC 40500.

While the majority of accessibility testing can use test tooling and automation, it is important to consult with people who have real-world accessibility issues.

### 6) Security Tests

All development is expected to incorporate security thinking at every stage. As such, the other test phases should incorporate specific security-focused tests appropriate to the system and its level of risk, classification, and sensitivity.

Additionally, systems will need to at least go through internal _automated security testing_ by the Cyber Security Team.

Systems and services classified at OFFICIAL-SENSITIVE or above and all systems and services accessible from the Internet MUST also go through at least _Penetration Testing_. They may be required to undertake full (and regular) _IT Health Checks_.

All development projects MUST contact the Cyber Security Team early in the project lifecycle to agree the level and type of security testing required. The Security Team _should_ already be aware of proposed projects via the IT Request and Business Case Approvals triage process.