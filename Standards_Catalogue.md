---
title: Catalogue of IT Standards for NHS England
description: >
   A list of the available standards.
created: 2020-06-29
lastUpdated: 2024-03-19 10:18:03
author: Julian Knight
---

- **[Application Development Standards](./application-development/readme)**
  
  - [Common Application Development Standards](./application-development/common-dev/readme)

    These apply to all development.

    - [Accessibility](application-development/common-dev/accessibility)
    - [Authentication](application-development/common-dev/authentication)
    - [Email Integration for Business Applications](application-development/common-dev/email-integration)
    - [Infrastructure](application-development/common-dev/infrastructure)
    - [License and Copyright](application-development/common-dev/code-license-and-copyright)
    - [Security](application-development/common-dev/security)
    - [Testing](application-development/common-dev/testing)

  - [Business Applications Development](./application-development/business-dev/readme)

    Business applications are bespoke applications developed on corporate/business platforms and will typically use C#, C++, Visual Basic.net, SQL Server, etc. They may be hosted on-premise or in the cloud.

  - [Platform Applications Development](./application-development/platform-dev/readme)

    Platform development refers to developing systems and solutions on existing platforms such as Office 365 or Dynamics 365. It does not refer to cloud platforms such as Azure or AWS since these are infrastructure platforms rather than application platforms.

  - [Web Applications Development](./application-development/web-dev/readme)

    Internet applications are mostly Internet facing, they may be public or private. They are developed using Internet standards such as HTML, CSS, JavaScript, etc.

  - [Mobile Applications Development](./application-development/mobile-dev/readme)

    Development of applications for mobile devices (those running mobile operating systems such as Apple iOS and Google Android).

  - [Desktop Applications Development](./application-development/mobile-dev/readme)

    Development of applications for desktop devices (those running desktop operating systems such as Apple MacOS and Microsoft Windows).

  - [Dependency & Software Version Management](./application-development/dependencies)

    Standards and guidance on managing software and service dependencies and version control.

 
- **[End User Compute (EUC)](./euc/readme)** - desktop and mobile

  Standards covering all matters relating to end-user computing. Including devices, operating systems and applications. Both mobile and desktop.

  * [Standards for Desktop EUC devices](euc/desktop-devices)
  * [Desktop Software](euc/desktop-software)
  * [End User Email Services](euc/email)
  * [Software Version Standards](euc/permitted-versions)
  * [User Types](euc/user-types)
  * [Windows 10 Standard Applications](euc/windows-10-standard-apps)


- **[Identity and Access Management](./idam/readme.md)**

  Standards for identifying, authenticating and authorising people and systems. Note that this does not include the _processes_ being used, only the standards.

  - [As Is](idam/as-is/readme) - How things are at the moment (prior to the implentation of the 2021 IDAM strategy)
  - [People Database](idam/peopledb) - Using the database of staff information


- **[Infrastructure](./infrastructure/readme.md)** - cloud and on-premise/data centre

  Standards covering all elements of infrastructure. This is defined as "back-end" hardware and software that supports business applications, networking, security, etc.

  * [Cloud Infrastructure](infrastructure/cloud)
  * [Physical Infrastructure (On-Premise, Data-Centre)](infrastructure/physical)
  * [Networks](infrastructure/networks) - Local and Wide-Area Networks (LAN, WAN)
  * [Availability](infrastructure/availability)

- **[Security](./security/readme.md)** - Security and Privacy

  Standards related to security and privacy.

  - [Cloud Apps & Services Guidance](security/acceptable-cloud-tools)
  - [Guidance for using Open Internet Tools](security/guidance-for-using-open-internet-tools)
  - [TLS Standards](security/tls) - How to properly use Transport Level Security

- **[Services](Services/readme.md)** - IT Service procurement and implementation

  - [Procurement Requirements](Services/service-procurement.md)

- **Other Applicable UK Government and NHS Standards**

  All of the standards for NHS England are subject to both NHS and UK Government policies, strategies and standards, the key ones of which are listed here.

  * **[NHS Digital Service Manual](https://service-manual.nhs.uk/)** - "Use the service manual to build consistent, usable services that put people first.​ Learn from the research and experience of other NHS teams."
  * **[Gov.uk Service Manual](https://www.gov.uk/service-manual)** - "Helping teams to create and run great public services that meet the **[Service Standard](https://www.gov.uk/service-manual/service-standard)"**. See also the **[Government Design Principles](https://www.gov.uk/guidance/government-design-principles)** and the **[Gov.uk Design System](https://design-system.service.gov.uk/)**.
  * **[Tech Code of Practice](https://www.gov.uk/government/publications/technology-code-of-practice/technology-code-of-practice)** - A set of criteria to help government design, build and buy technology. It is a cross-government agreed standard used for the Cabinet Office spend control process and the Local Digital Declaration.
  * The UK Government **[Tech Vision](https://www.gov.uk/government/publications/the-future-of-healthcare-our-vision-for-digital-data-and-technology-in-health-and-care/the-future-of-healthcare-our-vision-for-digital-data-and-technology-in-health-and-care)** - ‘Standards that meet user needs: we must be clear how these standards address the user needs of people who use health and care services, carers and families, as well as care professionals and commissioners.’
  * The **[NHS Long Term Plan](https://www.longtermplan.nhs.uk/areas-of-work/digital-transformation/)** - ‘Set standards that keep information secure and make sure NHS IT systems talk to each other to provide health and care staff with complete access to joined up patient records.’​
  *  **[DSP Toolkit](https://www.dsptoolkit.nhs.uk/)** - "an online self-assessment tool that allows organisations to measure their performance against the National Data Guardian’s 10 data security standards. All organisations that have access to NHS patient data and systems must use this toolkit to provide assurance that they are practising good data security and that personal information is handled correctly."
  *  **[Cyber Essentials Plus](https://www.ncsc.gov.uk/cyberessentials/overview)** - "a simple but effective, Government backed scheme that will help you to protect your organisation, whatever its size, against a whole range of the most common cyber attacks." All NHS organisations are now required to be certified to CE+.
  *  **[Government Functional Standard GovS 007: Security](https://www.gov.uk/government/publications/government-functional-standard-govs-007-security)** - "part of a suite of functional standards designed to promote consistent and coherent working within government organisations and across organisational boundaries."

  The OECD's Observatory of Public Sector Innovation (OPSI) also has a useful list of **[worldwide innovation tool-kits](https://oecd-opsi.org/search-toolkits/)** that include other governments takes on digital innovation and development.
