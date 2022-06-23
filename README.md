# (W3SC) Web3 System Controls
June 22, 2022 this project is being moved to [Game7 DAO](https://github.com/G7DAO/w3sc)

The goal of this project is to create an opensource and collaborative security
controls checklist that the industry can use as a security guide. With enough
community input, we hope this guide will eventually be viewed as "Best Practice" and potentially evolve into an open security standard for Web3.

This project is a WIP and is being actively developed. Frequent changes to the contents of this project should be expected.
This project was launched for the primary purpose of beginning the conversation around Web3 Security 
Best Practice.

## Attribution
The following organizations and people have contributed to this guide and will be listed as Authors of the final specification:
* [Game7](https://game7.io/)
* DCentn
* BlockSecNerd
* [Moonstream](https://moonstream.to)
* [Kompotkot](https://github.com/kompotkot)

_note: Attribution is very import. Please feel free to point out any deficiencies._ 

## W3SC Roadmap

### Stage 1 - Checklists

- [x] [Hello World](https://github.com/G7DAO/w3sc/README.md) - 04/2022
- [x] [Access Controls](https://github.com/G7DAO/w3sc/blob/main/checklists/access-controls.md) - 04/2022
- [x] [Change Management](https://github.com/G7DAO/w3sc/blob/main/checklists/change-management.md) - 04/2022
- [x] [Critical Information Communication](https://github.com/G7DAO/w3sc/blob/main/checklists/critical-information.md) - 04/2022
- [x] [Incident Response](https://github.com/G7DAO/w3sc/blob/main/checklists/incident-response.md)  - 04/2022
- [x] [Network Security](https://github.com/G7DAO/w3sc/blob/main/checklists/network-security.md) - 04/2022
- [x] [Organizational Management](https://github.com/G7DAO/w3sc/blob/main/checklists/organizational-management.md) - 04/2022
- [x] [Risk Assessment](https://github.com/G7DAO/w3sc/blob/main/checklists/risk-assessment.md) - 04/18/2022
- [x] [Vulnerability Management](https://github.com/G7DAO/w3sc/blob/main/checklists/vulnerability-management.md) - 04/2022
- [x] [Physical Security](https://github.com/G7DAO/w3sc/blob/main/checklists/physical-security.md) - 04/2022
- [x] [Confidentiality](https://github.com/G7DAO/w3sc/blob/main/checklists/confidentiality.md) - 04/2022
- [x] [Availability](https://github.com/G7DAO/w3sc/blob/main/checklists/availability.md) - 04/2022
- [x] [Business Continuity](https://github.com/G7DAO/w3sc/blob/main/checklists/business-continuity.md) - 04/2022
- [x] [Information Security](https://github.com/G7DAO/w3sc/blob/main/checklists/information-security.md) - 04/2022
- [ ] [Penetration Testing](#) - 08/2022
    - [x] [Web Penetration Testing](https://github.com/G7DAO/w3sc/blob/main/checklists/penetration-testing/penetration-testing-web.md) - 04/2022
- [ ] [Smart Contracts](#) - 08/2022
    - [x] [Solidity Smart Contract Checklist](https://github.com/G7DAO/w3sc/blob/main/checklists/smart-contracts/solidity-checklist.md) - 04/2022
- [ ] End–users, Employees, Contractors and Management - 04/2022
- [ ] Privacy - 04/2022
- [ ] Community - 05/2022
- [ ] Cloud Security - 05/2022
- [ ] Application security - 05/2022
- [ ] Operational security - 05/2022
- [ ] Disaster recovery - 05/2022
- [ ] Resilience - 05/2022
- [ ] Integrity - 05/2022
- [ ] Automation - 05/2022
- [ ] Tokens and Keys - 06/2022
- [ ] Web3 Controls - 06/2022
- [ ] Offensive OpSec - 06/2022
- [ ] Whitehat Hacker - 06/2022

### Stage 2 - Best Practice
TODO

### Standards
This guide follows existing Cybersecurity, Network Security, Operations Security, Information Security and Personal Security best practice as described in the following specifications. _A brief description of each of these standards can be found at the bottom of this document._
* **Information security management system (ISMS) (ISO/IEC 27000 Family):** ISO/IEC 27001, ISO/IEC 27002, ISO/IEC 27003, ISO/IEC 27004, ISO/IEC 27005, ISO/IEC 27006, and ISO/IEC 27007
* **System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA)**
* **Common Criteria (ISO/IEC 15408)**
* **ISO/IEC 18043**
* **Center of Internet Security, CIS (https://www.cisecurity.org/)**
* **ISO 22301:2012**
* **National Information Security Technology (NIST) Standard Specification**
* **SANS Security Policy Resource**
* **ISO 28000**
* **OWASP Foundation**
* **ISO/IEC 27037**
* **Payment Card Industry Data Security Standard (PCI DSS)**
* **Cloud Security Alliance (CSA)**
* **ISO/SAE 21434**
* **ISO/IEC 20243-1**

### Standards Described
**SOC 2 Type 2**

System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA). They're intended to examine services provided by a service organization so that end users can assess and address the risk associated with an outsourced service.

A SOC 2 Type 2 attestation is performed under:

* SSAE No. 18, Attestation Standards: Clarification and Recodification, which includes AT-C section 105, Concepts Common to All Attestation Engagements, and AT-C section 205, Examination Engagements (AICPA, Professional Standards).
* SOC 2 Reporting on an Examination of Controls at a Service Organization Relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy (AICPA Guide).
* TSP section 100, 2017 Trust Services Criteria for Security, Availability, Processing Integrity, Confidentiality, and Privacy (AICPA, 2017 Trust Services Criteria).

**SOC 3 overview**

System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA). They are intended to examine services provided by a service organization so that end users can assess and address the risk associated with an outsourced service.

SOC 3 SOC for Service Organizations: Trust Services Criteria for General Use Report is a short, publicly facing version of the SOC 2 Type 2 attestation report for users who need assurances about service organization's controls relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy but do not need a full SOC 2 report. Because SOC 3 reports are general use reports, they can be freely distributed.

A SOC 3 report contains a written assertion by service organization management regarding control effectiveness to achieve commitments based on the applicable trust services criteria, as well as service auditor's opinion on whether management's assertion is stated fairly.

**ISO/IEC 27001 overview**

The International Organization for Standardization (ISO) is an independent nongovernmental organization and the world's largest developer of voluntary international standards. The International Electrotechnical Commission (IEC) is the world's leading organization for the preparation and publication of international standards for electrical, electronic, and related technologies.

Published under the joint ISO/IEC subcommittee, the ISO/IEC 27000 family of standards outlines hundreds of controls and control mechanisms to help organizations of all types and sizes keep information assets secure. These global standards provide a framework for policies and procedures that include all legal, physical, and technical controls involved in an organization's information risk management processes.

ISO/IEC 27001 is a security standard that formally specifies an Information Security Management System (ISMS) that is intended to bring information security under explicit management control. As a formal specification, it mandates requirements that define how to implement, monitor, maintain, and continually improve the ISMS. It also prescribes a set of best practices that include documentation requirements, divisions of responsibility, availability, access control, security, auditing, and corrective and preventive measures. Certification to ISO/IEC 27001 helps organizations comply with numerous regulatory and legal requirements that relate to the security of information.


**Information security management system (ISMS) (ISO/IEC 27000 Family):**  It is a set of guidelines for maintaining infrastructure, mainly the company's data centers, to follow certain legal, technical and physical policies to ensure confidentiality, integrity, and availability of data reside in the company's data centers. It consists of a set of ISO/IEC 27001, ISO/IEC 27002, ISO/IEC 27003, ISO/IEC 27004, ISO/IEC 27005, ISO/IEC 27006, and ISO/IEC 27007.

**Common Criteria (ISO/IEC 15408):** This standard mainly deals with the certification of IT products. It ensures the evaluation of IT products based on a set of approving standards that are widely followed by industry and governments. ISO/IEC 15408 consists of three parts: Part 1 (Introduction and general model), Part 2 (Security functional requirements), and Part 3 (Security assurance requirements). The Common Evaluation Methodology (CEM) is another document used by security auditors to evaluate IT products. You can get more information on the link: https://www.commoncriteriaportal.org/.

**ISO/IEC 18043:** This standard helps an organization in the selection, deployment, and operations of intrusion detection systems within an organization's IT infrastructure.

**Center of Internet Security, CIS (https://www.cisecurity.org/):** CIS publishes security benchmarks for mobile devices, network devices, server operating systems, virtualization platforms and cloud, desktops, and web browsers. These benchmarks are security configuration guides that governments, the industry widely accept and are available for free. Most of the security auditing organizations used these benchmarks to evaluate the configuration of IT infrastructure.

**ISO 22301:2012:** This standard contains requirements of Business continuity management systems.

**National Information Security Technology (NIST) Standard Specification:** NIST is a US-based agency that publishes cybersecurity-related standards. Most of the cryptography-related standards come from NIST, and different countries across the globe widely follow it. NIST 800-115 (Technical Guide to Information Security Testing and Assessment) is an important standard for assessing the IT system.

**SANS Security Policy Resource:** This resource contains templates related to network devices, servers, and application security.

**ISO 28000:** This ISO standard contains the specification for security management systems for the supply chain.

**OWASP Foundation:** It is a non-profit organization that regularly publishes Top 10 security issues of the web application, mobile, web services, etc. Most of the security auditing organizations follow these Top 10 security issues to categorize security vulnerabilities.

**ISO/IEC 27037:** This ISO standard contains guidelines for the identification, collection, acquisition, and preservation of digital evidence.

**Payment Card Industry Data Security Standard (PCI DSS):** This compliance formulates financial organizations and sellers' requirements to transact credit card payments securely.

**Cloud Security Alliance (CSA):** CSA is a non-profit organization that regularly publishes the best security practices related to cloud security.

**ISO/SAE 21434:** Standard covers the aspects of automotive cybersecurity. This standard includes the list of requirements related to cyber security risk management. It also covers a cybersecurity process framework that help OEM to come on common platform and communicate risks related to security.

**ISO/IEC 20243-1:** This Information technology standard refers Open Trusted Technology ProviderTM Standard (O-TTPS). This particular standard helps in mitigating maliciously tainted and counterfeit products.


