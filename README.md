# Threat Modeling Project

## Project Title: Threat Modeling for BigMart’s Digital Strategy

## Objective:
To ensure the security and resilience of BigMart’s new online web store by identifying, analyzing, and mitigating potential threats. The goal is to provide a secure, uninterrupted, and enhanced user experience to BigMart’s customers.

## Tools and Methodologies Used:

- Threat Modeling: STRIDE, OWASP Top 10
- Threat Rating: DREAD model
- Security Solutions: SSL/TLS, firewalls, WAF, IDS, VPN
- Programming: Python
- Database: Oracle/Microsoft SQL Server
- Web Server: Nginx

## Key Responsibilities:

1. ### Identify Business and Security Objectives:

- Business Objectives: Secure #1 market leader position in daily groceries and home requirements by adopting a digital strategy, enhancing customer experience, and ensuring continuous service availability.
- Security Objectives: Protect customer data, ensure secure transactions, prevent unauthorized access, and ensure the integrity and availability of the web store.
2. ### Phase 1: Identify Assets:

- Assets: Customer data (personal information, order details), payment information, web store application, backend database, sales team access, administrator access.
- Actors: Customers, sales team, administrators, third-party payment processors, threat actors.
- Data Elements: User credentials, order details, payment information.
- Technologies: Python (programming language), Oracle/Microsoft SQL Server (database), Nginx (webserver).
- External Dependencies: Third-party payment processor, third-party backup location.
3. ### Phase 2: Create Architecture Overview:

- #### Physical Network Topology:
  - Use a firewall for boundary protection.
  - Use a web application firewall (WAF) to protect the application.
  - Use an Intrusion Detection System (IDS) to monitor for malicious traffic.
  - Application server placed in the DMZ (Demilitarized Zone).
  - Database server placed in the internal network.
4. ### Phase 3: Decompose Architecture:

- #### Logical Topology:
  - Customers access the web store via SSL/TLS.
  - Trust boundaries between the web server and application server, and between the application server and database.
  - Secure VPN connection between components.
5. ### Phase 4: Identify Threats:

- #### Applied the STRIDE model to identify threats:
  - Spoofing: Unauthorized users gain access to the system by impersonating legitimate users.
  - Tampering: Unauthorized alteration of data during transmission or storage.
  - Repudiation: Users deny actions they performed, leading to a lack of accountability.
  - Information Disclosure: Exposure of sensitive information to unauthorized users.
  - Denial of Service (DoS): Overloading the system to make it unavailable to legitimate users.
  - Elevation of Privilege: Unauthorized users gaining higher access levels.
6. ### Phase 5: Document Threats:

  - #### Created a threat template for identified threats:
    - Threat Description: Spoofing of user credentials.
    - Threat Target: User authentication system.
    - Attack Techniques: Phishing attacks to steal user credentials.
    - Controls/Countermeasures: Implement multi-factor authentication (MFA), user education on phishing, and use of CAPTCHA to prevent automated attacks.
    - Threat Description: SQL injection attacks on the database.
    - Threat Target: Backend database.
    - Attack Techniques: Injection of malicious SQL queries via input fields.
    - Controls/Countermeasures: Use parameterized queries, input validation, and regular security audits.

7. ### Phase 6: Rate Threats:

- #### Applied the DREAD model to rate each threat:
  - Threat: Spoofing of user credentials

     - Damage Potential (D): 3
     - Reproducibility (R): 3
     - Exploitability (E): 3
     - Affected Users (A): 3
     - Discoverability (D): 3
     - Total Rating: 15 (High)
- #### Threat: SQL injection attacks on the database

  - Damage Potential (D): 3
  - Reproducibility (R): 3
  - Exploitability (E): 2
  - Affected Users (A): 3
  - Discoverability (D): 2
  - Total Rating: 13 (High)
    
- ### Solutions and Recommendations:

- Multi-Factor Authentication (MFA):

  - Implement MFA to add a layer of security to the authentication process, reducing the risk of spoofing attacks.
User Education:
  - Conduct regular training sessions to educate users about phishing attacks and safe online practices.

- CAPTCHA Implementation:

  - Use CAPTCHA on login and registration pages to prevent automated attacks.
- Parameterized Queries and Input Validation:

  - Implement parameterized queries and robust input validation to prevent SQL injection attacks.
- Regular Security Audits:

  - Conduct regular security audits and penetration testing to identify and mitigate vulnerabilities.
- Incident Response Plan:

  - Develop and implement a comprehensive incident response plan to quickly detect, respond to, and recover from security incidents.
    
## Achievements:

Enhanced Security Posture: Significantly improved the security of BigMart’s web store, reducing the risk of spoofing and SQL injection attacks.
Increased User Trust: By implementing MFA and educating users, increased trust and confidence among customers in using the online platform.
Compliance and Risk Mitigation: Ensured compliance with industry standards and best practices, effectively mitigating potential risks.

## Conclusion:
The Threat Modeling project for BigMart’s digital strategy successfully identified and mitigated potential threats to the web store. By applying industry-standard methodologies and implementing robust security measures, the project ensured a secure, uninterrupted, and enhanced user experience for BigMart’s customers, contributing to the organization’s goal of becoming the market leader in daily groceries and home requirements.

