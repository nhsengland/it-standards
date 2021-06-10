---
title: Windows 10 Standard Applications
description: >
   Defines the standard applications for devices running a desktop OS
stage: 3. Development Stage
created: 2020-06-15 10:00:00
lastUpdated: 2020-06-19 21:46:45
reviewDate: 2021-01-01
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

  - Firefox
    
    Available as an alternative to Edge.

- File Compression: 7zip

- Collaboration

  - Microsoft Teams
  - Microsoft Whiteboard

## NHS England specific

Only differences from the [Common Standard](#common-standard) are listed.

TBC

- Anti-malware: Trend
  
- Browsers
  
  - Internet Explorer 11
  - Google Chrome
  - Firefox

  IE11 will be replaced by Microsoft Edge (Chromium) with enterprise mode configured to redirect sites known to need IE to use the built-in IE-mode. It is possible that Chrome will then be removed.

## NHS Improvement specific

Only differences from the [Common Standard](#common-standard) are listed.

TBC

- Anti-malware: Kasperski
  
- Browsers
  
  - Internet Explorer 11
  - Google Chrome
  - Firefox

  IE11 will be replaced by Microsoft Edge (Chromium) with enterprise mode configured to redirect sites known to need IE to use the built-in IE-mode. It is possible that Chrome will then be removed.

## NHSX Specific

Only differences from the [Common Standard](#common-standard) are listed.
