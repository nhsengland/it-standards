**ALL** TCP/IP endpoints must be secured with TLS or an equivalent standard of encryption such that all data transfers are encrypted.

The minimum version of TLS that may be targetted is v1.2 though please note that this may change.
If in doubt, check with the lastest information from NCSC and NIST.

Suitable encryption standards should also be targetted and updated periodically when older standards
are deemed no longer secure. Again, NCSC and NIST recommendations should be referenced.

Certificates used for encryption must be based on well-known Certificate Root Authorities and should have a validity period of no more than 3 years.
Please note that validity periods are generally getting shorter and that browsers may enforce a period. The use of Let's Encrypt is acceptable.
