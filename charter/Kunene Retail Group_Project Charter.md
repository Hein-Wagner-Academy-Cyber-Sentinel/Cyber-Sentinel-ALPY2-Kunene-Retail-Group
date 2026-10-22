**Kunene Retail Group — Project Charter**

**1. Project Information**

**Project:** Build It Anywhere — A Zero-Cost, Code-Defined Secure Platform

**Business Persona:** Kunene Retail Group

**Pair:** Pair 2

**Project Phase:** Phase 1 — Foundation and Charter

**Project Period:** 21 August 2026 – 30 July 2027

**2. Project Purpose**

The purpose of this project is to design and demonstrate a secure, code-defined platform for Kunene Retail Group.

The platform will support Kunene’s transition from traditional in-store tills towards e-commerce and card payments.

Security decisions will be connected to business risks, privacy requirements and measurable technical evidence.

**3. Business Problem**

Kunene is a growing multi-branch retailer modernising its operations.

Moving towards e-commerce and electronic payments introduces additional security concerns, including:

-   Protection of customer information
-   Protection of payment-related information
-   Security of distributed store endpoints
-   Protection of user accounts
-   Availability of online services
-   Increased seasonal demand

The project must therefore demonstrate how security can be built into the platform rather than added only after deployment.

**4. Project Objectives**

The project aims to:

1.  Understand Kunene’s business and security requirements.
2.  Identify the most important threats and risks.
3.  Design a secure platform using code-defined infrastructure.
4.  Apply security hardening to systems.
5.  Build and secure containerised workloads.
6.  Create a CI/CD pipeline that checks security automatically.
7.  Design disaster recovery procedures.
8.  Assess security risks associated with an AI feature.
9.  Develop an incident response process.
10. Model the cost of the proposed cloud platform without deploying it.
11. Produce accessible, reproducible technical evidence.

**5. Phase 1 Objectives**

During Phase 1, the project team will:

-   Confirm the pair and working protocol.
-   Establish the project repository.
-   Verify the required toolchain.
-   Research Kunene Retail Group.
-   Assess POPIA exposure.
-   Create Threat Model v0.
-   Define the project scope.
-   Define success criteria.
-   Document assumptions.
-   Define what is out of scope.
-   Record evidence using accessible text-based methods.

**6. Project Scope**

**In Scope**

The project includes:

-   Business and security research
-   POPIA exposure assessment
-   Threat modelling
-   Secure architecture design
-   Infrastructure as code
-   Linux security hardening
-   Container security
-   CI/CD security controls
-   Disaster recovery planning
-   AI security and governance assessment
-   Incident response
-   Cloud cost modelling
-   Automated testing
-   Security evidence
-   Technical documentation

The implementation will use simulated environments and data.

**7. Out of Scope**

The following are outside the project scope:

-   Access to real Kunene Retail Group systems
-   Use of real customer personal information
-   Use of real payment-card information
-   Use of real passwords, API keys or credentials
-   Production deployment for Kunene
-   Real-world penetration testing against Kunene
-   Formal legal advice or certification for POPIA compliance
-   Purchasing paid infrastructure or services for the project

**8. Success Criteria**

The project will be considered successful when:

**Repository**

-   The project repository is created and organised.
-   Required project documentation is stored in the repository.
-   No real credentials or personal information are committed.

**Phase 1**

-   Business profile completed.
-   POPIA exposure assessment completed.
-   Threat Model v0 completed.
-   Project charter completed.
-   Required development tools are verified.
-   CI pipeline is operational.
-   Evidence is recorded using Asciinema and other approved formats.

**Technical Project**

The later project phases should demonstrate measurable security improvements through testing, logs, scans, pipeline results and other reproducible evidence.

**Accessibility**

Technical evidence must be understandable without requiring visual interpretation.

**9. Key Risks**

The initial project risks are:

| **Risk**                                           | **Priority** | **Response**                                                                |
|----------------------------------------------------|--------------|-----------------------------------------------------------------------------|
| Payment/personal information compromise            | High         | Strong access control, encryption, secure application design and monitoring |
| Distributed endpoint compromise                    | High         | Hardening, least privilege, segmentation and monitoring                     |
| E-commerce availability disruption                 | High         | Resilience, backups, recovery planning and availability testing             |
| Accidental exposure of credentials                 | High         | Secret management and repository checks                                     |
| Incorrect assumptions about the simulated business | Medium       | Clearly document assumptions and update them as the project develops        |

**10. Assumptions**

The project assumes:

-   Kunene is a simulated South African retail business.
-   Kunene operates multiple branches.
-   Kunene is moving towards e-commerce and card payments.
-   Customer and employee information may be processed.
-   Store endpoints are distributed across branches.
-   Seasonal periods may increase demand.
-   Testing will use simulated data.
-   Project infrastructure will be designed and tested in controlled environments.
-   No real customer or payment information will be used.

Where information is not provided by the project brief, it will be labelled as an assumption.

**11. Evidence Strategy**

The project will use accessible and reproducible evidence.

-   Terminal transcripts
-   Asciinema recordings
-   Configuration files
-   Git history
-   CI/CD pipeline results
-   Scanner reports
-   Security logs
-   Automated test results
-   Text-based diagrams
-   Runbooks

Screenshots will not be used as the primary evidence format.

**12. Repository Structure**

The project repository will use the following structure:

README.md

charter/

threat-model/

architecture/

infrastructure/

hardening/

containers/

.github/workflows/

runbooks/

ai/

automation/

cost/

evidence/

reflections/

This structure will allow each phase to add its artefacts without losing traceability.

**13. Working Principles**

The project team will follow these principles:

-   Security by design
-   Least privilege
-   Minimise unnecessary data
-   Automate security checks where possible
-   Keep infrastructure defined as code
-   Produce reproducible evidence
-   Use only simulated data
-   Never commit secrets
-   Document assumptions
-   Measure security improvements
-   Keep technical decisions connected to business risks

**14. Roles and Collaboration**

The project is being completed by Pair 2.

The pair will use a collaborative working model with role rotation so that both members gain experience across the project.

Work will be tracked through the project repository and documented through commits and evidence.

**15. Phase 1 Deliverables**

The Phase 1 deliverables are:

-   Business Profile
-   POPIA Exposure Assessment
-   Threat Model v0
-   Project Charter
-   Toolchain verification evidence
-   Passing pipeline evidence
-   Asciinema evidence

**16. Conclusion**

The project will provide Kunene Retail Group with a simulated secure platform design based on its business needs and identified security risks.

The initial work establishes the foundation for the remaining phases by identifying the business context, POPIA exposure, threats, project scope and success criteria.

The three most important initial security concerns are:

1.  Protecting payment and personal information
2.  Securing distributed store endpoints
3.  Maintaining e-commerce availability during seasonal demand
