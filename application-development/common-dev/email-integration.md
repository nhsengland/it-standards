---
title: Email Integration for Business Applications
description: >
   Standards and requirements for the integration of email with business applications.
stage: 3. Development Stage
created: 2021-07-06 13:57:02
lastUpdated: 2022-06-24 10:29:18
author: Julian Knight
---

## Sending

Any application requiring the ability to send emails will need access to a suitable _mail relay_.

Both NHS England's Exchange Online (Office 365) and NHSmail services have mail relay's available. Both of these mail systems are secured to the [DCB1596 standard](https://digital.nhs.uk/data-and-information/information-standards/information-standards-and-data-collections-including-extractions/publications-and-notifications/standards-and-collections/dcb1596-secure-email).

Mail sending must be carefully controlled to prevent the relay from being marked as a source of SPAM. In particular, mass mailing should be done via a dedicated mass-mailing service and must not use the user-facing Exchange Online and NHSmail services.

Connections to a mail relay MUST be secured using [TLS v1.2+](https://www.ncsc.gov.uk/guidance/using-tls-to-protect-data) or an equivalent, standards-based and approved security mechanism.

Any mail relay in use MUST be a closed relay so that non-authenticated connections cannot use the relay.

## Receiving

Any application requiring the ability to receive email MUST require inbound connections to be secured using [TLS v1.2+](https://www.ncsc.gov.uk/guidance/using-tls-to-protect-data) or an equivalent, standards-based and approved security mechanism.

Receiving applications:

* MUST have the ability to deal with SPAM, Phishing and other malicious emails.
* MUST have the ability to deal with unwanted and unsafe email attachments.

Such security requirements may be dealt with by an upstream mail receiving service (e.g. Exchange Online). In that case, the application must connect to the service over a [TLS v1.2+](https://www.ncsc.gov.uk/guidance/using-tls-to-protect-data) secured Exchange, HTTPS, IMAP or POP3 connection. Any such connection MUST be authenticated using a dedicated service account. Credentials for accounts must be protected and stored in a suitable keystore.

Integrations to upstream email services MUST be documented not only in the application documentation but also in the upstream service documentation. The NHS England Configuration Management Database (CMDB) in Service Now is a suitable place for such information to be stored.

!> Undocumented interfaces MAY be disabled at any time.

## Security

As noted, ALL connections to and from email services and servers MUST use encrypted links and MUST be authenticated.

It should be noted that the exchange of OFFICIAL-SENSITIVE information MUST use a mail service that is certified to the [DCB1596 standard](https://digital.nhs.uk/data-and-information/information-standards/information-standards-and-data-collections-including-extractions/publications-and-notifications/standards-and-collections/dcb1596-secure-email). This includes personally and patient identifiable information. 

Any application that handles information classified at OFFICIAL-SENSITIVE or above is required to register with the NHS England Information Asset Management System (IAMS). Please contact your Information Governance representative for further information.

Exchange of information classified at SECRET or above will require additional handling measures. Contact the NHS England IT/Cyber Security team for details.

## On-premise vs Cloud Email services

In line with the NHS England, NHS and Government strategies, only cloud-based email services should be used.

Applications using legacy on-premise mail services must plan for and deploy alternative services.