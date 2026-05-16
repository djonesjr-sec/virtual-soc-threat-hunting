# Virtual SOC Threat Hunting Portfolio

## Overview

This project documents a Virtual SOC threat-hunting portfolio built around Security Onion. The portfolio focuses on threat hunting, enterprise security monitoring, log management, Zeek network analysis, Suricata IDS investigation, PCAP review, and incident-style reporting.

The purpose of this project is to show a practical analyst workflow: identifying suspicious activity, reviewing network evidence, correlating alerts with logs, documenting indicators, and producing clear findings that could support escalation or remediation.

## Project Scope

This portfolio focuses on network-based detection and investigation using Security Onion in a controlled virtual environment. The work emphasizes analyst decision-making, evidence handling, and structured reporting rather than simply displaying tool screenshots.

Focus areas include:

- Threat hunting using Security Onion
- Enterprise security monitoring
- Log review and event analysis
- Zeek network log investigation
- Suricata IDS alert review
- PCAP-based evidence review
- Indicator documentation
- Incident-style reporting
- Analyst workflow development

## Investigation Workflow

The investigation workflow follows a practical SOC-style process:

1. Review Security Onion alerts and identify activity requiring investigation
2. Establish source, destination, protocol, port, and timeline context
3. Pivot into Zeek network logs for connection, DNS, HTTP, and related metadata
4. Review Suricata IDS alerts for detection context
5. Examine PCAP evidence when deeper packet-level review is needed
6. Document indicators, observations, and supporting evidence
7. Produce an incident-style report with findings and recommended next steps

## Tools and Technologies

- Security Onion
- Zeek
- Suricata
- PCAP analysis
- Virtualized environment
- Markdown documentation
- Indicator tracking
- Analyst reporting

## Portfolio Contents

This repository will include:

- Investigation write-ups
- Sanitized Security Onion screenshots
- Zeek log analysis examples
- Suricata alert review examples
- PCAP review notes
- Threat-hunting queries
- Indicator documentation
- Incident-style reports

## Reporting Approach

Each investigation is documented with an emphasis on clarity, evidence, and defensible conclusions. Reports are written to show what was observed, why it mattered, what evidence supported the finding, and what actions would be recommended in a real environment.

## Project Status

In progress.

## Disclaimer

This project is performed in a controlled virtual environment using sanitized, non-production data. No employer, customer, private network, or sensitive information is included.
