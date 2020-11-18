---
title: Application Development Standards
description: >
   Defines the standards for developing bespoke applications.
stage: 1. Proposal Stage
created: 2020-11-17 13:23:29
lastUpdated: 2020-11-18 11:44:12
---

# Application Development

**Documentation Stage**: 1. Proposal Stage

> Proposal stage documents are not yet accepted. They are reviewed by appropriate SME's

This category defines the standards for bespoke deveopment in NHS England and NHS Improvement.

Things to cover (in no specific order):

* Passwords - Azure Key Vault, no sensitive information in code
* Development/project style (e.g. agile vs waterfall)
* Documentation standards - "documentation as code"
* Code management and publishing - Use of Git and GitHub
* Code and documentation licensing and copyright
* Azure first (Cloud first, mobility first)
* Azure standard configuration (e.g. resource groups, tagging, etc
* NHS Design Manual (follows UK Govt GDS Design Manual)
* Back-end development stack
   * .NET - core development for business applications
   * PYTHON 3 - for scripting where cross-platform compatibility is important
   * PowerShell - for scripting of Windows specific services
   * Other: ??
* Front-end development stack
   * REACT
   * ?? CSS Framework ??
* Terraform used for auto-provisioning
* Selenium WebDriver
* Security - secure development principles, security testing
* Environment and infrastructure management (DevOps automation to be used throughout)
* Testing
* Acceptance into service
* Accessibility

Note that these standards should be used by all projects. If a project has a legitimate need to do something different, that will require review and approval from the Architecture Review Board.
