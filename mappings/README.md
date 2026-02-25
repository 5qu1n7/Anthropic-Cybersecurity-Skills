# Security Framework Mappings

This directory maps the 607+ cybersecurity skills in this repository to industry-standard security frameworks, enabling practitioners and AI agents to discover relevant skills through the lens of established security models.

## Supported Frameworks

### MITRE ATT&CK v15

The [MITRE ATT&CK](https://attack.mitre.org/) framework is a globally accessible knowledge base of adversary tactics and techniques based on real-world observations. Skills are mapped to:

- **Tactics** (TA00xx) -- the adversary's tactical goals during an operation
- **Techniques** (T1xxx) -- the specific methods used to achieve those goals
- **Sub-techniques** (T1xxx.xxx) -- more granular variations of techniques

See [`mitre-attack/`](mitre-attack/) for the full mapping and coverage analysis.

### NIST Cybersecurity Framework 2.0

The [NIST CSF 2.0](https://www.nist.gov/cyberframework) provides a taxonomy of high-level cybersecurity outcomes organized into 6 core functions:

| Function | Code | Description |
|----------|------|-------------|
| Govern | GV | Establishing and monitoring cybersecurity risk management strategy |
| Identify | ID | Understanding organizational cybersecurity risk |
| Protect | PR | Safeguarding assets through security controls |
| Detect | DE | Finding and analyzing cybersecurity events |
| Respond | RS | Taking action regarding detected incidents |
| Recover | RC | Restoring capabilities after an incident |

See [`nist-csf/`](nist-csf/) for the full alignment and category mapping.

### OWASP Top 10 (2025)

The [OWASP Top 10](https://owasp.org/www-project-top-ten/) represents the most critical security risks to web applications. Skills are mapped to each risk category to provide hands-on remediation and testing capabilities.

See [`owasp/`](owasp/) for the full mapping.

## How Mappings Work

Each skill in this repository has YAML frontmatter with `domain`, `subdomain`, and `tags` fields. Framework mappings aggregate skills by subdomain relevance and tag correlation:

```
Skill YAML frontmatter
  -> subdomain (e.g., "penetration-testing")
  -> tags (e.g., ["mitre-attack", "privilege-escalation"])
  -> Framework mapping (e.g., ATT&CK TA0004 Privilege Escalation)
```

Mappings are maintained at the subdomain level for scalability. Individual skills may also carry framework-specific tags in their frontmatter for precise lookups.

## Subdomain Distribution (607 skills)

| Subdomain | Skills | Primary Frameworks |
|-----------|--------|--------------------|
| cloud-security | 48 | ATT&CK, NIST CSF |
| threat-intelligence | 43 | ATT&CK, NIST CSF |
| web-application-security | 41 | ATT&CK, OWASP |
| threat-hunting | 35 | ATT&CK, NIST CSF |
| digital-forensics | 34 | ATT&CK, NIST CSF |
| malware-analysis | 34 | ATT&CK, NIST CSF |
| identity-access-management | 33 | ATT&CK, NIST CSF |
| network-security | 33 | ATT&CK, NIST CSF |
| soc-operations | 33 | ATT&CK, NIST CSF |
| api-security | 28 | OWASP, ATT&CK |
| ot-ics-security | 28 | ATT&CK (ICS), NIST CSF |
| container-security | 26 | ATT&CK, NIST CSF |
| incident-response | 24 | ATT&CK, NIST CSF |
| vulnerability-management | 24 | ATT&CK, NIST CSF, OWASP |
| penetration-testing | 23 | ATT&CK |
| red-teaming | 24 | ATT&CK |
| devsecops | 16 | NIST CSF, OWASP |
| endpoint-security | 16 | ATT&CK, NIST CSF |
| phishing-defense | 16 | ATT&CK, NIST CSF |
| cryptography | 13 | NIST CSF |
| zero-trust-architecture | 13 | NIST CSF |
| mobile-security | 12 | ATT&CK (Mobile), OWASP |
| compliance-governance | 5 | NIST CSF |
| ransomware-defense | 5 | ATT&CK, NIST CSF |

## Contributing

To add or update a framework mapping:

1. Identify the skill subdomain and relevant framework category
2. Update the corresponding mapping file in the framework directory
3. Ensure the skill's YAML frontmatter tags reflect the mapping
4. Submit a pull request with the mapping justification
