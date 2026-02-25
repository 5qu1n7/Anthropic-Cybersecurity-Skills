# Reddit Launch Posts

## Timing Guidance

- Space posts **2 hours apart** to avoid spam detection and maximize individual post visibility.
- Post **Tuesday through Thursday** for best engagement.
- Optimal window: **9:00 AM - 12:00 PM EST**.
- Suggested schedule: first post at 9:00 AM EST, second at 11:00 AM EST, third at 1:00 PM EST, then remaining posts over the following day.
- Do NOT cross-post (use Reddit's crosspost feature). Write unique copy for each subreddit.

---

## 1. r/netsec (~540K subscribers) -- Technical Focus

**Title:** Open-source database of 611+ structured cybersecurity skills for AI agents -- covers DFIR, malware analysis, cloud pentesting, and more

**Body:**

I've been building an open-source database of cybersecurity skills formatted for AI agent consumption. There are 611 skills across 24 subdomains, each following a structured YAML + Markdown format.

What makes this different from a wiki or cheat sheet:

- **Progressive disclosure architecture**: YAML frontmatter tells the agent WHEN to activate (trigger conditions, prerequisites), and the Markdown body provides the HOW (exact commands, tool flags, decision trees).
- **Tool-specific, not generic**: Skills reference specific tools with real commands. "Analyzing Memory Dumps with Volatility" includes the actual `vol3` plugin sequence, not "use a memory forensics tool."
- **Real references**: MITRE ATT&CK technique IDs, NIST control mappings, actual CVE numbers, CIS benchmark references.
- **Practitioner scripts and templates**: Each skill can include helper scripts and filled-in report/checklist templates.

Subdomain breakdown:
- Cloud Security (48 skills) -- AWS, Azure, GCP specific
- Threat Intelligence (43) -- STIX/TAXII, MISP, diamond model
- Web App Security (41) -- OWASP Top 10, specific injection types
- Threat Hunting (35) -- hypothesis-driven, ATT&CK-mapped
- Malware Analysis (34) -- static, dynamic, reverse engineering
- Digital Forensics (34) -- disk, memory, network, mobile
- Plus 18 more subdomains

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills

Format follows the agentskills.io open standard. MIT licensed. Looking for practitioner contributors.

---

## 2. r/cybersecurity (~1M+ subscribers) -- Broader Audience

**Title:** I built an open-source library of 611 cybersecurity skills that AI agents can actually use -- from memory forensics to cloud pentesting

**Body:**

AI coding agents like Claude Code and GitHub Copilot are increasingly used for security tasks, but they lack structured cybersecurity knowledge. When you ask them to analyze a suspicious process or triage a SIEM alert, you get generic advice instead of the specific Volatility plugin, Splunk query, or Nessus configuration a practitioner would use.

I built an open-source database of 611 cybersecurity skills designed to give AI agents real practitioner-level knowledge.

**What each skill includes:**
- When to use it (and when NOT to)
- Tool-specific prerequisites
- Step-by-step workflows with exact commands
- References to MITRE ATT&CK, NIST, CIS benchmarks
- Helper scripts and report templates

**Coverage across 24 subdomains:**
Cloud Security, Threat Intelligence, Web App Security, Threat Hunting, Malware Analysis, Digital Forensics, SOC Operations, Network Security, IAM, OT/ICS Security, API Security, Container Security, Vulnerability Management, Red Teaming, Incident Response, Penetration Testing, Zero Trust, Phishing Defense, Endpoint Security, DevSecOps, Cryptography, Mobile Security, Ransomware Defense, Compliance & Governance.

The skills use a "progressive disclosure" format -- the YAML frontmatter gives the agent enough context to know when to activate, and the full body has the detailed procedure.

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills

MIT licensed. Looking for contributors, especially from practitioners who want to encode their expertise into a format AI agents can use.

---

## 3. r/blueteamsec (~34K subscribers) -- Defensive Focus

**Title:** Open-source skill library for AI-assisted blue team operations -- 611 skills covering DFIR, threat hunting, SOC operations, and detection engineering

**Body:**

Built an open-source database of 611 cybersecurity skills structured for AI agent consumption, with strong coverage of defensive operations:

**Blue team coverage:**
- **Threat Hunting (35 skills)**: Hypothesis-driven hunts for beaconing, LOLBins, persistence mechanisms, DNS tunneling, lateral movement, supply chain compromise
- **SOC Operations (33 skills)**: Alert triage, detection rule building (Sigma, Splunk SPL), SOAR playbooks, escalation matrices, metrics/KPI tracking
- **Incident Response (24 skills)**: Containment procedures, forensic collection, timeline reconstruction, ransomware response, lessons learned
- **Digital Forensics (34 skills)**: Memory forensics with Volatility, disk analysis with Autopsy, network forensics with Wireshark/Zeek, timeline analysis with Plaso
- **Threat Intelligence (43 skills)**: STIX/TAXII integration, MISP feeds, IOC enrichment, threat actor profiling, diamond model analysis
- **Detection Engineering**: Sigma rules, Splunk SPL queries, Suricata rules, Zeek scripts

Each skill includes the exact tool commands, decision trees, and real framework references (MITRE ATT&CK techniques, NIST controls) that a practitioner would use.

The format is designed so AI agents (Claude Code, Copilot, etc.) can use these skills to assist with real security work -- not replace analysts, but give them an AI assistant that actually knows the right Volatility plugin or Splunk query.

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills

MIT licensed. Contributions welcome -- especially from SOC analysts and IR practitioners.

---

## 4. r/hacking

**Title:** 611 cybersecurity skills structured for AI agents -- open-source, covers pentesting, red teaming, malware analysis, forensics, and more

**Body:**

Open-sourced a database of 611 cybersecurity skills that AI agents can use to assist with real security work.

Skills cover both offensive and defensive domains:
- **Penetration Testing (23 skills)**: Web app, network, cloud, mobile, AD, wireless
- **Red Teaming (24 skills)**: C2 infrastructure, lateral movement, persistence, AD attack paths
- **Malware Analysis (34 skills)**: Reverse engineering with Ghidra, dynamic analysis with CAPE/Cuckoo, packed malware unpacking
- **Web App Security (41 skills)**: SQLi, XSS, SSRF, deserialization, race conditions, request smuggling
- **Network Security (33 skills)**: Nmap, Wireshark, Suricata, Zeek, ARP spoofing, VLAN hopping

Each skill has real commands, not pseudocode. The Metasploit skill has actual `msfconsole` commands. The SQLMap skill has actual flags and tamper scripts. The Bloodhound skill has actual Cypher queries.

Format: YAML frontmatter + structured Markdown. Follows the agentskills.io open standard.

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills

MIT licensed. PRs welcome.

---

## 5. r/redteamsec

**Title:** Open-source AI agent skills for red team operations -- AD attack paths, C2 infrastructure, lateral movement, persistence techniques

**Body:**

I built a structured skill database for AI agents that includes significant red team coverage:

- **Red Teaming (24 skills)**: C2 with Sliver/Havoc, AD attack simulation, engagement planning, purple team exercises
- **Penetration Testing (23 skills)**: Full-scope pentesting, AD pentesting, cloud pentesting with Pacu/ScoutSuite, wireless with Aircrack-ng
- **Active Directory**: Bloodhound CE, Kerberoasting with Impacket, DCSync, constrained delegation abuse, NoPac, Zerologon, certificate services ESC1
- **Web exploitation**: SQLi, SSRF, deserialization, template injection, prototype pollution, request smuggling, race conditions

Each skill is structured with YAML frontmatter (triggers, prerequisites, tags) and a Markdown body with exact tool commands, decision trees, and MITRE ATT&CK mappings.

The idea: give AI agents the structured knowledge to assist with authorized security testing, not replace operators but augment them with instant recall of the right tool flag or attack chain.

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills

MIT licensed. Would especially appreciate contributions from red teamers on evasion techniques and emerging TTPs.

---

## 6. r/artificial

**Title:** Built 611 cybersecurity skills for AI agents -- how structured knowledge databases can make AI actually useful for specialized domains

**Body:**

AI coding agents (Claude Code, Cursor, GitHub Copilot) are powerful at general software engineering, but they struggle with specialized domains like cybersecurity. Ask them to analyze a memory dump and you get vague advice. Give them a structured skill file with the exact Volatility plugin sequence and decision tree, and they become genuinely useful.

I built an open-source database of 611 cybersecurity skills structured for AI agent consumption:

**The core insight: progressive disclosure**

The skills use a two-layer architecture:
1. **YAML frontmatter** -- Tells the agent WHEN to activate: skill name, description, domain/subdomain, tags. This is what gets indexed and matched against user queries.
2. **Markdown body** -- The HOW: step-by-step workflows with exact commands, tool flags, decision trees, validation steps. Only loaded when the skill activates.

This mirrors how human expertise works -- a senior analyst doesn't consciously think through every step of memory forensics until they need to, but they know instantly when it's the right approach.

**24 subdomains, 611 skills** covering cloud security, malware analysis, threat hunting, incident response, penetration testing, red teaming, and more.

The format follows the agentskills.io open standard, so any agent framework can index and use these skills.

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills

Interested in the broader question: how do we build domain-specific knowledge layers for AI agents? Cybersecurity is just one domain -- the same pattern could work for medicine, law, finance, etc.

---

## 7. r/opensource

**Title:** Open-sourced 611 cybersecurity skills for AI agents -- MIT licensed, structured for any agent framework

**Body:**

I've open-sourced a database of 611 cybersecurity skills designed for AI agent consumption.

**Why this exists:** AI agents are increasingly used for security tasks, but they lack the structured, tool-specific knowledge that practitioners have. This database encodes that knowledge in a format any AI agent can use.

**What's in it:**
- 611 skills across 24 cybersecurity subdomains
- Each skill: YAML frontmatter + structured Markdown with real commands
- References to MITRE ATT&CK, NIST, CIS benchmarks
- Helper scripts and report templates
- Follows the agentskills.io open standard

**Tech stack:** Pure Markdown + YAML. No build system, no dependencies. Any tool that can read files can use these skills.

**License:** MIT

**Contributing:** Looking for cybersecurity practitioners who want to improve existing skills or add new ones. The format is simple -- if you can write a runbook, you can contribute a skill.

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills
