# Security Assessments Portfolio

## About this project

This portfolio documents hands-on security assessment work across three domains: cloud security, network security, and application security. Each assessment follows a structured methodology: identify the scope, analyze the environment, document findings, and recommend remediations.

The goal is to demonstrate practical cybersecurity skills using real tools and frameworks, not just textbook knowledge. Every finding includes the context of why it matters, how it was discovered, and how to fix it.

## What this covers

| Area | What I did |
|------|-----------|
| **Cloud Security (AWS)** | Hardened a free-tier AWS account: enabled MFA, configured least-privilege IAM policies, set up CloudTrail logging, restricted S3 bucket access |
| **Network Security** | Captured and analyzed network traffic with Wireshark, configured firewall rules in pfSense/iptables, documented a segmented network architecture with DMZ |
| **Application Security** | Used OWASP Juice Shop to identify and document vulnerabilities including SQL injection, XSS, and broken authentication, with remediation strategies for each |

## Tools used

- AWS Free Tier (IAM, CloudTrail, S3)
- Wireshark
- pfSense / iptables
- OWASP Juice Shop
- VirtualBox
- Linux (Ubuntu)
- draw.io (network diagrams)

## Project structure

```
security-assessments/
├── 01-cloud-security-aws/
│   ├── account-hardening.md
│   ├── iam-least-privilege.md
│   ├── cloudtrail-logging.md
│   ├── s3-bucket-policies.md
│   └── screenshots/
├── 02-network-security/
│   ├── wireshark-analysis/
│   │   ├── dns-lookup.md
│   │   ├── tcp-handshake.md
│   │   ├── http-request.md
│   │   ├── arp-discovery.md
│   │   └── pcap-files/
│   ├── firewall-rules.md
│   ├── network-segmentation-diagram.md
│   └── screenshots/
├── 03-application-security/
│   ├── owasp-juice-shop-setup.md
│   ├── findings/
│   │   ├── sql-injection.md
│   │   ├── cross-site-scripting.md
│   │   ├── broken-authentication.md
│   │   ├── sensitive-data-exposure.md
│   │   └── broken-access-control.md
│   ├── assessment-report.md
│   └── screenshots/
└── README.md
```

## Assessment report format

Each finding follows a consistent structure:

```
## Finding: [Vulnerability Name]

**Severity:** Critical / High / Medium / Low
**Domain:** Cloud / Network / Application
**Tool used:** [Tool name]

### Description
What the vulnerability is and why it matters.

### How I found it
Step-by-step walkthrough with screenshots.

### Impact
What an attacker could do if this were exploited.

### Remediation
Specific steps to fix the issue.
```

## Key decisions and rationale

- Why IAM policies use the principle of least privilege rather than broad admin access
- Why Wireshark captures focus on specific protocol scenarios rather than raw dumps
- Why the OWASP assessment prioritizes findings by business impact, not just technical severity
- Why the network architecture uses a DMZ for public-facing services

## Status

- [x] Repository structure created
- [x] AWS Free Tier account active
- [ ] AWS hardening: MFA, IAM, CloudTrail, S3
- [ ] Wireshark captures and analysis
- [ ] Firewall rule documentation
- [ ] Network segmentation diagram
- [ ] OWASP Juice Shop setup
- [ ] Vulnerability findings documented
- [ ] Final assessment report compiled

## Frameworks referenced

- NIST Cybersecurity Framework (CSF)
- OWASP Top 10
- AWS Well-Architected Framework (Security Pillar)
- PCI DSS
- GDPR

## About me

Celest Moreira | B.S. Management Information Systems, Long Beach State (May 2026)
[LinkedIn](https://linkedin.com/in/celest-moreira)
