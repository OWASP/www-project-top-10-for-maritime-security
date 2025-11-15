# Maritime Cybersecurity Analysis Tools

This directory contains Python tools for analyzing maritime cybersecurity vulnerabilities, generating risk scores, and producing reports to support the OWASP Top 10 for Maritime Security project.

## Tools

### vulnerability_analyzer.py

Analyzes the maritime vulnerability database and generates risk scores, rankings, and reports based on the project methodology.

**Features:**
- Calculates risk scores using the OWASP Maritime methodology
- Ranks vulnerabilities by risk level
- Generates comprehensive analysis reports
- Exports data to CSV and JSON formats
- Analyzes threat actors and incidents
- Provides category and severity breakdowns

**Usage:**

```bash
# Install dependencies
pip install -r requirements.txt

# Generate analysis report
python vulnerability_analyzer.py --report

# Analyze and display results
python vulnerability_analyzer.py --analyze

# Export to CSV
python vulnerability_analyzer.py --export-csv results.csv

# Export to JSON
python vulnerability_analyzer.py --export-json results.json

# Specify custom data path
python vulnerability_analyzer.py --report --data-path /path/to/vulnerabilities
```

**Output Example:**

```
================================================================================
OWASP MARITIME CYBERSECURITY VULNERABILITY ANALYSIS REPORT
================================================================================
Generated: 2025-11-02 17:30:00
Total Vulnerabilities Analyzed: 12
Total Threat Actors: 8
Total Incidents: 12

TOP 10 VULNERABILITIES BY RISK SCORE
--------------------------------------------------------------------------------
Rank   ID         Risk   CVSS   Name
--------------------------------------------------------------------------------
1      MAR-007    9.40   9.4    Insecure Remote Access
2      MAR-011    9.30   9.3    Volt Typhoon and APT Targeting Critical Infr...
3      MAR-004    9.20   9.2    Ransomware Attacks on Maritime Infrastructure
4      MAR-001    9.10   9.1    GNSS/GPS Spoofing and Jamming
...
```

## Requirements

- Python 3.7+
- PyYAML 6.0.1+

## Data Sources

The tools analyze data from:
- `../vulnerabilities/maritime_vulnerabilities.yaml`
- `../vulnerabilities/threat_actors.yaml`
- `../vulnerabilities/incidents.yaml`

## Methodology

Risk scores are calculated using the OWASP Maritime Security methodology:

```
Risk_Score = (Frequency × 0.25) + (Impact × 0.35) + (Exploitability × 0.20) +
             (Prevalence × 0.15) + (Detection_Difficulty × 0.05)
```

See `../methodology/METHODOLOGY.md` for complete details.

## Development

To extend or modify the analysis tools:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test with the existing data
5. Submit a pull request

### Adding New Analysis Features

The `MaritimeVulnerabilityAnalyzer` class can be extended with additional methods:

```python
from vulnerability_analyzer import MaritimeVulnerabilityAnalyzer

analyzer = MaritimeVulnerabilityAnalyzer()
analyzer.load_data()

# Add custom analysis
def analyze_by_system_type(self):
    # Your analysis code
    pass

# Use the analyzer
results = analyzer.analyze_vulnerabilities()
```

## Future Enhancements

Planned features:
- Visualization generation (charts, graphs)
- Trend analysis over time
- Attack path modeling
- MITRE ATT&CK mapping
- Control effectiveness analysis
- Cost-benefit analysis for mitigations

## Contributing

Contributions welcome! Please ensure:
- Code follows PEP 8 style guidelines
- Functions include docstrings
- New features include usage examples
- Analysis methodology alignment

## License

Creative Commons Attribution-ShareAlike 4.0

## Contact

For questions or suggestions:
- Submit an issue on GitHub
- Contact project leaders via OWASP project page
