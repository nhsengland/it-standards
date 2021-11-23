---
title: Protecting Data Transfer with TLS
description: >
   **ALL** TCP/IP endpoints must be secured with TLS or an equivalent standard of encryption 
   such that all data transfers are encrypted.
stage: 4. Final Approval Stage
created: 2021-03-29 17:25:00
lastUpdated: 2021-11-23 13:03:26
author: Julian Knight
---

The minimum version of TLS that may be targetted is v1.2 though please note that this may change.
If in doubt, check with the lastest information from [NCSC](https://www.ncsc.gov.uk/guidance/using-tls-to-protect-data) and NIST.

Suitable encryption standards should also be targetted and updated periodically when older standards
are deemed no longer secure. Again, NCSC and NIST recommendations should be referenced.

Certificates used for encryption must be based on well-known Certificate Root Authorities and should have a validity period of no more than 3 years.
Please note that validity periods are generally getting shorter and that browsers may enforce a period. The use of Let's Encrypt is acceptable.

## References

* [NCSC: Using TLS to protect data](https://www.ncsc.gov.uk/guidance/using-tls-to-protect-data)
* [Wikipedia: TLS](https://en.wikipedia.org/wiki/Transport_Layer_Security)
* [NIST: TLS Glossary](https://csrc.nist.gov/glossary/term/transport_layer_security)
* [NIST: Guidelines for the Selection, Configuration, and Use of Transport Layer Security (TLS) Implementations](https://www.nist.gov/publications/guidelines-selection-configuration-and-use-transport-layer-security-tls-0)