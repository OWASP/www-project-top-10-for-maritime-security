# Maritime Cybersecurity Data Collection

This directory contains authoritative source documents on maritime cybersecurity, including regulatory guidelines, industry standards, threat intelligence, incident reports, and technical guidance. These materials form the evidentiary basis for the OWASP Top 10 for Maritime Security.

## Collection Overview

**Total Documents:** 34 source documents  
**Document Types:** PDFs (regulations, guidelines, reports, threat intelligence, incident analyses)  
**Date Range:** 2017-2024  
**Geographic Coverage:** Global (IMO, US, EU perspectives)  

## Directory Structure

```
data collection/
├── IMO/                    # International Maritime Organization documents
├── Public Sources/         # Publicly available industry reports and guidelines
├── US Coast Guard/         # USCG Maritime Cyber Alerts, Bulletins, and guidance
├── DNV GL.pdf             # Classification society guidelines
└── IAPH-Port-Community-Cyber-Security-Report-Q2-2020.pdf
```

## Document Categories

### 1. International Regulatory Framework (IMO/)

**International Maritime Organization (IMO)** - UN specialized agency responsible for maritime safety and security regulations.

#### Key Documents:

**MSC-FAL.1/Circ.3/Rev.2 - Guidelines On Maritime Cyber Risk Management (Secretariat).pdf**
- **Date:** 2021
- **Type:** Regulatory Guidance
- **Scope:** Global maritime industry
- **Key Content:**
  - Cyber risk management framework for ships
  - Integration with ISM Code and SMS
  - Risk assessment methodology
  - Functional elements at risk (navigation, cargo handling, propulsion, etc.)
  - Cyber incident response procedures
- **Importance:** Primary international guidance for maritime cyber risk management

**Resolution MSC.428(98).pdf**
- **Date:** June 2017
- **Type:** Resolution
- **Scope:** Mandatory for SOLAS vessels
- **Key Content:**
  - Mandates cyber risk management in Safety Management Systems (SMS)
  - Effective from first annual verification of company DOC after January 1, 2021
  - Links cyber risk to ship safety under ISM Code
- **Importance:** Made maritime cybersecurity mandatory for international shipping

**ANNEX Guidelines on Cyber Security Onboard Ships v.4.pdf**
- **Date:** Version 4 (Latest)
- **Type:** Technical Guidelines
- **Key Content:**
  - Detailed technical guidance for ship cyber security
  - System-specific vulnerabilities and controls
  - Bridge systems, machinery, cargo handling
  - Network architecture and segmentation
  - Crew training requirements
- **Importance:** Practical implementation guidance for shipboard systems

### 2. Classification Society Standards (IMO/ and Public Sources/)

**IACS Recommendation 166 (rec-166-corr2-apr-2022-ul.pdf and rec166corr2.pdf)**
- **Organization:** International Association of Classification Societies
- **Date:** April 2022 (Corrected version)
- **Type:** Unified Requirement
- **Key Content:**
  - Cyber resilience requirements for ships
  - Applies to new vessels and major conversions
  - Network segmentation requirements
  - Remote access security controls
  - Software maintenance and patching
  - Incident response capabilities
- **Importance:** Enforceable technical standards for classed vessels
- **Effective:** Ships contracted on/after July 1, 2024

### 3. Industry Best Practices (Public Sources/)

**DNV GL.pdf**
- **Organization:** DNV GL (now DNV) - Leading classification society
- **Type:** Class Guideline (DNVGL-CG-0264 - Cyber Security Resilience Management)
- **Key Content:**
  - Cyber security framework for vessels
  - Assessment methodology
  - Security levels and implementation
  - Controls catalog
  - Certification process
- **Importance:** Widely adopted voluntary standard

**IAPH-Port-Community-Cyber-Security-Report-Q2-2020.pdf**
- **Organization:** International Association of Ports and Harbors
- **Date:** Q2 2020
- **Type:** Industry Report
- **Key Content:**
  - Port cybersecurity threat landscape
  - Survey of port cyber incidents
  - Best practices for port facilities
  - Public-private partnerships
  - Critical infrastructure protection
- **Importance:** Port-side perspective on maritime cyber security

### 4. US Government Guidance and Threat Intelligence (US Coast Guard/)

#### Maritime Cyber Alerts

**Maritime Cyber Alert 01-23 VOLT TYPHOON TLP CLEAR.pdf**
- **Date:** 2023
- **Threat:** Volt Typhoon (PRC state-sponsored APT)
- **Key Content:**
  - Living-off-the-land techniques targeting US critical infrastructure
  - Maritime sector as target
  - Detection indicators
  - Mitigation recommendations
- **References:** CISA CSA on Volt Typhoon

**Maritime Cyber Alert 02-23 BLACKBASTA TLP CLEAR.pdf**
- **Date:** 2023
- **Threat:** BlackBasta ransomware group
- **Key Content:**
  - BlackBasta ransomware TTPs
  - Maritime sector targeting
  - Indicators of compromise (IOCs)
  - Prevention and response guidance
- **Importance:** Real-world threat affecting shipping companies

**Maritime Cyber Alert 03-23 TLP CLEAR.pdf**
- **Date:** 2023
- **Type:** Threat Advisory
- **Content:** Current threat intelligence for maritime sector

#### Maritime Cyber Bulletins

**Maritime Cyber Bulletin 01-23.pdf**
- **Date:** 2023
- **Type:** Periodic Security Bulletin
- **Content:** Quarterly threat summary, trends, and recommendations

**Maritime Cyber Bulletin 02-23 TLP-CLEAR.pdf**
- **Date:** 2023
- **Type:** Periodic Security Bulletin
- **Content:** Updated threat landscape and defensive measures

#### Ransomware and Threat Intelligence

**#StopRansomware_ CL0P Ransomware Gang Exploits CVE-2023-34362 MOVEit Vulnerability _ CISA.pdf**
- **Date:** 2023
- **Threat:** CL0P ransomware gang
- **Vulnerability:** CVE-2023-34362 (MOVEit Transfer)
- **Key Content:**
  - Mass exploitation campaign details
  - Affected organizations (including maritime)
  - Detection and mitigation
  - Indicators of compromise
- **Impact:** Global supply chain impact including maritime organizations

**aa23-158a-stopransomware-cl0p-ransomware-gang-exploits-moveit-vulnerability_8.pdf**
- **Source:** CISA Alert AA23-158A
- **Content:** Detailed technical analysis of CL0P/MOVEit campaign

**Ransomware.pdf**
- **Type:** General Guidance
- **Content:** Ransomware prevention, detection, and response for maritime

**Cost of a Data Breach Report 2024.pdf**
- **Source:** IBM/Ponemon Institute
- **Content:** 
  - Financial impact of data breaches
  - Industry-specific analysis
  - Maritime sector relevant findings
  - Cost factors and mitigation ROI

#### Advanced Persistent Threats

**CSA_PRC_State_Sponsored_Cyber_Living_off_the_Land_v1.1.pdf**
- **Source:** CISA Cybersecurity Advisory
- **Threat:** PRC state-sponsored cyber actors
- **Key Content:**
  - Living-off-the-land (LotL) techniques
  - Critical infrastructure targeting including maritime
  - Detection strategies
  - Hardening guidance
- **Importance:** Nation-state threat to maritime critical infrastructure

**Volt Typhoon targets US critical infrastructure with living-off-the-land techniques _ Microsoft Security Blog.pdf**
- **Source:** Microsoft Threat Intelligence
- **Content:** Detailed analysis of Volt Typhoon campaign
- **Technical Details:** TTPs, indicators, timeline

#### Phishing and Authentication

**Phishing Guidance - Stopping the Attack Cycle at Phase One_508c.pdf**
- **Source:** CISA
- **Content:**
  - Phishing attack lifecycle
  - Prevention strategies
  - Technical controls
  - User awareness training
- **Relevance:** Phishing is primary initial access vector in maritime

**fact-sheet-implementing-phishing-resistant-mfa-508c.pdf**
- **Source:** CISA
- **Content:**
  - Multi-factor authentication (MFA) implementation
  - Phishing-resistant MFA methods
  - Deployment guidance
- **Importance:** Critical control for maritime remote access

#### Technical Standards and Frameworks

**NIST.SP.800-63b.pdf**
- **Title:** Digital Identity Guidelines - Authentication and Lifecycle Management
- **Source:** National Institute of Standards and Technology
- **Content:**
  - Authentication assurance levels
  - Credential types and management
  - MFA requirements
- **Application:** Maritime user authentication systems

**NIST.SP.800-82r3.pdf**
- **Title:** Guide to Industrial Control Systems (ICS) Security
- **Source:** NIST
- **Date:** Revision 3
- **Content:**
  - ICS/SCADA security fundamentals
  - Maritime OT systems applicability
  - Network segmentation
  - Risk management for OT
  - Incident response for ICS
- **Importance:** Foundational guidance for maritime OT security (vessels, ports)

#### Policy and Strategy

**National-Cybersecurity-Strategy-2023.pdf**
- **Source:** White House
- **Date:** March 2023
- **Content:**
  - US national cybersecurity strategy
  - Critical infrastructure pillars including transportation/maritime
  - Public-private partnerships
  - International cooperation
- **Relevance:** Policy context for maritime cybersecurity priorities

**USCG MARITIME COMMERCE STRATEGIC OUTLOOK-RELEASABLE.pdf**
- **Source:** US Coast Guard
- **Content:**
  - USCG strategic priorities
  - Maritime domain awareness
  - Cybersecurity as enabler and risk
  - Port and vessel security

#### Conferences and Research

**CTIME_2023_FINAL.pdf**
- **Event:** Cyber Technologies in Maritime Environments (CTIME) Conference
- **Date:** 2023
- **Content:**
  - Conference proceedings
  - Technical papers on maritime cyber
  - Research findings
  - Industry case studies

**230404_Fagan_Beyond_USCoastline.pdf**
- **Type:** Research/Presentation
- **Content:** Maritime cyber threats beyond US coastline

## Data Usage

These documents are used for:

1. **Vulnerability Identification:** Extracting known vulnerabilities from guidelines and incident reports
2. **Threat Intelligence:** Understanding threat actors, TTPs, and targeting of maritime sector
3. **Risk Assessment:** Informing frequency, impact, and prevalence metrics
4. **Mitigation Development:** Extracting best practices and controls
5. **Regulatory Alignment:** Ensuring OWASP Top 10 aligns with IMO and industry standards
6. **Incident Analysis:** Learning from real-world maritime cyber incidents

## Analysis Methodology

See `../methodology/METHODOLOGY.md` for details on how these sources are analyzed and synthesized into the OWASP Top 10 for Maritime Security.

## Source Credibility

All sources are from authoritative organizations:

- **IMO:** UN agency, international maritime regulatory authority
- **IACS:** Classification societies representing 90% of world fleet
- **USCG:** US maritime regulatory and enforcement authority
- **CISA:** US critical infrastructure cybersecurity lead agency
- **NIST:** US standards and technology institute
- **DNV/DNV GL:** Leading classification society
- **IAPH:** International port association
- **Microsoft/IBM:** Industry threat intelligence and research

## Contribution Guidelines

To contribute additional source documents:

1. **Ensure authoritative source:** Government, international organization, recognized industry body
2. **Maritime relevance:** Document must have maritime-specific content
3. **Public availability:** Must be publicly releasable (no classified or proprietary)
4. **Proper categorization:** Place in appropriate subfolder
5. **Update this README:** Add document description

### Submitting Documents

- Create pull request with document and README update
- Include source URL and download date
- Verify document is not already in collection
- Confirm licensing allows redistribution

## Document Licensing

- **IMO documents:** © IMO, used for research and non-commercial purposes
- **US Government documents:** Public domain
- **Industry reports:** Check individual document copyright

All documents used in accordance with fair use for cybersecurity research and education.

## Future Data Collection

Areas for expansion:

- European Maritime Safety Agency (EMSA) cybersecurity guidelines
- Additional classification society standards (LR, ABS, BV)
- Port-specific incident reports
- Maritime OEM security advisories
- Academic research on maritime cyber
- International case law on cyber incidents
- Insurance industry maritime cyber reports

## Questions and Contact

For questions about the data collection:
- Submit issue on GitHub
- Contact project leaders via OWASP page

---

**Last Updated:** November 2025  
**Collection Status:** Active - Ongoing data collection  
**Next Review:** Quarterly updates with new threat intelligence and guidance
