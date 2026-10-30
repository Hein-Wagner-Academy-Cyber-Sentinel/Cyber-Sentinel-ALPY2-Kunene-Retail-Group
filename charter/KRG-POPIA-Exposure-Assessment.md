**Kunene Retail Group — POPIA Exposure Assessment**

**1. Purpose**

This document provides a project-level assessment of how Kunene Retail Group may be exposed to risks relating to the Protection of Personal Information Act (POPIA).

This is **not a legal opinion or formal POPIA compliance assessment**.

The purpose is to identify security requirements that can guide the technical design of the project.

**2. Why POPIA Matters to Kunene**

Kunene Retail Group is a South African retailer moving from in-store tills towards e-commerce and card payments.

This business model is likely to involve the processing of personal information belonging to customers and employees.

POPIA aims to protect personal information processed by public and private bodies and establishes minimum requirements for lawful processing. ([South African Government](https://www.gov.za/documents/protection-personal-information-act?utm_source=chatgpt.com))

**3. Potential Personal Information**

For this project, Kunene may need to process information such as:

-   Customer names
-   Contact details
-   Delivery information
-   Customer account information
-   Order information
-   Transaction-related information
-   Employee information
-   User account information

The exact information processed by a real Kunene environment is not provided in the project brief. Therefore, these items are treated as project assumptions.

**4. Main POPIA Exposure Areas**

**4.1 Unauthorised Access**

Customer or employee information could be accessed by someone who does not have permission.

Possible causes include:

-   Stolen credentials
-   Weak authentication
-   Excessive user privileges
-   Compromised employee accounts
-   Compromised store endpoints

**Technical response:**

-   Least-privilege access
-   Strong authentication
-   Role-based access control
-   Secure credential management
-   Logging and monitoring

**4.2 Loss or Disclosure of Personal Information**

Personal information could be lost, copied, disclosed or accessed by an unauthorised person.

POPIA Section 19 requires appropriate and reasonable technical and organisational measures to protect the integrity and confidentiality of personal information. It also requires organisations to identify reasonably foreseeable internal and external risks and maintain appropriate safeguards. ([Justice](https://www.justice.gov.za/legislation/acts/2013-004.pdf?utm_source=chatgpt.com))

**Technical response:**

-   Encryption where appropriate
-   Access controls
-   Secure storage
-   Network protection
-   Security monitoring
-   Backup protection
-   Incident response procedures

**4.3 Excessive Collection or Storage**

A retailer should avoid collecting or keeping information that is not necessary for its intended purpose.

For this project, the technical design should therefore follow a principle of **data minimisation**.

**Technical response:**

-   Store only required information
-   Define retention requirements
-   Delete information when it is no longer required
-   Avoid placing sensitive information in logs
-   Avoid unnecessary copies of personal information

**4.4 Third-Party Processing**

Kunene may use external technology or payment service providers.

Where another party processes personal information on behalf of a responsible party, POPIA places security and confidentiality responsibilities on the parties involved. ([Justice](https://www.justice.gov.za/legislation/acts/2013-004.pdf?utm_source=chatgpt.com))

**Technical response:**

-   Define third-party access
-   Apply least privilege
-   Protect data transferred to service providers
-   Monitor third-party access
-   Ensure appropriate security requirements are documented

**4.5 Security Compromise**

A security incident could result in personal information being accessed or acquired by an unauthorised person.

POPIA Section 22 requires notification of the Information Regulator and affected data subjects where there are reasonable grounds to believe that personal information has been accessed or acquired by an unauthorised person. ([Justice](https://www.justice.gov.za/legislation/acts/2013-004.pdf?utm_source=chatgpt.com))

**Technical response:**

-   Centralised security logging
-   Incident detection
-   Incident response procedures
-   Evidence preservation
-   Defined escalation process
-   Breach notification runbook

**5. POPIA Conditions Relevant to the Project**

POPIA contains eight conditions for lawful processing of personal information. The Information Regulator identifies these as conditions governing lawful processing. ([Empowered Compliance Monitor](https://inforegulator.org.za/popia/?utm_source=chatgpt.com))

For this project, the most technically relevant areas are:

| **POPIA area**                | **Technical consideration**                                                  |
|-------------------------------|------------------------------------------------------------------------------|
| Accountability                | Assign responsibility for protecting information                             |
| Processing limitation         | Avoid unnecessary collection and processing                                  |
| Purpose specification         | Know why information is collected                                            |
| Further processing limitation | Do not reuse information for unrelated purposes without proper justification |
| Information quality           | Keep information accurate where required                                     |
| Openness                      | Make appropriate information available to data subjects                      |
| Security safeguards           | Protect confidentiality and integrity using reasonable safeguards            |
| Data subject participation    | Support appropriate access, correction and related requests                  |

**6. Security Controls Required by the Project**

The POPIA exposure identified above supports the need for the following controls:

**Identity and Access**

-   Least privilege
-   Strong authentication
-   Role-based access
-   Secure administrator access

**Data Protection**

-   Encryption
-   Data minimisation
-   Secure storage
-   Retention and deletion controls

**Endpoint Security**

-   Secure configuration
-   Patch management
-   Reduced attack surface
-   Monitoring of distributed endpoints

**Application Security**

-   Secure e-commerce design
-   Input validation
-   Authentication and authorisation
-   Protection of APIs
-   Secure payment integration

**Monitoring and Incident Response**

-   Centralised logging
-   Security alerts
-   Incident response procedures
-   Evidence collection
-   Breach response process

**7. Connection to the Threat Model**

The POPIA assessment directly supports the threat model.

The three major risk areas identified for Kunene are:

1.  **Payment and personal information compromise**
2.  **Compromise of distributed store endpoints**
3.  **Availability disruption during seasonal demand**

These risks will be examined in more detail in the Threat Model v0.

**8. Project-Level Risk Rating**

| **Exposure**                           | **Impact**  | **Priority** |
|----------------------------------------|-------------|--------------|
| Personal information compromise        | High        | High         |
| Payment-related information compromise | High        | High         |
| Compromised store endpoint             | High        | High         |
| Unauthorised account access            | High        | High         |
| Excessive data retention               | Medium      | Medium       |
| Third-party processing risk            | Medium–High | High         |
| E-commerce availability disruption     | High        | High         |

These ratings are qualitative project assessments, not measurements of an actual Kunene environment.

**9. Conclusion**

Kunene’s transition to e-commerce and card payments increases the importance of protecting personal information and maintaining secure systems.

The POPIA assessment shows that security controls are not separate from the business requirements. They provide a technical way of reducing the risks associated with personal information processing.

The project should therefore use **least privilege, secure authentication, encryption, data minimisation, secure endpoints, monitoring, logging and incident response** as key security principles.

All testing should use simulated information. Real customer information, real payment-card information, credentials and other sensitive information must not be placed in the public project repository.
