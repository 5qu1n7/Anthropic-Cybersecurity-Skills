# Hacker News - Show HN Post

## Title

Show HN: 611+ Cybersecurity Skills for AI Agents (agentskills.io open standard)

## Body

I built an open-source database of 611+ cybersecurity skills that AI agents can use to perform real security work -- from malware analysis with Volatility to cloud pen-testing with Pacu.

Each skill follows a structured format (YAML frontmatter + Markdown body) with:

- When to use (and when NOT to)
- Prerequisites and tool requirements
- Step-by-step workflows with real commands, not pseudocode
- References to real standards (NIST, MITRE ATT&CK, CIS)
- Practitioner helper scripts and report templates

The 611 skills cover 24 subdomains: cloud security, threat intelligence, web app security, threat hunting, malware analysis, digital forensics, SOC operations, network security, IAM, OT/ICS security, API security, container security, vulnerability management, red teaming, incident response, penetration testing, zero trust, phishing defense, endpoint security, DevSecOps, cryptography, mobile security, ransomware defense, and compliance/governance.

Why I built this: AI coding agents (Claude Code, Cursor, Copilot) are great at software engineering but have no structured cybersecurity knowledge. When you ask them to analyze a memory dump or triage a SIEM alert, they give generic advice instead of the precise Volatility plugin sequence or Splunk SPL query a practitioner would use.

The skills use "progressive disclosure" -- the frontmatter tells the agent WHEN to activate a skill, and the full body provides the HOW with exact commands, flags, and decision trees.

Format follows the agentskills.io open standard so any agent framework can consume them.

Repo: https://github.com/mukul975/Anthropic-Cybersecurity-Skills

Tech details:
- Each skill has SKILL.md + references/ + scripts/ + assets/
- Skills are tool-specific (not "use a scanner" but "use Nessus with these plugin families")
- Real CVE references, real MITRE ATT&CK technique IDs
- MIT licensed

Looking for contributors, especially practitioners who want to improve existing skills or add new ones in underrepresented areas (mobile security, OT/ICS, compliance).

## Timing

Post at 6:00 AM Pacific (9:00 AM Eastern) for maximum HN visibility. Tuesday through Thursday are optimal days.

## Engagement Rules

1. **Respond within 1 hour** of posting. Early engagement signals to the HN algorithm that the post is active and worth ranking higher.
2. **Be technical, not promotional.** Answer questions with specific technical details. Reference actual skill files, tool commands, and MITRE technique IDs.
3. **No vote requests.** Never ask anyone to upvote. This violates HN guidelines and can get the post flagged or penalized.
4. **Engage authentically.** If someone raises a valid criticism (e.g., "these skills are too shallow for real practitioners"), acknowledge it and explain the contribution model.
5. **Link to specific skills** when answering questions. For example: "Here's the actual Volatility skill that covers that -- [link to SKILL.md]"
6. **Avoid marketing language.** No "revolutionary," "game-changing," or "disrupting." Stick to factual descriptions of what the repo contains.
7. **Be prepared for skepticism.** HN users will question whether AI agents can actually do security work. Have concrete examples ready showing how an agent uses a skill file.
