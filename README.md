# Botium-Toys-Security-Audit-Writeup

# Table of contents

1. [Introduction](#introduction)
2. [Scenario](#scenario)
3. [Internal Security Audit Workflow](#workflow)
4. [Controls Assessment](#control-assessment)
5. [Compliance Checklist](#compliance-checklist)
6. [Stakeholder Memorandum](#stakeholder-memo)
7. [Conclusion](#conclusion)

-------

# Introduction <a name="introduction">

An internal security audit assessment done on Botium Toys, a fictitious toy company, completed as part of my cybersecurity portfolio and as part of Google's <a href='https://www.coursera.org/google-certificates/cybersecurity-certificate'>Cybersecurity Professional Certificate</a> on Coursera in the  <a href='https://www.coursera.org/learn/manage-security-risks?specialization=cybersecurity-certificate'> Play It Safe: Manage Security Risks </a> Course .
   
The goal is to perform an audit of Botium Toys’ cybersecurity program. The audit needs
to align current business practices with industry standards and best practices. The
audit is meant to provide mitigation recommendations for vulnerabilities found that are
classified as “high risk,” and present an overall strategy for improving the security
posture of the organization. The audit team needs to document their findings, provide
remediation plans and efforts, and communicate with stakeholders.

# Scenario  <a name="scenario">
Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location. However, its online presence has grown, attracting customers in the U.S. and abroad. Their information technology (IT) department is under increasing pressure to support their online market worldwide. 

The manager of the IT department has decided that an internal IT audit needs to be conducted. She expresses concerns about not having a solidified plan of action to ensure business continuity and compliance, as the business grows. She believes an internal audit can help better secure the company’s infrastructure and help them identify and mitigate potential risks, threats, or vulnerabilities to critical assets. The manager is also interested in ensuring that they comply with regulations related to accepting online payments and conducting business in the European Union (E.U.).   

The IT manager starts by implementing the **National Institute of Standards and Technology Cybersecurity Framework** (NIST CSF), establishing an audit scope and goals, and completing a risk assessment. The goal of the audit is to provide an overview of the risks the company might experience due to the current state of their security posture. The IT manager wants to use the audit findings as evidence to obtain approval to expand his department.

------------------------


The goals for Botium Toys’ internal IT audit are:
- To adhere to the National Institute of Standards and Technology Cybersecurity
Framework (NIST CSF)
- Establish a better process for their systems to ensure they are compliant
- Fortify system controls
- Implement the concept of least permissions when it comes to user credential
management
- Establish their policies and procedures, which includes their playbooks
- Ensure they are meeting compliance requirements

   
## Internal Security Audit Workflow  <a name="workflow">
The internal security audit can be broken down into two parts each with their own steps to follow.

### Part 1
1. Analyze the audit scope, audit goals, and risk assessment
2. Conduct the Audit
   - Complete Controls assessment 
     - Select controls needing to be implemented.
     - Rate each selected control on prioirty (i.e. needing to be implemented immediately or in the future).
   - Complete Compliance checklist
     - Explain why selected compliance regulations and standards need to be adhered to.
### Part 2
1. Review results and deliverables completed in Part 1, Step #2
   - make note of findings
   - consider how to summarize your recommendations clearly and concisely to stakeholders. 
2. Send findings and recommendations to stakeholders in a concise format


Controls Assessment  <a name="control-assessment">
===================


Current Assets 
--------------

Assets managed by the IT Department include:

- On-premises equipment for in-office business needs 

- Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.

- Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management

- Internet access

- Internal network

- Vendor access management

- Data center hosting services 

- Data retention and storage

- Badge readers

- Legacy system maintenance: end-of-life systems that require human monitoring

### Administrative Controls 
| Control Name | Control type and explanation | Needs to be implemented (X) | Priority |
| --- | --- | --- | --- |
| Least Privilege | Preventative; reduces risk by making sure vendors and non-authorized staff only have access to the assets/data they need to do their jobs | X | High |
| Disaster recovery plans | Corrective; business continuity to ensure systems are able to run in the event of an incident/there is limited to no loss of productivity downtime/impact to system components, including: computer room environment (air conditioning, power supply, etc.); hardware (servers, employee equipment); connectivity (internal network, wireless); applications (email, electronic data); data and restoration | X | High |
| Password policies | Preventative; establish password strength rules to improve security/reduce likelihood of account compromise through brute force or dictionary attack techniques | X | High |
| Access control policies | Preventative; increase confidentiality and integrity of data | X | High |
| Account management policies | Preventative; reduce attack surface and limit overall impact from disgruntled/former employees | X | High |
| Separation of duties | Preventative; ensure no one has so much access that they can abuse the system for personal gain | X | High |

### Technical Controls 
| Control Name | Control type and explanation | Needs to be implemented (X) | Priority |
| --- | --- | --- | --- |
| Firewall | Preventative; firewalls ***are already in place*** to filter unwanted/malicious traffic from entering internal network | NA | NA |
| Intrusion Detection System (IDS) | Detective; allows IT team to identify possible intrusions (e.g., anomalous traffic) quickly | X | High |
| Encryption | Deterrent; makes confidential information/data more secure (e.g., website payment transactions) | X | High |
| Backups | Corrective; supports ongoing productivity in the case of an event; aligns to the disaster recovery plan | X | High |
| Password management system | Corrective; password recovery, reset, lock out notifications | X | High |
| Antivirus (AV) software | Corrective; detect and quarantine known threats | X | High |
| Manual monitoring, maintenance, and intervention | Preventative/corrective; required for legacy systems to identify and mitigate potential threats, risks, and vulnerabilities | X | High |


### Physical Controls
| Control Name | Control type and explanation | Needs to be implemented (X) | Priority |
| --- | --- | --- | --- |
| Time-controlled safe | Deterrent; reduce attack surface/impact of physical threats | X | Medium/Low |
| Adequate lighting | Deterrent; limit “hiding” places to deter threats | X | Medium/Low |
| Closed-circuit television (CCTV) surveillance | Preventative/detective; can reduce risk of certain events; can be used after event for investigation | X | High/Medium |
| Locking cabinets (for network gear) | Preventative; increase integrity by preventing unauthorized personnel/individuals from physically accessing/modifying network infrastructure gear | X | High/Medium |
| Signage indicating alarm service provider | Deterrent; makes the likelihood of a successful attack seem low | X | Low |
| Locks | Preventative; physical and digital assets are more secure | X | High |
| Fire detection and prevention (fire alarm, sprinkler system, etc.) | Detective/Preventative; detect fire in the toy store’s physical location to prevent damage to inventory, servers, etc. | X | Medium |

Compliance checklist
====================

To review compliance regulations and standards, read the [controls, frameworks, and compliance](https://www.coursera.org/learn/foundations-of-cybersecurity/supplement/xu4pr/controls-frameworks-and-compliance) document.
   
I found that Botium Toys will need to adhere to the following standards:
     
General Data Protection Regulation (GDPR)
  -  GDPR is a European Union (E.U.) general data regulation that protects the processing of E.U. citizens' data and their right to privacy in and out of E.U. territory. Additionally, if a breach occurs and a E.U. citizen's data is compromised, they must be informed within 72 hours of the incident.
      -  Botium Toys is expanding to offer services and handle the data of customers abroad, GDPR compliance is in scope for the handling of financial and personal information for customers in the European Union.
   

  Payment Card Industry Data Security Standard (PCI DSS)
  -  PCI DSS is an international security standard meant to ensure that organizations storing, accepting, processing, and transmitting credit card information do so in a secure environment. 

       - Botium Toys must adhere to PCI DSS as it accepts payments online and person and They also store and processes customer credit card on an international scale. It's requirements and compliance need to be taken seriously based on possible consequences. The consequences of not complying with this standard is more severe in impact: Monetary fines monthly (ranging from 5,000-100,000 USD), costs of forensic audits upon a data breach, payment brand restrictions, damage to brand reputation, and possibility of lawsuit costs in the event of data breaches. 


  System and Organizations Controls (SOC type 1, SOC type 2)
   - The SOC1 and SOC2 are a series of reports that focus on an organization's user access policies at different organizational levels. They are used to assess an organization's financial compliance and levels of risk. They also cover confidentiality, privacy, integrity, availability, security, and overall data safety. Control failures in these areas can lead to fraud.

      - Botium Toys needs to establish and maintain appropriate user access for internal and external (third-party vendor) personnel to mitigate risk and ensure data safey.
      - Both of these standards evaluate the effectiveness of a company's internal controls. While SOC1 I focused on financial reporting controls, SOC2 is concerned with information security controls, including customer data safety. 
----------------
   

# Stakeholder memorandum <a name="stakeholder-memo">

To: IT Manager, Stakeholders

From: Joshua Constantin

Date: August 4, 2024

Subject: Internal Security Audit Findings and Recommendations

Introduction:

The internal IT audit conducted for Botium Toys has yielded critical insights into the current security posture and compliance status of the organization. This memorandum outlines the scope, objectives, key findings, and actionable recommendations aimed at enhancing the company’s cybersecurity framework.

Scope of the Audit:

The audit focused on the following systems and controls:

  Systems Reviewed: Accounting, endpoint detection, firewalls, intrusion detection systems (IDS), and security information and event management (SIEM) tools.
  Areas of Evaluation: User permissions, implemented security controls, and adherence to regulatory compliance requirements including GDPR, PCI DSS, and SOC standards.
  Asset Inventory: Comprehensive review of technology and hardware assets, including both physical and digital resources.

Audit Objectives:

  Align security practices with the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF).
  Strengthen processes to ensure regulatory compliance.
  Enhance system controls to mitigate identified risks.
  Implement least privilege access controls and develop robust policies and procedures.

Key Findings

  - Critical Control Gaps:
        Least Privilege & Separation of Duties: Current practices do not fully enforce the principle of least privilege and separation of duties, increasing the risk of unauthorized access and potential abuse.
        Disaster Recovery Plans: Lack of comprehensive disaster recovery plans could lead to significant downtime and loss of data in the event of a system failure or incident.
        Password & Access Control Policies: Existing policies are inadequate, exposing the organization to potential security breaches and unauthorized access.
        Intrusion Detection System (IDS) & Encryption: Absence of a fully implemented IDS and encryption mechanisms for sensitive data could hinder the ability to detect and respond to intrusions effectively.
        Backup & Antivirus Solutions: Current backup solutions and antivirus software need enhancement to ensure data integrity and protection against malware.

  - Physical Security Enhancements Needed:
        CCTV & Locks: Inadequate physical security measures such as CCTV coverage and locking mechanisms for network gear require immediate attention to prevent unauthorized physical access.

Recommendations

  - Immediate Action Items:
        We’ve identified several key issues in our current security setup. First, we’re not fully applying the principles of least privilege and separation of duties, which means there’s a higher risk of unauthorized access and misuse. Also, our disaster recovery plans are lacking, leaving us vulnerable to significant downtime and data loss if something goes wrong. Our password and access control policies aren’t strong enough, putting us at risk of security breaches. We also don’t have a fully implemented Intrusion Detection System (IDS) or proper encryption for sensitive data, which limits our ability to spot and respond to threats. Lastly, our backup solutions and antivirus software need to be upgraded to better protect against data loss and malware.

  - Physical Security Improvements:
        Install CCTV & Enhance Locking Mechanisms: Upgrade physical security measures by installing CCTV cameras and enhancing locking mechanisms for critical infrastructure.
        Consider Additional Controls: Implement time-controlled safes, adequate lighting, and signage indicating alarm service providers to further bolster physical security.

# Conclusion <a name="conclusion">

The findings of this audit highlight several critical areas requiring immediate attention to strengthen Botium Toys’ security posture and compliance. Implementing the recommendations will not only address the current vulnerabilities but also enhance the overall resilience of the organization against potential threats.

I recommend prioritizing the control gaps and physical security enhancements to align with industry standards and ensure robust protection for the organization’s assets and data.

This would complete my mock security audit writeup. I hope you find it helpful! If you have any feedback or suggestions, please let me know.

Self-Evaluation: I’m confident I identified the key controls and compliance needs for Botium Toys. The assignment was a great way to apply what I've learned.

Lessons Learned:

I struggled with providing detailed findings in the stakeholder memo. I worked hard to be clearer and more concise, using lists and proofreading my work.

I also had difficulty explaining how the System and Organizations Controls standard impacts user access and overall data safety, beyond just financial aspects.
