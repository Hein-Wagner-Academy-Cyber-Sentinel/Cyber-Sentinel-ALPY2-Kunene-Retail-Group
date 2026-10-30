# KUNENE RETAIL GROUP

**Executive Business Profile & Security Architecture Summary**

- **Type:** Multi-Branch Retailer

- **Persona:** Simulated SA Business

- **Project Group:** Pair 2

## 1. BUSINESS OVERVIEW & DIGITAL TRANSFORMATION

Kunene Retail Group is a growing, simulated South African multi-branch retailer transitioning from traditional in-store tills to e-commerce and electronic card payments. The objective of this project is to design a secure, code-defined platform that supports business expansion while safeguarding sensitive data and ensuring high availability. Moving online increases the number of interacting systems and users, requiring robust protection for customer personal data, online accounts, orders, payment transactions, store endpoints, administrator accounts, and inventory records.

### Core Security Risk Areas

- Payment card data exposure & financial fraud

- Distributed store endpoints across multiple branches

- Seasonal increases in transaction & traffic demand

### Key Growth Pressures

```
- Higher online transaction & customer data volumes
```

- Expanded attack surface with more systems & endpoints

- Greater need for continuous service reliability during peaks

## 2. CRITICAL BUSINESS ASSETS

| Asset Category | Strategic & Operational Importance |
| - | - |
| **Customer Personal Info** | Must be protected from unauthorised access or disclosure (names, contact & delivery details). |
| **Payment-Related Info** | Compromise could cause severe financial loss and security consequences. |
| **E-Commerce & Availability** | Required for online sales; customers must have reliable access, especially during busy periods. |
| **Store Endpoint Systems** | Deployed across multiple retail branches, significantly increasing the enterprise attack surface. |
| **Accounts & Credentials** | Customer, employee, and admin credentials could be abused to gain unauthorised access. |
| **Orders & Inventory Data** | Essential for core retail operations, order fulfilment, and customer service. |


## 3. SECURITY PRIORITIES, POPIA RELEVANCE & STAKEHOLDERS

### Core Security Priorities

- Protect personal and payment-related information as mandated by the PCIDSS

- Control system/data access & protect user/employee accounts

- Secure distributed retail store endpoints

- Maintain e-commerce platform availability during peaks

- Detect and respond to security incidents effectively

- Keep security evidence in accessible, text-based formats

- Apply POPIA safeguards & avoid storing unnecessary sensitive data

### POPIA & PCIDSS Compliance Relevance

Retail and online activities process personal information (names, contact details, delivery addresses, transaction records). POPIA requires meeting conditions for lawful processing and applying appropriate security safeguards.

As KRG processes payment card information, it is also required to meet all security obligations as required by the PCIDSS.

### Key Stakeholders (Identified & Assumed)

Customers, store employees, branch management, business management, IT & security personnel, payment/technology service providers, and product vendors.

## 4. PROJECT ASSUMPTIONS & SCOPE BOUNDARIES

### Project Assumptions

- Operates 30 physical branches connected to business systems; 10 in the Western-Cape, 10 in Gauteng, 5 in Eastern Cape and 5 in Kwazulu-Natal.

- Uses an online retail platform & electronic payment services

- Experiences seasonal demand surges

- Uses simulated data only (no real customer or payment data)

### Out of Scope

- Accessing or modifying real Kunene production systems

- Using real customer info, payment-card data, or credentials

- Providing a formal legal opinion on POPIA compliance

