# Botium-Toys-Security-Audit
-------------------------------------
1. [Introduction](#introduction)
2. [Scenario](#scenario)
3. [Controls Assessment](#controls-assessment)
4. [Conclusion](#conclusion)

-------------------------------------------------
# Introduction <a name="introduction">
This is a mock internal security audit for a fictional company called Botium Toys as part of my cybersecurity portfolio. 
<p><b>Goals:</b></p>
<ul>
  <li>Adhere to the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF)</li>
  <li>Establish a better process for their systems to ensure they are compliant</li>
  <li>Fortify system controls</li>
  <li>Implement the concept of least permissions when it comes to user credential management</li>
  <li>Establish their policies and procedures, which includes their playbooks</li>
  <li>Ensure they are meeting compliance requirements </li>
</ul>

<p><b>Scope:</b></p>
<ul>
  <li>The following systems are in scope: accounting, end point detection, firewalls,
intrusion detection system, SIEM tool. The systems will be evaluated for:</li>
  <ul>
    <li>Current user permissions</li>
    <li>Current implemented controls</li>
    <li>Current procedures and protocols</li>
  </ul>
  <li>Ensure current user permissions, controls, procedures, and protocols in place
align with PCI DSS and GDPR compliance requirements.</li>
  <li>Ensure current technology is accounted for both hardware and system access.</li>
</ul>

<p><b>Critical findings:</b></p>
<ul>
  <li>Multiple controls need to be developed and implemented to meet the audit
goals, including:</li>
  <ul>
    <li>Control of Least Privilege and Separation of Duties</li>
    <li>Disaster recovery plans</li>
    <li>Password, access control, and account management policies, including
the implementation of a password management system</li>
    <li>Encryption (for secure website transactions)</li>
    <li>IDS</li>
    <li>Backups</li>
    <li>AV software</li>
    <li>CCTV</li>
    <li>Locks</li>
    <li>Manual monitoring, maintenance, and intervention for legacy systems</li>
    <li>Fire detection and prevention systems</li>
  </ul>
  <li>Policies need to be developed and implemented to meet PCI DSS and GDPR
compliance requirements.</li>
  <li>Policies need to be developed and implemented to align to SOC1 and SOC2
guidance related to user access policies and overall data safety.</li>
</ul>

<p><b>Other findings:</b></p>
<ul>
  <li>The following controls should be implemented when possible:
    <ul>
      <li>Time-controlled safe</li>
      <li>Adequate lighting</li>
      <li>Locking cabinets</li>
      <li>Signage indicating alarm service provider</li>
    </ul>
  </li>
</ul>

<p><b>Summary & Recommendations</b></p>
<ul>
Botium Toys must address critical compliance issues related to PCI DSS and GDPR, as the company processes online payments from global customers, including those in the EU. Additionally, guidance from SOC 1 and SOC 2 should be leveraged to strengthen user access controls and overall data security by implementing robust policies and procedures. Establishing disaster recovery plans and maintaining backups is essential to ensure business continuity in the event of an incident. Integrating intrusion detection systems (IDS) and antivirus (AV) software into existing infrastructure will enhance risk identification and mitigation, particularly since legacy systems currently require manual monitoring and intervention. To protect physical assets at Botium Toys’ single location, measures such as locks and CCTV should be implemented for security and threat investigation. While not immediately necessary, further improvements—such as encryption, time-controlled safes, adequate lighting, locking cabinets, fire detection and prevention systems, and signage indicating alarm service providers—will strengthen the company’s overall security posture.
</ul>

------------------------------------------------------------
# Scenario <a name="scenario">
Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location, which serves as their main office, a storefront, and warehouse for their products. However, Botium Toy’s online presence has grown, attracting customers in the U.S. and abroad. As a result, their information technology (IT) department is under increasing pressure to support their online market worldwide. 

The manager of the IT department has decided that an internal IT audit needs to be conducted. She's worried about maintaining compliance and business operations as the company grows without a clear plan. She believes an internal audit can help better secure the company’s infrastructure and help them identify and mitigate potential risks, threats, or vulnerabilities to critical assets. The manager is also interested in ensuring that they comply with regulations related to internally processing and accepting online payments and conducting business in the European Union (E.U.).  

The IT manager starts by implementing the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF), establishing an audit scope and goals, listing assets currently managed by the IT department, and completing a risk assessment. The goal of the audit is to provide an overview of the risks and/or fines that the company might experience due to the current state of their security posture.

------------------------------------------------------------
# Controls Assessment <a name="controls-assessment">

<h2>Current assets</h2>
<p>Assets managed by the IT Department include:</p>
<ul>
  <li>On-premises equipment for in-office business needs </li>
  <li>Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.</li>
  <li>Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management</li>
  <li>Internet access</li>
  <li>Internal network</li>
  <li>Vendor access management</li>
  <li>Data center hosting services</li>
  <li>Data retention and storage</li>
  <li>Badge readers</li>
  <li>Legacy system maintenance: end-of-life systems that require human monitoring</li>
</ul>

<h2>Control categories</h2>
<p><b>The 3 main categories:</b></p>

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


<h2>Compliance Overview</h2>
<p><b>General Data Protection Regulation (GDPR)</b></p>
<p>GDPR is a European Union (E.U.) general data regulation that protects the
processing of E.U. citizens’ data and their right to privacy in and out of E.U.
territory. Additionally, if a breach occurs and a E.U. citizen’s data is
compromised, they must be informed within 72 hours of the incident.</p>
<p>Botium Toys must be compliant with GDPR due to handling of financial and personal information of customer in the European Union. </p>

<p><b>Payment Card Industry Data Security Standard (PCI DSS)</b></p>
<p>PCI DSS is an international security standard meant to ensure that organizations
storing, accepting, processing, and transmitting credit card information do so in
a secure environment.</p>
<p>Botium Toys must comply with PCI DSS becuse it stores, accepts, processes, and transmits credit card information on an international scale.</p>

<p><b>System and Organizations Controls (SOC type 1, SOC type 2)</b></p>
<p>The SOC1 and SOC2 are a series of reports that focus on an organization's user
access policies at different organizational levels. They are used to assess an
organization’s financial compliance and levels of risk. They also cover
confidentiality, privacy, integrity, availability, security, and overall data safety.
Control failures in these areas can lead to fraud.</p>
<p>Botium Toys needs to establish and maintain appropriate user access for internal and external (third-party vendor) personnel to mitigate risk and ensure data safey.</p>

--------------------------------------------

# Conclusion <a name="conclusion">
<p>On a scale of 1 to 10, the risk score is 8, which is fairly high. This is due to a lack of
controls and adherence to compliance best practices. Currently, there is inadequate management of assets. Additionally, Botium Toys does
not have all of the proper controls in place and may not be fully compliant with U.S. and
international regulations and standards. The potential impact from the loss of an asset is rated as medium, because the IT
department does not know which assets would be at risk. The risk to assets or fines
from governing bodies is high because Botium Toys does not have all of the necessary
controls in place and is not fully adhering to best practices related to compliance
regulations that keep critical data private/secure.</p>

