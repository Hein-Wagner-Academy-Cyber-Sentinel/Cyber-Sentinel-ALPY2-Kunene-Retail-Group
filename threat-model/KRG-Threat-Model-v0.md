# Kunene Retail Group — Threat Model v0

## 1. Purpose

This threat model identifies the main assets, actors, entry points and security risks for the Kunene Retail Group project.

Kunene is a simulated multi-branch retailer moving from in-store tills towards e-commerce and card payments.

This is **Threat Model v0**, so it provides an initial risk view that will be refined during later project phases.

## 2. Business Context

Kunene Retail Group is expanding its digital retail operations.

The project brief identifies three dominant risk themes:

1. Payment card data

2. Distributed store endpoints

3. Seasonal load

The threat model focuses on these areas because they can directly affect customer information, business operations and service availability.

## 3. Important Assets

| **Asset** | **Description** | **Security importance** |
| :-: | :-: | :-: |
| Customer personal information | Information associated with customers and their orders | Confidentiality and privacy |
| Payment-related information | Information associated with electronic payments | Confidentiality and integrity |
| E-commerce platform | Online system used by customers to access and purchase products | Availability, integrity and confidentiality |
| Store endpoints | Computers and other systems used across branches | Confidentiality, integrity and availability |
| User accounts | Customer, employee and administrator accounts | Access control |
| Credentials | Passwords, authentication information and access secrets | Prevent unauthorised access |
| Orders and transactions | Information about purchases and transactions | Integrity and availability |
| Inventory information | Information required for retail operations | Integrity and availability |
| Security logs | Records used to detect and investigate security events | Integrity and availability |
| Online service availability | Ability of customers to access the online platform | Availability |


## 4. Threat Actors

### 4.1 External Cyber-criminal

An external attacker may attempt to gain access to customer information, payment-related information or business systems.

Possible methods include:

- Credential attacks

- Exploiting vulnerable applications

- Automated scanning

- Web attacks

- Malware

### 4.2 Compromised Customer Account

An attacker may obtain a legitimate customer’s credentials and use the account to access information or perform unauthorised activities.

### 4.3 Compromised Employee Account

An employee account could be compromised through phishing, stolen credentials or another attack.

An attacker could then use the account to access internal systems.

### 4.4 Malicious Insider

An authorised employee could intentionally misuse access to information or systems.

### 4.5 Compromised Store Endpoint

A branch computer or other endpoint could become compromised and provide an attacker with a starting point for further attacks.

### 4.6 Third-Party or Service Provider Risk

A technology or payment service provider could introduce additional security risks if its systems, credentials or integrations are compromised.

## 5. Entry Points

The following entry points are considered relevant to the project:

### E1 — E-commerce Website

The public-facing website is exposed to customers and potentially to internet-based attackers.

### E2 — Customer Login

Customer authentication creates a possible entry point for credential theft and account takeover.

### E3 — Payment Integration

Payment processing creates an important security boundary because payment-related information may pass through or interact with the platform.

### E4 — Store Endpoints

Computers and other systems used at different branches provide multiple possible entry points.

### E5 — Branch Network

The network connecting branch systems can provide an attacker with opportunities to move between systems if it is not properly secured.

### E6 — Administrative Access

Administrative interfaces provide privileged access and therefore require strong protection.

### E7 — Third-Party Integrations

External services and APIs may introduce additional trust relationships and attack paths.

## 6. Three Most Material Risks

### Risk 1 — Payment and Personal Information Compromise

**Asset:** Customer personal information and payment-related information

**Threat actor:** External cybercriminal or compromised account

**Entry points:** E-commerce website, customer login, payment integration

**Threat:** An attacker gains unauthorised access to customer or payment-related information.

**Potential impact:**

- Exposure of customer information

- Financial harm

- Loss of customer trust

- Business disruption

- Regulatory consequences

- Reputation Damage

**Likelihood:** High

**Impact:** High

**Risk level:** High

**Reason:** Kunene is specifically moving into e-commerce and card payments, making payment and personal information an important security priority.

### Risk 2 — Compromise of Distributed Store Endpoints

**Asset:** Store endpoint systems and connected business resources

**Threat actor:** External cybercriminal, compromised employee or malicious insider

**Entry points:** Store endpoints and branch network

**Threat:** An attacker compromises a branch endpoint and uses it to access information or other systems.

**Potential impact:**

- Loss of business information

- Malware infection

- Unauthorised access

- Lateral movement

- Business disruption

**Likelihood:** High

**Impact:** High

**Risk level:** High

**Reason:** Kunene operates across multiple branches. More endpoints create more systems that need to be secured and monitored.

### Risk 3 — E-commerce Availability Disruption During Seasonal Load

**Asset:** E-commerce platform and online services

**Threat actor:** External attacker or service disruption

**Entry points:** Public e-commerce website and APIs

**Threat:** The online service becomes unavailable or severely degraded during a period of high demand.

**Potential impact:**

- Lost sales

- Customers unable to place orders

- Poor customer experience

- Operational disruption

- Damage to business reputation

**Likelihood:** Medium–High

**Impact:** High

**Risk level:** High

**Reason:** Seasonal load is one of Kunene’s dominant risk themes. An availability problem during a busy period could have a larger business impact than the same disruption during a quiet period.

## 7. Risk Summary

| **Risk** | **Likelihood** | **Impact** | **Priority** |
| :-: | :-: | :-: | :-: |
| Payment and personal information compromise | High | High | High |
| Distributed store endpoint compromise | High | High | High |
| E-commerce availability disruption | Medium–High | High | High |


## 8. Initial Security Requirements

The threat model indicates that the platform should eventually include:

- Strong identity and access controls

- Least-privilege access

- Secure authentication

- Endpoint hardening

- Network segmentation

- Encryption

- Secure application configuration

- Secure payment integration

- Logging and monitoring

- Incident response procedures

- Backup and recovery capabilities

- Availability and resilience controls

These controls will be designed and tested in later project phases.

## 9. Assumptions and Limitations

This is an initial threat model for a simulated business persona.

The project brief does not provide:

- Kunene’s actual number of branches; we assume 30 branches.

- Its actual network architecture

- Its actual software platforms

- Its actual payment provider

- Its actual security controls

- Its actual customer database

Therefore, these details have not been presented as facts.

The threat model will be updated as the project architecture and technical implementation develop.

## 10. Threat Model v0 Conclusion

The initial threat model identifies three priority areas for Kunene Retail Group:

1. Protection of payment and personal information

2. Security of distributed store endpoints

3. Availability of e-commerce services during seasonal demand

These risks will guide the security architecture, infrastructure, hardening, container, CI/CD, monitoring and incident-response work in later phases.

