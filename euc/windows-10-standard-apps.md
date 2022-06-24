---
title: Windows 10 Standard Applications
description: >
   Defines the standard applications for devices running a desktop OS
stage: 3. Development Stage
created: 2020-06-15 10:00:00
lastUpdated: 2022-06-24 12:42:10
reviewDate: 2022-11-01
---

These are the standard applications that users can expect to have on their Windows 10 desktop OS.

## Common Standard

These are the application standards that must be used for future desktop platforms. Where current services differ from this standard, the differences are noted in the following sections.

- Windows 10 Enterprise
  
  Utilises the NHS M365 license agreement that includes W10E E5 licensing with Advanced Threat Protection.

- Anti-malware: Windows Defender
  
  No other live anti-malware tools should be included as these can cause support issues.

- Microsoft Office 365 (Click-to-run)
  
  The Office 365 version of Microsoft Office Pro-Plus is used throughout with all users being licensed for O365 E5.

  Includes: Word, Excel, PowerPoint, OneNote, Access, Outlook

- Browsers
  
  - Microsoft Edge (Chromium)
    
    As the new Edge is Chromium based, there is no need to include Chrome. Edge includes enterprise support modes which Chrome does not. Chrome also may leak browsing data to Google. Edge returns data to Microsoft but this is covered by much stricter privacy agreements.

    Edge's enterprise support includes "IE Mode". This allows for an exceptions list for sites known to need to use legacy IE. Such sites will be transparently set to use the legacy IE libraries.

    Staff are strongly encouraged to make use of Edge's profile synchronisation feature to ensure that their bookmarks, open tabs/windows, browsing history, etc are all backed up and available to different devices (including mobile and any replacement desktops). Profiles should also be used to keep multiple accounts on similar systems separate from each other (e.g. Office 365 and NHSmail).

  - Firefox
    
    Available as an alternative to Edge.

- File Compression: 7zip
- Password Management: Password Safe

- Collaboration

  - Microsoft Teams
  - Microsoft Whiteboard

## Other - Freely installable

Many common applications are made available either via a self-service "Company Portal" without the need for service desk involvement.

These include:

* Visual Studio Code
* R and R-Studio
* Python
* ... TBC ...

## Other - Restricted deployment

In addition, there are a variety of applications that may be requested via the standard *Technology Request & Requirements Form* in the Service Now self-service portal.

Typically, these are chargable applications and so will require approval from a budget-holder before being released.

Examples include:

* Microsoft Project
* Microsoft Visio
* Adobe Acrobat Pro

## Non-standard applications

Non-standard applications may be requested via the *Technology Request & Requirements Form* on the IT Service Portal (Service Now) and will be assessed by the weekly Technical Design Authority.

However, even where such software has a free license, there is still a cost to the organisation for maintaining it and so that cost must be recovered from a budget.

Users should always check the available catalogue for existing applications before spending time on a bespoke request.