---
title: Application Development Standards
description: >
  Defines the standards for developing bespoke applications. 
  Most of these standards also apply to off-the-shelf software and services.
stage: 3. Development Stage
created: 2020-11-17 13:23:29
lastUpdated: 2023-01-27 10:22:03
---

Please also see [#Issue 4](https://github.com/nhsengland/it-standards/issues/4) for the proposal for these standards.

!> It must be noted that NHS England is not in the business of developing software and bespoke services.<br><br>
The strategic approach to software and services is to use Commercial Off-The-Shelf (COTS) software and services and not to develop our own.<br><br>
Custom development should only take place where no other alternative exists.<br><br>
Projects are strongly encouraged to adopt standard operating models supported by COTS services and software so that they can continue to benefit from external improvements.<br><br>
Custom development means that software and services have to be continuously maintained and developed which adds ever increasing resource requirements to the organisation.

Things to cover (in no specific order):

* Passwords - Azure Key Vault, no sensitive information in code
* Development/project style (e.g. agile vs waterfall)
* Approvals required - before, during and after development - including alignment to standards, policies, architecture and service management
* Documentation standards - "documentation as code"
* Code management and publishing - Use of Git and GitHub
* Code and documentation licensing and copyright
* Available service/server platforms
  * Azure first (Cloud first, mobility first)
  * AWS - If Azure not suitable for some reason
  * Crown Hosting - if public cloud services not suitable
* Available application platforms
  * Azure cloud services (Saas options preferred over Paas over IaaS)
  * Office 365 for information management applications (SharePoint, Teams)
  * UDAL (Unified Data Access Layer) for health system wide, non-patient data (anonymised, aggregated) data and analytics
* Front-end (End User Compute) platforms - see also the separate EUC standards
  * Applications should be web-based and not require browser extensions or non-standard browser versions or settings.
  * Mobile apps may be native - but always require additional pre-approval.
  * Windows 10 - the preferred internal desktop environment, Microsoft Chromium Edge is the default browser
  * Apple MacOS - in limited use
  * iOS - for internal & external use
  * Android - for external use only
* Azure standard configuration (e.g. resource groups, tagging, etc)
* NHS Design Manual (follows UK Govt GDS Design Manual)
* Back-end development stack
   * .NET - core development for business applications
   * PYTHON 3 - for scripting where cross-platform compatibility is important
   * PowerShell - for scripting of Windows specific services
   * Other: ??
* Front-end development stack
   * REACT
   * ?? CSS Framework ??
* Mobile Development - ?? stack ??, Additional pre-approvals required (e.g. GDS)
* Terraform used for auto-provisioning
* Selenium WebDriver
* Security - secure development principles, security testing
* Environment and infrastructure management (DevOps automation to be used throughout)
* Testing
* Acceptance into service
* Accessibility
* Containerisation - where it makes sense, using Kubernetes.
* Identity and Access Management - end users, administrators - _requires a separate document_ - TL:DR Okta for "external" users, Azure SSO/AAD for assured internal users. Current use of Okta is for non-assured identities only (no identity assurance and no authorisation. If this is required, a separate instance of Okata may be required).
* Copyright & Licensing - see [Issue #2](https://github.com/nhsengland/it-standards/issues/2) and [PR #3](https://github.com/nhsengland/it-standards/pull/3) - Crown Copyright & dual MIT/OGL licensing.
* Documentation - needs to be accessible, comprehensive and living. PDF's should always be avoided.

Note that these standards should be used by all projects. If a project has a legitimate need to do something different, that will require review and approval from the Architecture Review Board.
