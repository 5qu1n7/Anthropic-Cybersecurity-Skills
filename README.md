# Anthropic Cybersecurity Skills

An open-source database of 600+ cybersecurity skills for AI agents, practitioners, and security teams.

## Structure

```
skills/cybersecurity/{skill-name}/
├── SKILL.md          # Skill definition with YAML frontmatter
├── references/
│   ├── standards.md  # Real standard numbers, CVE refs, NIST/MITRE links
│   └── workflows.md  # Deep technical procedure reference
├── scripts/
│   └── process.py    # Real practitioner helper script
└── assets/
    └── template.md   # Real filled-in checklist/report template
```

## Domains Covered

- Web Application Security
- Network Security
- Penetration Testing
- Red Teaming
- Digital Forensics & Incident Response (DFIR)
- Malware Analysis
- Threat Intelligence
- Cloud Security
- Container Security
- Identity & Access Management
- Cryptography
- Vulnerability Management
- Compliance & Governance
- Zero Trust Architecture
- OT/ICS Security
- DevSecOps
- And more...

## Usage

Each `SKILL.md` follows the agentskills.io open standard with YAML frontmatter and structured Markdown body.

## License

MIT
