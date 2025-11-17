# Botium-Toys-Security-Audit
-------------------------------------
1. [Introduction](#introduction)
2. [Scenario](#scenario)
3. [Controls Assessment](#controls-assessment)


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

