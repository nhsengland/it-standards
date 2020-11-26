# NHSmail Single Sign On

[NHSmail][1] provide a single sign on service for organisations who would like to enable [NHSmail single sign][2] on for other web and desktop applications.

Full technical documentation regarding implementing NHSmail Single Sign On can be found [here][3]

## As-Is position

NHSmail is currently the primary email provider for NHS England and NHS Improvement. Across the Health and Care community, NHSmail has close to 1.5m users, with more than half-a-million staff using the platform on a daily basis.

The FutureNHS Platform is currently testing NHSmails Single Sign On service with a view to providing this as an optional way of signing into its Kahootz based platform. As of 18 September 2020, over 50% of FutureNHS platform users (63,076) currently use their @nhs.net email address to login to the platform. It is hoped the implementation of NHSmail SSO will provide an enhanced experience for the majority of the platform's users with regards to logging in and registration. 

The platform will be using the SAML 2.0 federation protocol to provide this function via the NHSmail Active Directory Federation Services. 

### Benefits

#### For FutureNHS users (with NHSmail accounts): 

- Replacing many of the current disparate usernames and passwords with a single NHSmail credential 

- Users will not be re-prompted for credentials when signing on to multiple applications integrated to NHSmail authentication, for example Outlook Web Application (OWA), the NHSmail Portal, third-party integrated applications etc. 

- Self-service password reset and unlock, along with 24x7 helpdesk support for any NHSmail account issues 

#### For the FutureNHS service 

- Enables us to more easily migrate NHSmail users from the old platform to the new platform. 

- Enhances security as users are less likely to write passwords down as they have fewer to remember 

- No need to issue new credentials per application and the account management lifecycle is already managed through existing NHSmail account lifecycle processes 

- Enhanced security processes – Multi-Factor Authentication (MFA), compromised account detection etc 




[1]: https://digital.nhs.uk/services/nhsmail
[2]: https://support.nhs.net/knowledge-base/single-sign-on-guide/
[3]: https://s3-eu-west-1.amazonaws.com/comms-mat/Comms-Archive/NHSmail+Single+Sign-on+Technical+Guidance.pdf
[4]: https://digital.nhs.uk/services/nhsmail


