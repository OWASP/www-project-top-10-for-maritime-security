# Maritime Cybersecurity Vulnerability Database

This directory contains a structured database of cybersecurity vulnerabilities and threats specific to the maritime industry, extracted and synthesized from authoritative sources including IMO guidelines, US Coast Guard alerts, IACS recommendations, and industry reports.

## Database Structure

### Files

- **`maritime_vulnerabilities.yaml`** - Comprehensive vulnerability database with detailed categorization
- **`threat_actors.yaml`** - Known threat actors targeting maritime infrastructure
- **`incidents.yaml`** - Documented maritime cyber incidents and case studies
- **`controls.yaml`** - Security controls and mitigation strategies

## Vulnerability Categories

Based on analysis of maritime-specific threats, vulnerabilities are categorized into:

1. **Operational Technology (OT) Vulnerabilities** - ECDIS, GPS/GNSS, AIS, radar systems
2. **Information Technology (IT) Vulnerabilities** - Networks, email systems, shore connections
3. **Supply Chain Vulnerabilities** - Third-party software, vendor access, component integrity
4. **Human Factor Vulnerabilities** - Phishing, social engineering, insider threats
5. **Communication System Vulnerabilities** - VSAT, radio systems, satellite communications
6. **Port Infrastructure Vulnerabilities** - Port management systems, cargo handling systems
7. **Regulatory & Compliance Gaps** - Insufficient cybersecurity policies, audit failures

## Data Sources

All vulnerability data is extracted from authoritative sources:

- **IMO (International Maritime Organization)** - MSC-FAL.1/Circ.3/Rev.2, Resolution MSC.428(98)
- **IACS (International Association of Classification Societies)** - Unified Requirements
- **US Coast Guard** - Maritime Cyber Alerts and Bulletins
- **DNV GL** - Class Guidelines and Recommended Practices
- **IAPH** - Port Community Cyber Security Reports
- **NIST** - Special Publications on ICS/OT Security

## Methodology

Vulnerabilities are assessed using:

- **Frequency** - How often the vulnerability appears across sources and incidents
- **Impact** - Potential consequences (safety, financial, environmental, operational)
- **Exploitability** - Ease of exploitation and availability of exploit tools
- **Prevalence** - How widespread the vulnerability is across maritime assets
- **Detection Difficulty** - How hard it is to detect exploitation

## Usage

This database supports:

1. Development of the OWASP Top 10 for Maritime Security
2. Risk assessment and threat modeling for maritime organizations
3. Security awareness and training programs
4. Regulatory compliance and audit preparation
5. Research and analysis of maritime cyber threats

## Contributing

To contribute vulnerability data:

1. Ensure the vulnerability is maritime-specific or has maritime-specific implications
2. Provide credible source references
3. Follow the YAML schema structure
4. Include real-world incident examples where available
5. Submit via pull request with detailed description

## Schema

See individual YAML files for detailed schema documentation. All entries include:

- Unique identifier
- Descriptive name and title
- Category and subcategory
- Detailed description
- Impact assessment
- Affected systems
- Attack vectors
- Mitigation strategies
- Source references
- Related incidents
