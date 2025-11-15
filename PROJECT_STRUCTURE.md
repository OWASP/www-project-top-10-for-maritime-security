# OWASP Maritime Top 10 Project Structure

## Repository Overview

This document provides a comprehensive overview of the project structure, components, and organization.

## Directory Structure

```
www-project-top-10-for-maritime-security/
│
├── .github/                          # GitHub configuration
│   ├── workflows/                    # CI/CD workflows
│   └── dependabot.yml               # Dependency management
│
├── assets/                          # Web assets
│   └── images/                      # Project images and logos
│
├── data collection/                 # Source documents and research data
│   ├── IMO/                        # International Maritime Organization documents
│   ├── Public Sources/             # Industry reports and guidelines
│   ├── US Coast Guard/             # USCG alerts, bulletins, and guidance
│   └── README.md                   # Documentation of data sources
│
├── vulnerabilities/                 # Structured vulnerability database
│   ├── maritime_vulnerabilities.yaml  # Comprehensive vulnerability catalog
│   ├── threat_actors.yaml          # Threat actor profiles
│   ├── incidents.yaml              # Maritime cyber incident database
│   └── README.md                   # Database documentation
│
├── methodology/                     # Analysis methodology
│   └── METHODOLOGY.md              # Detailed methodology framework
│
├── top10/                          # OWASP Maritime Top 10 deliverables
│   └── OWASP-Maritime-Top-10-2024.md  # Published Top 10 list
│
├── CONTRIBUTING.md                  # Contribution guidelines
├── LICENSE                         # CC-BY-SA 4.0 license
├── SECURITY.md                     # Security policy
├── PROJECT_STRUCTURE.md            # This file
├── readme.md                       # Main project README
├── index.md                        # Website homepage
├── info.md                         # Project metadata
├── leaders.md                      # Project leadership
└── project.owasp.yaml              # OWASP project configuration
```

## Component Descriptions

### Core Project Files

**readme.md / index.md**
- Project overview and introduction
- Roadmap and phases
- Getting involved information
- License and attribution

**project.owasp.yaml**
- OWASP Foundation metadata
- Project classification and tags
- Leadership information

**CONTRIBUTING.md**
- How to contribute to the project
- Branching model (master/develop)
- Submission guidelines
- Code of conduct

### Data Collection (`data collection/`)

**Purpose:** Repository of authoritative source documents

**Contents:**
- 34 PDF documents from regulatory bodies, threat intelligence, industry reports
- Organized by source (IMO, USCG, Public Sources)
- Forms evidentiary basis for vulnerability analysis

**Key Documents:**
- IMO MSC-FAL.1/Circ.3/Rev.2 (Maritime Cyber Risk Management Guidelines)
- IACS Rec. 166 (Cyber Resilience Requirements)
- USCG Maritime Cyber Alerts (Current threat intelligence)
- NIST SP 800-82r3 (ICS Security Guide)

**Documentation:** `data collection/README.md` provides detailed catalog

### Vulnerability Database (`vulnerabilities/`)

**Purpose:** Structured, machine-readable vulnerability database

**Schema:** YAML format for easy parsing and version control

**Files:**

1. **maritime_vulnerabilities.yaml** (12 vulnerabilities)
   - Unique ID (MAR-001 through MAR-012)
   - Category, severity, CVSS score
   - Detailed descriptions
   - Affected systems and attack vectors
   - Impact analysis (safety, operational, financial)
   - Mitigation strategies
   - Real-world incidents and references
   - CWE mappings

2. **threat_actors.yaml** (8 threat actors)
   - State-sponsored APTs (Volt Typhoon, Sandworm, etc.)
   - Cybercriminal groups (BlackBasta, CL0P, etc.)
   - Attribution, motivation, sophistication
   - Tactics, tools, and maritime incidents
   - Detection indicators

3. **incidents.yaml** (12 documented incidents)
   - Real-world maritime cyber incidents (2011-2024)
   - Maersk NotPetya, Port ransomware, GPS spoofing campaigns
   - Impact analysis and lessons learned
   - Recovery timelines and costs

**Usage:**
- Input for analysis tools
- Reference for maritime security professionals
- Training and awareness material
- Research data for academic studies

### Methodology (`methodology/`)

**METHODOLOGY.md**
- Comprehensive analysis framework
- Risk scoring calculation: `Risk = f(Frequency, Impact, Exploitability, Prevalence, Detection)`
- Weighting rationale (Impact 35%, Frequency 25%, etc.)
- Vulnerability categorization taxonomy
- Top 10 selection criteria
- Validation and review process
- Alignment with OWASP methodology
- Data quality and limitations

**Purpose:**
- Transparency in analysis
- Repeatability and peer review
- Adaptation by other sectors
- Academic rigor

### Top 10 List (`top10/`)

**OWASP-Maritime-Top-10-2025.md**

The primary deliverable: Maritime-specific Top 10 cybersecurity risks

**Contents:**
1. Ransomware and Destructive Malware (9.2/10)
2. GNSS/GPS Manipulation and Jamming (9.1/10)
3. Phishing and Social Engineering (8.1/10)
4. Insecure Remote Access (9.4/10)
5. Unpatched and Legacy Systems (8.4/10)
6. Insufficient Network Segmentation (8.2/10)
7. ECDIS and Navigation System Compromise (8.8/10)
8. AIS Spoofing and Manipulation (7.5/10)
9. Supply Chain Compromise (8.6/10)
10. Insufficient Cybersecurity Awareness (7.6/10)

**Each entry includes:**
- Risk description and score
- Why it's critical for maritime
- Affected systems
- Real-world examples
- Mitigation strategies
- Regulatory references

**Format:** Markdown for web publishing and PDF generation

## Project Phases

### Phase 1: Data Collection (COMPLETED)
- ✅ Gathered 34 authoritative source documents
- ✅ Organized by source type
- ✅ Documented in README

### Phase 2: Analysis and Top 10 Development (CURRENT)
- ✅ Extracted vulnerabilities from sources
- ✅ Created structured database (12 vulnerabilities)
- ✅ Developed analysis methodology
- ✅ Calculated risk scores
- ✅ Generated preliminary Top 10 list
- ✅ Built analysis tools

### Phase 3: Validation and Publication (NEXT)
- ⏳ Community review and feedback
- ⏳ Expert validation
- ⏳ Regulatory stakeholder consultation
- ⏳ Final publication
- ⏳ Dissemination and outreach

## Data Flow

```
Source Documents (data collection/)
        ↓
Manual Extraction & Synthesis
        ↓
Structured Database (vulnerabilities/*.yaml)
        ↓
Analysis Tools (analysis-tools/)
        ↓
Risk Scores & Rankings
        ↓
Top 10 List (top10/OWASP-Maritime-Top-10-2024.md)
        ↓
Publication & Dissemination
```

## Technology Stack

**Data Formats:**
- YAML: Structured data (vulnerabilities, incidents)
- Markdown: Documentation and deliverables
- PDF: Source documents
- CSV/JSON: Export formats

**Tools:**
- Python 3.7+: Analysis and automation
- Git: Version control
- GitHub: Collaboration and hosting
- Jekyll: Static site generation (OWASP theme)

**Standards:**
- CVSS 3.1: Vulnerability scoring
- CWE: Weakness enumeration
- MITRE ATT&CK: Tactics and techniques (future)

## Contribution Points

Areas where contributions are welcome:

1. **Data Collection**
   - Additional source documents
   - Incident reports
   - Threat intelligence

2. **Vulnerability Database**
   - New maritime-specific vulnerabilities
   - Additional real-world examples
   - Mitigation strategy refinements

3. **Analysis Tools**
   - Visualization features
   - Trend analysis
   - MITRE ATT&CK mapping

4. **Documentation**
   - Case studies
   - Implementation guides
   - Training materials

5. **Validation**
   - Expert review
   - Real-world testing
   - Feedback from maritime operators

See CONTRIBUTING.md for submission guidelines.

## Maintenance and Updates

**Update Cycle:** Annual with quarterly threat intelligence updates

**Version Control:**
- Semantic versioning for Top 10 list
- Date-based versioning for databases
- Git tags for releases

**Review Process:**
- Annual full data review (next: Q4 2026)
- Quarterly threat intelligence updates
- Continuous vulnerability addition
- Community feedback integration

## Contact and Support

**Project Leadership:**
- Faiz Ahmed Zaidi - Project Leader
- Manish Tripathy - Contributor

**Communication Channels:**
- GitHub Issues: Technical discussions, bug reports
- GitHub Discussions: General questions, ideas
- OWASP Slack: Real-time community chat
- Mailing List: Announcements and updates

**Resources:**
- Project Website: https://owasp.org/www-project-top-10-for-maritime-security/
- GitHub Repository: https://github.com/OWASP/www-project-top-10-for-maritime-security
- OWASP Project Page: Links and resources

---

**Document Version:** 1.1  
**Last Updated:** November 2025  
**Maintained By:** Project contributors
