---
title: System Authentication
description: >
   Defines the standards for authenticating users to bespoke applications.
stage: 3. Development Stage
created: 2021-04-28 10:00:00
lastUpdated: 2021-11-23 12:47:14
---

In general, **all** systems MUST require a login. Only systems delivering _public_ information will be accessible without a login.

Please refer to the Identity and Access Management strategy and standards before trying to implement a new system. 
We have a number of options in the strategy depending on the requirements.

Internally facing systems MUST always use Single Sign-On based on NHS England's **Azure Active Directory** (AAD). 
Contact the Head of Architecture or the Head of Development in the Corporate IT and Smarter Working team (CISW) for more specific information.

Externally facing systems MUST use our identity service based on **Okta**. 
Contact the Head of Architecture or the Head of Development in the Corporate IT and Smarter Working team (CISW) for more specific information.

Exceptions to the standards listed here may be permissible but must be discussed with CISW in advance and will be subject to
review and approval via the Architecture Review Board (ARB).

## General Notes

* Login data MUST be encrypted at source

  All data for logins MUST be **encrypted before transfer**. In most cases, this means ensuring that all of the communications
  between the client and the server are encrypted using [TLS v1.2](https://www.ncsc.gov.uk/guidance/using-tls-to-protect-data) or better.

* Login forms SHOULD be independent of the system they are securing.

  This facilitates system maintenance windows but allows users to log in and receive notification about maintenance times.
  
  Maintenance windows **MUST NOT** be shown to unauthenticated users.

* Help information MUST NOT include detailed information about security settings

  e.g. password lengths and complexity.
  
  These details must only be available to authenticated users.
  
* **Multi-factor authentication SHOULD be required**
  
  This provides far better security than a complex, often changing password.
  
* Login processing MUST set a minimum password length (not less than 12 characters) 
  but SHOULD NOT have a maximum length
  
  Systems may set a reasonable maximum of 255 characters. In order to prevent password-stuffing and variable overflow vulnerabilities.
  
* Password complexity SHOULD be _allowed_ but NOT _enforced_
  
  Password length is more important than complexity. Enforcement of complexity results in excessive forgotten passwords or ones that are
  insecurely documented.
  
* Systems SHOULD implement background password checks

  So that simplistic and easily guessed passwords are prevented. This may be an out-of-bounds check as long as it is a standard and
  automated process.

* Password change periods should be 12 months or set to not expire.
  
  However, the system may alert the user if not changed in >12m

* Systems SHOULD NOT implement their own login processes

  Pre-existing, dedicated authentication services should always be used so that systems
  get the best quality and security.

* Login forms MUST validate inputs
  
  Of course, this is a universal standard for all user input. Ensure that inputs can only be something sensible.
  Check the length and the allowed characters at least. Apply other checks to ensure that the input data matches the expected
  data type or schema.

  Use common modules and shared functions wherever possible to do these checks to ensure consistency and enable the checks to be updated in a single place.

* Web-based login forms MUST NOT pass data in the URL & MUST use POST not GET
  
  No URL parameters may be used in a login form (e.g. not `/login?id=mypersonalid`) since these may be logged by unsecured proxies.

  Using POST rather than GET helps to enforce this concept.

