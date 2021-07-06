---
title: End User Email Services
description: >
   Standards and requirements for user-facing email.
stage: 3. Development Stage
created: 2021-07-06 14:24:16
lastUpdated: 2021-07-06 14:24:22
author: Julian Knight
---

NHSEI use two email services, our own Office 365 Exchange Online and the NHSmail service.

At the time of writing, NHSmail is the primary service and O365 the secondary. This may change in the future.

Both systems are certified to the NHS [DCB1596 Secure Email Standard](https://digital.nhs.uk/data-and-information/information-standards/information-standards-and-data-collections-including-extractions/publications-and-notifications/standards-and-collections/dcb1596-secure-email). A standard under the provision of section 250 of the Health and Social Care Act 2012.

Either system is certified therefore for the exchange of OFFICIAL-SENSITIVE information including personal and patient identifiable.

!> Other email systems MUST NOT be used for NHSEI official business. Under no circumstances may personal or consumer email services be used for NHSEI business.

?> Note that the exchange of OFFICIAL-SENSITIVE information may be subject to other Information Governance policies. If in doubt, please contact your local or national IG representative.

## Sending limits

Both systems have limits on how much email can be sent. The NHSmail limits are fixed. Some of the NHS England limits may be changable. However, note that both use Office 365 and are therefore subject to those limits as well. Because NHSmail is a single tenancy for over 400 organisations and 2 million people, it is generally subject to stricter limits than our own service.

Typically, you can only send to a maximum of 400 individually addressed people in a single email. However, you can get round this by having a Distribution Group created.

Any single account is prevented from sending more than 10,000 emails in a day and may send no more than 30 emails per minute.

## Long-term storage and archiving

?> Note that email is NOT considered an archive. Nor is email considered an organisational _record_. Please see the Records Management policy and guidance from the Records Management team for specific information on record-keeping. Email is a transient communications tool. There is no guarentee that emails will be retained for a long period.

Both email systems have an archiving mailbox attached. To use the archive mailbox, you have to manually move old emails to the other mailbox.

When trying to free space in your main mailbox, note that your "Deleted Items" count towards your mailbox limit. Also note that NHSmail does not immediately free up space even if your deleted items are cleared.

NHSmail accounts normally have a limit of 4GB. NHS England mailboxes have a standard limit of 50GB (which can be changed on request). The archive mailboxes are theoretically "unlimited" but may have practical limits.

## References

* [Exchange Online limits - Service Descriptions | Microsoft Docs](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)
* [DCB1596 Secure Email Standard](https://digital.nhs.uk/data-and-information/information-standards/information-standards-and-data-collections-including-extractions/publications-and-notifications/standards-and-collections/dcb1596-secure-email)